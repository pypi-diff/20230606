# Comparing `tmp/django-adminlte-ui-1.7.2.tar.gz` & `tmp/django-adminlte-ui-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-adminlte-ui-1.7.2.tar", last modified: Tue Jul 12 08:57:25 2022, max compression
+gzip compressed data, was "django-adminlte-ui-2.0.0.tar", last modified: Tue Jun  6 05:48:16 2023, max compression
```

## Comparing `django-adminlte-ui-1.7.2.tar` & `django-adminlte-ui-2.0.0.tar`

### file list

```diff
@@ -1,591 +1,582 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.755121 django-adminlte-ui-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1062 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       94 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      966 2022-07-12 08:57:25.755121 django-adminlte-ui-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2956 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      658 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.679121 django-adminlte-ui-1.7.2/adminlteui/
--rw-r--r--   0 runner    (1001) docker     (116)       74 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.679121 django-adminlte-ui-1.7.2/adminlteui/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (116)      246 2022-07-12 08:57:25.000000 django-adminlte-ui-1.7.2/adminlteui/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (116)    14883 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/admin.py
--rw-r--r--   0 runner    (1001) docker     (116)      297 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.671121 django-adminlte-ui-1.7.2/adminlteui/locale/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.671121 django-adminlte-ui-1.7.2/adminlteui/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.679121 django-adminlte-ui-1.7.2/adminlteui/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     3983 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    17514 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.671121 django-adminlte-ui-1.7.2/adminlteui/locale/zh-Hans/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.679121 django-adminlte-ui-1.7.2/adminlteui/locale/zh-Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     3983 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/locale/zh-Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    17514 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/locale/zh-Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.679121 django-adminlte-ui-1.7.2/adminlteui/migrations/
--rw-r--r--   0 runner    (1001) docker     (116)      985 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (116)      411 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/migrations/0002_options_valid.py
--rw-r--r--   0 runner    (1001) docker     (116)     1706 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/migrations/0003_menu.py
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/migrations/0004_auto_20190708_1832.py
--rw-r--r--   0 runner    (1001) docker     (116)      436 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/migrations/0005_menu_priority_level.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3088 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.671121 django-adminlte-ui-1.7.2/adminlteui/static/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.679121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/css/
--rw-r--r--   0 runner    (1001) docker     (116)    57193 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/css/ionicons.css
--rw-r--r--   0 runner    (1001) docker     (116)    51284 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/css/ionicons.min.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.679121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/fonts/
--rw-r--r--   0 runner    (1001) docker     (116)   120724 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/fonts/ionicons.eot
--rw-r--r--   0 runner    (1001) docker     (116)   333834 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/fonts/ionicons.svg
--rw-r--r--   0 runner    (1001) docker     (116)   188508 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/fonts/ionicons.ttf
--rw-r--r--   0 runner    (1001) docker     (116)    67904 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/fonts/ionicons.woff
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.695121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/
--rw-r--r--   0 runner    (1001) docker     (116)    25682 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css
--rw-r--r--   0 runner    (1001) docker     (116)    48005 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css.map
--rw-r--r--   0 runner    (1001) docker     (116)    23411 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (116)    75600 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css.map
--rw-r--r--   0 runner    (1001) docker     (116)   145933 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (116)   390887 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (116)   121457 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (116)   540434 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.699121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/fonts/
--rw-r--r--   0 runner    (1001) docker     (116)    20127 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (116)   108738 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (116)    45404 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (116)    23424 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (116)    18028 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.699121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/js/
--rw-r--r--   0 runner    (1001) docker     (116)    75484 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (116)    39680 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      484 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/js/npm.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.683121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/
--rw-r--r--   0 runner    (1001) docker     (116)    13792 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css
--rw-r--r--   0 runner    (1001) docker     (116)    16046 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css.map
--rw-r--r--   0 runner    (1001) docker     (116)    13084 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     1894 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.683121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/
--rw-r--r--   0 runner    (1001) docker     (116)      557 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/alpha-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (116)      488 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/alpha.png
--rw-r--r--   0 runner    (1001) docker     (116)      478 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/hue-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (116)      504 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/hue.png
--rw-r--r--   0 runner    (1001) docker     (116)     4143 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/saturation.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.683121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/
--rw-r--r--   0 runner    (1001) docker     (116)    38926 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.js
--rw-r--r--   0 runner    (1001) docker     (116)    20771 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.683121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/
--rw-r--r--   0 runner    (1001) docker     (116)    17190 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css
--rw-r--r--   0 runner    (1001) docker     (116)    18548 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css.map
--rw-r--r--   0 runner    (1001) docker     (116)    15731 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.min.css
--rw-r--r--   0 runner    (1001) docker     (116)    18056 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css
--rw-r--r--   0 runner    (1001) docker     (116)    20785 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css.map
--rw-r--r--   0 runner    (1001) docker     (116)    16452 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.min.css
--rw-r--r--   0 runner    (1001) docker     (116)    22835 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css
--rw-r--r--   0 runner    (1001) docker     (116)    23849 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css.map
--rw-r--r--   0 runner    (1001) docker     (116)    21100 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.min.css
--rw-r--r--   0 runner    (1001) docker     (116)    23600 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css
--rw-r--r--   0 runner    (1001) docker     (116)    25703 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css.map
--rw-r--r--   0 runner    (1001) docker     (116)    21734 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.min.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.683121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/
--rw-r--r--   0 runner    (1001) docker     (116)    57898 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.js
--rw-r--r--   0 runner    (1001) docker     (116)    33693 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.695121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/
--rw-r--r--   0 runner    (1001) docker     (116)      636 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker-en-CA.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      704 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar-tn.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      714 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      531 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.az.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      615 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bg.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      562 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bm.min.js
--rw-r--r--   0 runner    (1001) docker     (116)     1210 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bn.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      510 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.br.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      475 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bs.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      513 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ca.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      536 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.cs.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      433 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.cy.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      514 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.da.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      517 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.de.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      764 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.el.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      517 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-AU.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      518 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-CA.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      518 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-GB.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      518 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-IE.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      517 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-NZ.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      517 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-ZA.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      515 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eo.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      513 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.es.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      537 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.et.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      528 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eu.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      670 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fa.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      528 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fi.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      488 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fo.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      512 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr-CH.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      536 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      489 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.gl.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      563 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.he.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      944 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hi.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      462 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hr.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      541 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hu.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      757 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hy.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      453 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.id.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      496 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.is.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      506 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.it-CH.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      525 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.it.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      502 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ja.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      970 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ka.min.js
--rw-r--r--   0 runner    (1001) docker     (116)     1076 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kh.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      649 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kk.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      945 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.km.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      532 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ko.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      575 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kr.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      565 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lt.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      526 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lv.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      493 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.me.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      657 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mk.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      638 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mn.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      448 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ms.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      522 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl-BE.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      513 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      515 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.no.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      515 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.oc.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      552 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pl.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      504 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pt-BR.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      498 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pt.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      505 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ro.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      662 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs-latin.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      817 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      731 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ru.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      988 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.si.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      497 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sk.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      455 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sl.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      518 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sq.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      478 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sr-latin.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      651 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sr.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      492 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sv.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      431 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sw.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      934 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ta.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      700 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tg.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      833 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.th.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      530 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tk.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      495 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tr.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      722 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uk.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      703 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-cyrl.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      516 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-latn.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      551 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.vi.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      613 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-CN.min.js
--rw-r--r--   0 runner    (1001) docker     (116)      566 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-TW.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.695121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-daterangepicker/
--rw-r--r--   0 runner    (1001) docker     (116)     8163 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.css
--rw-r--r--   0 runner    (1001) docker     (116)    71115 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.699121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net/
--rw-r--r--   0 runner    (1001) docker     (116)      889 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net/.bower.json
--rw-r--r--   0 runner    (1001) docker     (116)     1096 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net/License.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2431 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net/Readme.md
--rw-r--r--   0 runner    (1001) docker     (116)      692 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.699121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net/js/
--rw-r--r--   0 runner    (1001) docker     (116)   447569 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.js
--rw-r--r--   0 runner    (1001) docker     (116)    82411 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.699121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/
--rw-r--r--   0 runner    (1001) docker     (116)     1023 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/.bower.json
--rw-r--r--   0 runner    (1001) docker     (116)     1096 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/License.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2272 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/Readme.md
--rw-r--r--   0 runner    (1001) docker     (116)      829 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.699121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/css/
--rw-r--r--   0 runner    (1001) docker     (116)     4791 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (116)     4188 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.699121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/js/
--rw-r--r--   0 runner    (1001) docker     (116)     4559 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (116)     1966 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/fastclick/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.699121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/fastclick/lib/
--rw-r--r--   0 runner    (1001) docker     (116)    25965 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/fastclick/lib/fastclick.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.699121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/css/
--rw-r--r--   0 runner    (1001) docker     (116)    37414 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (116)    21778 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/css/font-awesome.css.map
--rw-r--r--   0 runner    (1001) docker     (116)    31000 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.703121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/fonts/
--rw-r--r--   0 runner    (1001) docker     (116)   134808 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (116)   165742 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (116)   444379 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (116)   165548 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (116)    98024 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (116)    77160 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.703121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/
--rw-r--r--   0 runner    (1001) docker     (116)     9165 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/core.js
--rw-r--r--   0 runner    (1001) docker     (116)   280364 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/jquery.js
--rw-r--r--   0 runner    (1001) docker     (116)    88145 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (116)   136397 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/jquery.min.map
--rw-r--r--   0 runner    (1001) docker     (116)   227022 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/jquery.slim.js
--rw-r--r--   0 runner    (1001) docker     (116)    71037 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.js
--rw-r--r--   0 runner    (1001) docker     (116)   108757 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.map
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/external/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.703121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/external/sizzle/
--rw-r--r--   0 runner    (1001) docker     (116)     1605 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/external/sizzle/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.707121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/external/sizzle/dist/
--rw-r--r--   0 runner    (1001) docker     (116)    65666 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.js
--rw-r--r--   0 runner    (1001) docker     (116)    19841 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.js
--rw-r--r--   0 runner    (1001) docker     (116)    30740 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.map
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.703121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery-slimscroll/
--rw-r--r--   0 runner    (1001) docker     (116)    13832 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.js
--rw-r--r--   0 runner    (1001) docker     (116)     4724 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.707121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/css/
--rw-r--r--   0 runner    (1001) docker     (116)    17340 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/css/select2.css
--rw-r--r--   0 runner    (1001) docker     (116)    14954 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/css/select2.min.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.707121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.715121 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/
--rw-r--r--   0 runner    (1001) docker     (116)      865 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/af.js
--rw-r--r--   0 runner    (1001) docker     (116)      904 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ar.js
--rw-r--r--   0 runner    (1001) docker     (116)      720 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/az.js
--rw-r--r--   0 runner    (1001) docker     (116)      967 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/bg.js
--rw-r--r--   0 runner    (1001) docker     (116)     1290 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/bn.js
--rw-r--r--   0 runner    (1001) docker     (116)      964 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/bs.js
--rw-r--r--   0 runner    (1001) docker     (116)      899 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ca.js
--rw-r--r--   0 runner    (1001) docker     (116)     1291 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/cs.js
--rw-r--r--   0 runner    (1001) docker     (116)      827 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/da.js
--rw-r--r--   0 runner    (1001) docker     (116)      876 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/de.js
--rw-r--r--   0 runner    (1001) docker     (116)     1016 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/dsb.js
--rw-r--r--   0 runner    (1001) docker     (116)     1181 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/el.js
--rw-r--r--   0 runner    (1001) docker     (116)      843 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/en.js
--rw-r--r--   0 runner    (1001) docker     (116)      921 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/es.js
--rw-r--r--   0 runner    (1001) docker     (116)      800 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/et.js
--rw-r--r--   0 runner    (1001) docker     (116)      867 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/eu.js
--rw-r--r--   0 runner    (1001) docker     (116)     1022 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/fa.js
--rw-r--r--   0 runner    (1001) docker     (116)      802 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/fi.js
--rw-r--r--   0 runner    (1001) docker     (116)      923 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/fr.js
--rw-r--r--   0 runner    (1001) docker     (116)      923 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/gl.js
--rw-r--r--   0 runner    (1001) docker     (116)      983 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/he.js
--rw-r--r--   0 runner    (1001) docker     (116)     1174 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/hi.js
--rw-r--r--   0 runner    (1001) docker     (116)      851 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/hr.js
--rw-r--r--   0 runner    (1001) docker     (116)     1017 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/hsb.js
--rw-r--r--   0 runner    (1001) docker     (116)      830 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/hu.js
--rw-r--r--   0 runner    (1001) docker     (116)     1027 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/hy.js
--rw-r--r--   0 runner    (1001) docker     (116)      767 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/id.js
--rw-r--r--   0 runner    (1001) docker     (116)      806 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/is.js
--rw-r--r--   0 runner    (1001) docker     (116)      896 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/it.js
--rw-r--r--   0 runner    (1001) docker     (116)      861 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ja.js
--rw-r--r--   0 runner    (1001) docker     (116)     1194 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ka.js
--rw-r--r--   0 runner    (1001) docker     (116)     1087 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/km.js
--rw-r--r--   0 runner    (1001) docker     (116)      854 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ko.js
--rw-r--r--   0 runner    (1001) docker     (116)      943 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/lt.js
--rw-r--r--   0 runner    (1001) docker     (116)      899 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/lv.js
--rw-r--r--   0 runner    (1001) docker     (116)     1037 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/mk.js
--rw-r--r--   0 runner    (1001) docker     (116)      810 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ms.js
--rw-r--r--   0 runner    (1001) docker     (116)      777 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/nb.js
--rw-r--r--   0 runner    (1001) docker     (116)     1356 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ne.js
--rw-r--r--   0 runner    (1001) docker     (116)      903 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/nl.js
--rw-r--r--   0 runner    (1001) docker     (116)      946 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/pl.js
--rw-r--r--   0 runner    (1001) docker     (116)     1048 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ps.js
--rw-r--r--   0 runner    (1001) docker     (116)      875 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (116)      877 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/pt.js
--rw-r--r--   0 runner    (1001) docker     (116)      937 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ro.js
--rw-r--r--   0 runner    (1001) docker     (116)     1170 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ru.js
--rw-r--r--   0 runner    (1001) docker     (116)     1305 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/sk.js
--rw-r--r--   0 runner    (1001) docker     (116)      924 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/sl.js
--rw-r--r--   0 runner    (1001) docker     (116)      902 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/sq.js
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/sr-Cyrl.js
--rw-r--r--   0 runner    (1001) docker     (116)      979 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/sr.js
--rw-r--r--   0 runner    (1001) docker     (116)      785 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/sv.js
--rw-r--r--   0 runner    (1001) docker     (116)     1073 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/th.js
--rw-r--r--   0 runner    (1001) docker     (116)      770 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/tk.js
--rw-r--r--   0 runner    (1001) docker     (116)      774 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/tr.js
--rw-r--r--   0 runner    (1001) docker     (116)     1155 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/uk.js
--rw-r--r--   0 runner    (1001) docker     (116)      795 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/vi.js
--rw-r--r--   0 runner    (1001) docker     (116)      767 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/zh-CN.js
--rw-r--r--   0 runner    (1001) docker     (116)      706 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/zh-TW.js
--rw-r--r--   0 runner    (1001) docker     (116)   167790 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/select2.full.js
--rw-r--r--   0 runner    (1001) docker     (116)    76652 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/select2.full.min.js
--rw-r--r--   0 runner    (1001) docker     (116)   147864 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/select2.js
--rw-r--r--   0 runner    (1001) docker     (116)    68382 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/select2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.715121 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/
--rw-r--r--   0 runner    (1001) docker     (116)   127585 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/AdminLTE.css
--rw-r--r--   0 runner    (1001) docker     (116)   106548 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/AdminLTE.min.css
--rw-r--r--   0 runner    (1001) docker     (116)   309656 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/adminlte.css.map
--rw-r--r--   0 runner    (1001) docker     (116)   306319 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/adminlte.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.715121 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/
--rw-r--r--   0 runner    (1001) docker     (116)    30145 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.css
--rw-r--r--   0 runner    (1001) docker     (116)    26356 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     1820 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.css
--rw-r--r--   0 runner    (1001) docker     (116)     1469 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     3042 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.css
--rw-r--r--   0 runner    (1001) docker     (116)     2732 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.min.css
--rw-r--r--   0 runner    (1001) docker     (116)    91800 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.css
--rw-r--r--   0 runner    (1001) docker     (116)    75269 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     8606 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/app.css
--rw-r--r--   0 runner    (1001) docker     (116)      566 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/django.css
--rw-r--r--   0 runner    (1001) docker     (116)    16022 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/fontgoogle.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.719121 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/
--rw-r--r--   0 runner    (1001) docker     (116)    48473 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/_all-skins.css
--rw-r--r--   0 runner    (1001) docker     (116)    41635 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/_all-skins.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     4841 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-black-light.css
--rw-r--r--   0 runner    (1001) docker     (116)     4134 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-black-light.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     4163 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-black.css
--rw-r--r--   0 runner    (1001) docker     (116)     3513 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-black.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     4533 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-blue-light.css
--rw-r--r--   0 runner    (1001) docker     (116)     3916 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-blue-light.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     3688 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-blue.css
--rw-r--r--   0 runner    (1001) docker     (116)     3156 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-blue.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     4299 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-green-light.css
--rw-r--r--   0 runner    (1001) docker     (116)     3719 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-green-light.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     3513 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-green.css
--rw-r--r--   0 runner    (1001) docker     (116)     3010 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-green.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     4350 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-purple-light.css
--rw-r--r--   0 runner    (1001) docker     (116)     3768 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-purple-light.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     3560 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-purple.css
--rw-r--r--   0 runner    (1001) docker     (116)     3055 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-purple.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     4197 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-red-light.css
--rw-r--r--   0 runner    (1001) docker     (116)     3621 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-red-light.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     3419 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-red.css
--rw-r--r--   0 runner    (1001) docker     (116)     2920 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-red.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     4350 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-yellow-light.css
--rw-r--r--   0 runner    (1001) docker     (116)     3768 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-yellow-light.min.css
--rw-r--r--   0 runner    (1001) docker     (116)     3560 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-yellow.css
--rw-r--r--   0 runner    (1001) docker     (116)     3055 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-yellow.min.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.719121 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/img/
--rw-r--r--   0 runner    (1001) docker     (116)     1094 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/img/calendar-icons.svg
--rw-r--r--   0 runner    (1001) docker     (116)   223437 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/img/default-log.svg
--rw-r--r--   0 runner    (1001) docker     (116)     7070 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/img/default.jpg
--rw-r--r--   0 runner    (1001) docker     (116)     3291 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/img/selector-icons.svg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.719121 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/js/
--rw-r--r--   0 runner    (1001) docker     (116)    29749 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/js/adminlte.js
--rw-r--r--   0 runner    (1001) docker     (116)    13611 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/js/adminlte.min.js
--rw-r--r--   0 runner    (1001) docker     (116)    18608 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/js/demo.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.723121 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/js/pages/
--rw-r--r--   0 runner    (1001) docker     (116)     6112 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/js/pages/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (116)     9607 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/js/pages/dashboard2.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.723121 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/bootstrap-slider/
--rw-r--r--   0 runner    (1001) docker     (116)    51062 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/bootstrap-slider/bootstrap-slider.js
--rw-r--r--   0 runner    (1001) docker     (116)     8486 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/bootstrap-slider/slider.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.723121 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/bootstrap-wysihtml5/
--rw-r--r--   0 runner    (1001) docker     (116)   566620 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js
--rw-r--r--   0 runner    (1001) docker     (116)   210932 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js
--rw-r--r--   0 runner    (1001) docker     (116)     2553 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css
--rw-r--r--   0 runner    (1001) docker     (116)     2226 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.723121 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/
--rw-r--r--   0 runner    (1001) docker     (116)     1568 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/all.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.727120 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/
--rw-r--r--   0 runner    (1001) docker     (116)    13773 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/_all.css
--rw-r--r--   0 runner    (1001) docker     (116)     1428 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/aero.css
--rw-r--r--   0 runner    (1001) docker     (116)     1520 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/aero.png
--rw-r--r--   0 runner    (1001) docker     (116)     3218 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1428 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/blue.css
--rw-r--r--   0 runner    (1001) docker     (116)     1518 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/blue.png
--rw-r--r--   0 runner    (1001) docker     (116)     3217 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1369 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/flat.css
--rw-r--r--   0 runner    (1001) docker     (116)     1515 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/flat.png
--rw-r--r--   0 runner    (1001) docker     (116)     3217 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/flat@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1443 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/green.css
--rw-r--r--   0 runner    (1001) docker     (116)     1444 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/green.png
--rw-r--r--   0 runner    (1001) docker     (116)     3117 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1428 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/grey.css
--rw-r--r--   0 runner    (1001) docker     (116)     1516 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/grey.png
--rw-r--r--   0 runner    (1001) docker     (116)     3217 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1458 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/orange.css
--rw-r--r--   0 runner    (1001) docker     (116)     1518 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/orange.png
--rw-r--r--   0 runner    (1001) docker     (116)     3275 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1428 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/pink.css
--rw-r--r--   0 runner    (1001) docker     (116)     1522 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/pink.png
--rw-r--r--   0 runner    (1001) docker     (116)     3218 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1458 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/purple.css
--rw-r--r--   0 runner    (1001) docker     (116)     1519 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/purple.png
--rw-r--r--   0 runner    (1001) docker     (116)     3218 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1413 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/red.css
--rw-r--r--   0 runner    (1001) docker     (116)     1516 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/red.png
--rw-r--r--   0 runner    (1001) docker     (116)     3276 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1458 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/yellow.css
--rw-r--r--   0 runner    (1001) docker     (116)     1516 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/yellow.png
--rw-r--r--   0 runner    (1001) docker     (116)     3216 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.727120 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/futurico/
--rw-r--r--   0 runner    (1001) docker     (116)     1421 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/futurico/futurico.css
--rw-r--r--   0 runner    (1001) docker     (116)     1734 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/futurico/futurico.png
--rw-r--r--   0 runner    (1001) docker     (116)     3446 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/futurico/futurico@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)    14161 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/icheck.js
--rw-r--r--   0 runner    (1001) docker     (116)     4516 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/icheck.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.727120 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/
--rw-r--r--   0 runner    (1001) docker     (116)    21689 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/_all.css
--rw-r--r--   0 runner    (1001) docker     (116)     2222 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/aero.css
--rw-r--r--   0 runner    (1001) docker     (116)     2222 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/blue.css
--rw-r--r--   0 runner    (1001) docker     (116)     2244 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/green.css
--rw-r--r--   0 runner    (1001) docker     (116)     2222 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/grey.css
--rw-r--r--   0 runner    (1001) docker     (116)     2103 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/line.css
--rw-r--r--   0 runner    (1001) docker     (116)      588 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/line.png
--rw-r--r--   0 runner    (1001) docker     (116)     1073 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/line@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     2260 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/orange.css
--rw-r--r--   0 runner    (1001) docker     (116)     2222 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/pink.css
--rw-r--r--   0 runner    (1001) docker     (116)     2266 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/purple.css
--rw-r--r--   0 runner    (1001) docker     (116)     2200 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/red.css
--rw-r--r--   0 runner    (1001) docker     (116)     2266 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/yellow.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.731121 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/
--rw-r--r--   0 runner    (1001) docker     (116)    14176 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/_all.css
--rw-r--r--   0 runner    (1001) docker     (116)     1626 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/aero.css
--rw-r--r--   0 runner    (1001) docker     (116)     1151 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/aero.png
--rw-r--r--   0 runner    (1001) docker     (116)     1409 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1626 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/blue.css
--rw-r--r--   0 runner    (1001) docker     (116)     1132 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/blue.png
--rw-r--r--   0 runner    (1001) docker     (116)     1410 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1643 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/green.css
--rw-r--r--   0 runner    (1001) docker     (116)     1143 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/green.png
--rw-r--r--   0 runner    (1001) docker     (116)     1408 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1626 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/grey.css
--rw-r--r--   0 runner    (1001) docker     (116)     1142 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/grey.png
--rw-r--r--   0 runner    (1001) docker     (116)     1407 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1563 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/minimal.css
--rw-r--r--   0 runner    (1001) docker     (116)     1114 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/minimal.png
--rw-r--r--   0 runner    (1001) docker     (116)     1410 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/minimal@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1660 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/orange.css
--rw-r--r--   0 runner    (1001) docker     (116)     1139 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/orange.png
--rw-r--r--   0 runner    (1001) docker     (116)     1407 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1626 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/pink.css
--rw-r--r--   0 runner    (1001) docker     (116)     1150 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/pink.png
--rw-r--r--   0 runner    (1001) docker     (116)     1409 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1660 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/purple.css
--rw-r--r--   0 runner    (1001) docker     (116)     1132 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/purple.png
--rw-r--r--   0 runner    (1001) docker     (116)     1409 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1609 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/red.css
--rw-r--r--   0 runner    (1001) docker     (116)     1130 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/red.png
--rw-r--r--   0 runner    (1001) docker     (116)     1410 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1660 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/yellow.css
--rw-r--r--   0 runner    (1001) docker     (116)     1135 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/yellow.png
--rw-r--r--   0 runner    (1001) docker     (116)     1406 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.731121 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/polaris/
--rw-r--r--   0 runner    (1001) docker     (116)     1557 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/polaris/polaris.css
--rw-r--r--   0 runner    (1001) docker     (116)     6401 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/polaris/polaris.png
--rw-r--r--   0 runner    (1001) docker     (116)    16760 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/polaris/polaris@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.735121 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/
--rw-r--r--   0 runner    (1001) docker     (116)    15591 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/_all.css
--rw-r--r--   0 runner    (1001) docker     (116)     1611 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/aero.css
--rw-r--r--   0 runner    (1001) docker     (116)     2167 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/aero.png
--rw-r--r--   0 runner    (1001) docker     (116)     4455 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/aero@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1611 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/blue.css
--rw-r--r--   0 runner    (1001) docker     (116)     2185 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/blue.png
--rw-r--r--   0 runner    (1001) docker     (116)     4485 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/blue@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1628 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/green.css
--rw-r--r--   0 runner    (1001) docker     (116)     2193 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/green.png
--rw-r--r--   0 runner    (1001) docker     (116)     4498 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/green@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1611 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/grey.css
--rw-r--r--   0 runner    (1001) docker     (116)     2186 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/grey.png
--rw-r--r--   0 runner    (1001) docker     (116)     4483 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/grey@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1645 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/orange.css
--rw-r--r--   0 runner    (1001) docker     (116)     2181 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/orange.png
--rw-r--r--   0 runner    (1001) docker     (116)     4474 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/orange@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1611 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/pink.css
--rw-r--r--   0 runner    (1001) docker     (116)     2189 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/pink.png
--rw-r--r--   0 runner    (1001) docker     (116)     4479 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/pink@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1645 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/purple.css
--rw-r--r--   0 runner    (1001) docker     (116)     2188 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/purple.png
--rw-r--r--   0 runner    (1001) docker     (116)     4501 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/purple@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1594 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/red.css
--rw-r--r--   0 runner    (1001) docker     (116)     2190 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/red.png
--rw-r--r--   0 runner    (1001) docker     (116)     4490 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/red@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1546 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/square.css
--rw-r--r--   0 runner    (1001) docker     (116)     2175 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/square.png
--rw-r--r--   0 runner    (1001) docker     (116)     4478 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/square@2x.png
--rw-r--r--   0 runner    (1001) docker     (116)     1645 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/yellow.css
--rw-r--r--   0 runner    (1001) docker     (116)     2131 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/yellow.png
--rw-r--r--   0 runner    (1001) docker     (116)     4385 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/yellow@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.739121 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/
--rw-r--r--   0 runner    (1001) docker     (116)    22814 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.date.extensions.js
--rw-r--r--   0 runner    (1001) docker     (116)     5315 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.extensions.js
--rw-r--r--   0 runner    (1001) docker     (116)    90539 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.js
--rw-r--r--   0 runner    (1001) docker     (116)     9118 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.numeric.extensions.js
--rw-r--r--   0 runner    (1001) docker     (116)     1576 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.phone.extensions.js
--rw-r--r--   0 runner    (1001) docker     (116)     9392 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.regex.extensions.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.739121 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/phone-codes/
--rw-r--r--   0 runner    (1001) docker     (116)     3631 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-be.json
--rw-r--r--   0 runner    (1001) docker     (116)    39492 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-codes.json
--rw-r--r--   0 runner    (1001) docker     (116)       76 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/phone-codes/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.739121 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/jQueryUI/
--rw-r--r--   0 runner    (1001) docker     (116)   470596 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (116)   240427 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.739121 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/jvectormap/
--rw-r--r--   0 runner    (1001) docker     (116)      826 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.css
--rw-r--r--   0 runner    (1001) docker     (116)    33323 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js
--rw-r--r--   0 runner    (1001) docker     (116)    95062 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-usa-en.js
--rw-r--r--   0 runner    (1001) docker     (116)   144313 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-world-mill-en.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.739121 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/pace/
--rw-r--r--   0 runner    (1001) docker     (116)     2206 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/pace/pace.css
--rw-r--r--   0 runner    (1001) docker     (116)    26566 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/pace/pace.js
--rw-r--r--   0 runner    (1001) docker     (116)     1863 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/pace/pace.min.css
--rw-r--r--   0 runner    (1001) docker     (116)    12507 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/pace/pace.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.743121 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/
--rw-r--r--   0 runner    (1001) docker     (116)    71385 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.js
--rw-r--r--   0 runner    (1001) docker     (116)    38635 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.743121 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/
--rw-r--r--   0 runner    (1001) docker     (116)    10368 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.css
--rw-r--r--   0 runner    (1001) docker     (116)     9336 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.min.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.743121 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/timepicker/
--rw-r--r--   0 runner    (1001) docker     (116)     3475 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.css
--rw-r--r--   0 runner    (1001) docker     (116)    34375 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.js
--rw-r--r--   0 runner    (1001) docker     (116)     3034 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.css
--rw-r--r--   0 runner    (1001) docker     (116)    18685 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.679121 django-adminlte-ui-1.7.2/adminlteui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.743121 django-adminlte-ui-1.7.2/adminlteui/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (116)      300 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/404.html
--rw-r--r--   0 runner    (1001) docker     (116)      623 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/500.html
--rw-r--r--   0 runner    (1001) docker     (116)     1557 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/actions.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.675120 django-adminlte-ui-1.7.2/adminlteui/templates/admin/auth/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.743121 django-adminlte-ui-1.7.2/adminlteui/templates/admin/auth/user/
--rw-r--r--   0 runner    (1001) docker     (116)      350 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/auth/user/add_form.html
--rw-r--r--   0 runner    (1001) docker     (116)     5326 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/auth/user/change_password.html
--rw-r--r--   0 runner    (1001) docker     (116)    31833 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/base.html
--rw-r--r--   0 runner    (1001) docker     (116)     2856 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/base_site.html
--rw-r--r--   0 runner    (1001) docker     (116)     6139 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/change_form.html
--rw-r--r--   0 runner    (1001) docker     (116)     5698 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (116)      386 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/change_list_object_tools.html
--rw-r--r--   0 runner    (1001) docker     (116)     1894 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/change_list_results.html
--rw-r--r--   0 runner    (1001) docker     (116)      742 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/date_hierarchy.html
--rw-r--r--   0 runner    (1001) docker     (116)     3555 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/delete_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (116)     3535 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/delete_selected_confirmation.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.743121 django-adminlte-ui-1.7.2/adminlteui/templates/admin/edit_inline/
--rw-r--r--   0 runner    (1001) docker     (116)     2906 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/edit_inline/stacked.html
--rw-r--r--   0 runner    (1001) docker     (116)     5550 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/edit_inline/tabular.html
--rw-r--r--   0 runner    (1001) docker     (116)     1220 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/filter.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.747121 django-adminlte-ui-1.7.2/adminlteui/templates/admin/includes/
--rw-r--r--   0 runner    (1001) docker     (116)     3896 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/includes/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (116)      188 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/includes/object_delete_summary.html
--rw-r--r--   0 runner    (1001) docker     (116)     7379 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/index.html
--rw-r--r--   0 runner    (1001) docker     (116)      520 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/invalid_setup.html
--rw-r--r--   0 runner    (1001) docker     (116)     5641 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/login.html
--rw-r--r--   0 runner    (1001) docker     (116)     2564 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/object_history.html
--rw-r--r--   0 runner    (1001) docker     (116)     3829 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/pagination.html
--rw-r--r--   0 runner    (1001) docker     (116)     1642 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/search_form.html
--rw-r--r--   0 runner    (1001) docker     (116)     1479 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/submit_line.html
--rw-r--r--   0 runner    (1001) docker     (116)     1760 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/admin/tree_change_list_results.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.751121 django-adminlte-ui-1.7.2/adminlteui/templates/adminlte/
--rw-r--r--   0 runner    (1001) docker     (116)      707 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/adminlte/form.html
--rw-r--r--   0 runner    (1001) docker     (116)     1978 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/adminlte/general_option.html
--rw-r--r--   0 runner    (1001) docker     (116)      747 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/adminlte/menu_change_form.html
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/adminlte/menu_change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.751121 django-adminlte-ui-1.7.2/adminlteui/templates/adminlte/widgets/
--rw-r--r--   0 runner    (1001) docker     (116)      445 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/adminlte/widgets/select.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.751121 django-adminlte-ui-1.7.2/adminlteui/templates/registration/
--rw-r--r--   0 runner    (1001) docker     (116)     2965 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/registration/logged_out.html
--rw-r--r--   0 runner    (1001) docker     (116)      725 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/registration/password_change_done.html
--rw-r--r--   0 runner    (1001) docker     (116)     5828 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templates/registration/password_change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.751121 django-adminlte-ui-1.7.2/adminlteui/templatetags/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6098 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templatetags/adminlte_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     8520 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templatetags/adminlte_menu.py
--rw-r--r--   0 runner    (1001) docker     (116)     2237 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/templatetags/adminlte_options.py
--rw-r--r--   0 runner    (1001) docker     (116)       60 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/tests.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/views.py
--rw-r--r--   0 runner    (1001) docker     (116)     1017 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/adminlteui/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-12 08:57:25.755121 django-adminlte-ui-1.7.2/django_adminlte_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      966 2022-07-12 08:57:25.000000 django-adminlte-ui-1.7.2/django_adminlte_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    33626 2022-07-12 08:57:25.000000 django-adminlte-ui-1.7.2/django_adminlte_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-07-12 08:57:25.000000 django-adminlte-ui-1.7.2/django_adminlte_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-07-12 08:57:25.000000 django-adminlte-ui-1.7.2/django_adminlte_ui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-07-12 08:57:25.000000 django-adminlte-ui-1.7.2/django_adminlte_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2022-07-12 08:57:25.000000 django-adminlte-ui-1.7.2/django_adminlte_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-07-12 08:57:25.755121 django-adminlte-ui-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      689 2022-07-12 08:57:07.000000 django-adminlte-ui-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-06-06 05:48:15.000000 django-adminlte-ui-2.0.0/adminlteui/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5161 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/locale/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    17514 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/locale/zh-Hans/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/locale/zh-Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/locale/zh-Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    17514 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/locale/zh-Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.164289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    57193 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/css/ionicons.css
+-rw-r--r--   0 runner    (1001) docker     (122)    51284 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/css/ionicons.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.164289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   120724 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   333834 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.svg
+-rw-r--r--   0 runner    (1001) docker     (122)   188508 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    67904 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.woff
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.180289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    25682 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (122)    48005 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    23411 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    75600 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)   145933 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (122)   390887 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)   121457 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)   540434 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.180289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)    20127 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   108738 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (122)    45404 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    23424 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    18028 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.180289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    75484 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (122)    39680 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/js/npm.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.164289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    13792 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css
+-rw-r--r--   0 runner    (1001) docker     (122)    16046 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    13084 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.152289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.164289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/alpha-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/alpha.png
+-rw-r--r--   0 runner    (1001) docker     (122)      478 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/hue-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/hue.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4143 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/saturation.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.164289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    38926 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.js
+-rw-r--r--   0 runner    (1001) docker     (122)    20771 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.168289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    17190 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css
+-rw-r--r--   0 runner    (1001) docker     (122)    18548 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    15731 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    18056 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css
+-rw-r--r--   0 runner    (1001) docker     (122)    20785 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    16452 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    22835 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css
+-rw-r--r--   0 runner    (1001) docker     (122)    23849 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    21100 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    23600 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css
+-rw-r--r--   0 runner    (1001) docker     (122)    25703 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    21734 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.168289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    57898 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.js
+-rw-r--r--   0 runner    (1001) docker     (122)    33693 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.176289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker-en-CA.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar-tn.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      714 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.az.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bg.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bm.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bn.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.br.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bs.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ca.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.cs.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.cy.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.da.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.de.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.el.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-AU.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-CA.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-GB.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-IE.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-NZ.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-ZA.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eo.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.es.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.et.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eu.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fa.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fi.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fo.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      512 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr-CH.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.gl.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.he.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hi.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hr.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      541 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hu.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hy.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.id.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.is.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.it-CH.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.it.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ja.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ka.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kh.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kk.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      945 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.km.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ko.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kr.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lt.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lv.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.me.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mk.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mn.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ms.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl-BE.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.no.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.oc.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pl.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pt-BR.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pt.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ro.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs-latin.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ru.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.si.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sk.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sl.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sq.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      478 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sr-latin.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sr.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sv.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sw.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      934 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ta.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tg.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.th.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tk.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tr.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uk.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-cyrl.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-latn.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      551 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.vi.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-CN.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-TW.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.176289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-daterangepicker/
+-rw-r--r--   0 runner    (1001) docker     (122)     8163 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.css
+-rw-r--r--   0 runner    (1001) docker     (122)    71115 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.180289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/
+-rw-r--r--   0 runner    (1001) docker     (122)      889 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/License.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2431 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (122)      692 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/bower.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.184289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/js/
+-rw-r--r--   0 runner    (1001) docker     (122)   447569 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.js
+-rw-r--r--   0 runner    (1001) docker     (122)    82411 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.184289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/.bower.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/License.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/bower.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.184289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     4791 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4188 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.184289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/js/
+-rw-r--r--   0 runner    (1001) docker     (122)     4559 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1966 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/fastclick/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.184289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/fastclick/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)    25965 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/fastclick/lib/fastclick.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.184289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    37414 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (122)    21778 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)    31000 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.188289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   134808 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (122)   165742 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   444379 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (122)   165548 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    98024 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    77160 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.188289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/
+-rw-r--r--   0 runner    (1001) docker     (122)     9165 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/core.js
+-rw-r--r--   0 runner    (1001) docker     (122)   280364 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (122)    88145 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   136397 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.min.map
+-rw-r--r--   0 runner    (1001) docker     (122)   227022 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.js
+-rw-r--r--   0 runner    (1001) docker     (122)    71037 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   108757 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.map
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.188289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.188289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/
+-rw-r--r--   0 runner    (1001) docker     (122)    65666 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.js
+-rw-r--r--   0 runner    (1001) docker     (122)    19841 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)    30740 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.map
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.188289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery-slimscroll/
+-rw-r--r--   0 runner    (1001) docker     (122)    13832 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4724 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.188289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    17340 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/css/select2.css
+-rw-r--r--   0 runner    (1001) docker     (122)    14954 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/css/select2.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.192289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.196289 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/af.js
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ar.js
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/az.js
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/bg.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/bn.js
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/bs.js
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ca.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1291 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/cs.js
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/da.js
+-rw-r--r--   0 runner    (1001) docker     (122)      876 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/de.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/dsb.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/el.js
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/en.js
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/es.js
+-rw-r--r--   0 runner    (1001) docker     (122)      800 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/et.js
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/eu.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/fa.js
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/fi.js
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/fr.js
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/gl.js
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/he.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hi.js
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hr.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hsb.js
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hu.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hy.js
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/id.js
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/is.js
+-rw-r--r--   0 runner    (1001) docker     (122)      896 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/it.js
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ja.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ka.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/km.js
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ko.js
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/lt.js
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/lv.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/mk.js
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ms.js
+-rw-r--r--   0 runner    (1001) docker     (122)      777 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/nb.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ne.js
+-rw-r--r--   0 runner    (1001) docker     (122)      903 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/nl.js
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/pl.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ps.js
+-rw-r--r--   0 runner    (1001) docker     (122)      875 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/pt.js
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ro.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ru.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sk.js
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sl.js
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sq.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sr-Cyrl.js
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sr.js
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sv.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/th.js
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/tk.js
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/tr.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/uk.js
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/vi.js
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/zh-CN.js
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/zh-TW.js
+-rw-r--r--   0 runner    (1001) docker     (122)   167790 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.full.js
+-rw-r--r--   0 runner    (1001) docker     (122)    76652 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.full.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   147864 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.js
+-rw-r--r--   0 runner    (1001) docker     (122)    68382 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.156289 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.200289 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (122)   127585 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/AdminLTE.css
+-rw-r--r--   0 runner    (1001) docker     (122)   106548 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/AdminLTE.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)   309656 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/adminlte.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)   306319 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/adminlte.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.200289 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/
+-rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.css
+-rw-r--r--   0 runner    (1001) docker     (122)    26356 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2732 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    91800 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.css
+-rw-r--r--   0 runner    (1001) docker     (122)    75269 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     8670 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/app.css
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/django.css
+-rw-r--r--   0 runner    (1001) docker     (122)    16022 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/fontgoogle.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.204289 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/
+-rw-r--r--   0 runner    (1001) docker     (122)    48473 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/_all-skins.css
+-rw-r--r--   0 runner    (1001) docker     (122)    41635 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/_all-skins.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4841 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black-light.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4134 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black-light.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4163 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4533 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue-light.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3916 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue-light.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3688 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4299 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green-light.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3719 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green-light.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4350 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple-light.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple-light.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3055 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4197 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red-light.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red-light.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2920 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4350 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow-light.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow-light.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3055 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.204289 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/calendar-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (122)   223437 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/default-log.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     7070 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/default.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)     3291 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/selector-icons.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.204289 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    29749 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/adminlte.js
+-rw-r--r--   0 runner    (1001) docker     (122)    13611 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/adminlte.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)    18608 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/demo.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.204289 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/pages/
+-rw-r--r--   0 runner    (1001) docker     (122)     6112 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/pages/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (122)     9607 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/pages/dashboard2.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.204289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-slider/
+-rw-r--r--   0 runner    (1001) docker     (122)    51062 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-slider/bootstrap-slider.js
+-rw-r--r--   0 runner    (1001) docker     (122)     8486 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-slider/slider.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.208289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/
+-rw-r--r--   0 runner    (1001) docker     (122)   566620 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js
+-rw-r--r--   0 runner    (1001) docker     (122)   210932 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2226 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.208289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/all.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.212289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/
+-rw-r--r--   0 runner    (1001) docker     (122)    13773 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/_all.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/aero.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1520 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/aero.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3218 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/blue.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/blue.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3217 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/flat.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1515 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/flat.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3217 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/flat@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/green.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/green.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/grey.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/grey.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3217 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/orange.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/orange.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3275 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/pink.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/pink.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3218 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/purple.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/purple.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3218 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/red.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/red.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3276 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3216 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.212289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/futurico/
+-rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)    14161 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/icheck.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4516 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/icheck.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.212289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/
+-rw-r--r--   0 runner    (1001) docker     (122)    21689 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/_all.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/aero.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/blue.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/green.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/grey.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/line.css
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/line.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/line@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/orange.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/pink.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/purple.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/red.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/yellow.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.216289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/
+-rw-r--r--   0 runner    (1001) docker     (122)    14176 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/_all.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/aero.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/aero.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/blue.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/blue.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/green.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/green.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1408 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/grey.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1142 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/grey.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/orange.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/orange.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/pink.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/pink.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/purple.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/purple.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/red.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/red.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.216289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/polaris/
+-rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris.css
+-rw-r--r--   0 runner    (1001) docker     (122)     6401 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris.png
+-rw-r--r--   0 runner    (1001) docker     (122)    16760 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.220289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/
+-rw-r--r--   0 runner    (1001) docker     (122)    15591 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/_all.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/aero.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/aero.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/aero@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/blue.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/blue.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4485 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/blue@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/green.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/green.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4498 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/green@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/grey.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/grey.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4483 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/grey@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/orange.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/orange.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4474 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/orange@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/pink.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/pink.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4479 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/pink@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/purple.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2188 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/purple.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4501 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/purple@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/red.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2190 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/red.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4490 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/red@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/square.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2175 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/square.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/square@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/yellow.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4385 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/yellow@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.220289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/
+-rw-r--r--   0 runner    (1001) docker     (122)    22814 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.date.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5315 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (122)    90539 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.js
+-rw-r--r--   0 runner    (1001) docker     (122)     9118 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.numeric.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.phone.extensions.js
+-rw-r--r--   0 runner    (1001) docker     (122)     9392 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.regex.extensions.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.224289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/phone-codes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3631 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-be.json
+-rw-r--r--   0 runner    (1001) docker     (122)    39492 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-codes.json
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/phone-codes/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.224289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jQueryUI/
+-rw-r--r--   0 runner    (1001) docker     (122)   470596 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (122)   240427 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.224289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.css
+-rw-r--r--   0 runner    (1001) docker     (122)    33323 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)    95062 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-usa-en.js
+-rw-r--r--   0 runner    (1001) docker     (122)   144313 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-world-mill-en.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.224289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.css
+-rw-r--r--   0 runner    (1001) docker     (122)    26566 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    12507 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.224289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/
+-rw-r--r--   0 runner    (1001) docker     (122)    71385 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.js
+-rw-r--r--   0 runner    (1001) docker     (122)    38635 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.224289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    10368 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.css
+-rw-r--r--   0 runner    (1001) docker     (122)     9336 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.228289 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.css
+-rw-r--r--   0 runner    (1001) docker     (122)    34375 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)    18685 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.228289 django-adminlte-ui-2.0.0/adminlteui/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/404.html
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/500.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/actions.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.160289 django-adminlte-ui-2.0.0/adminlteui/templates/admin/auth/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.228289 django-adminlte-ui-2.0.0/adminlteui/templates/admin/auth/user/
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/auth/user/add_form.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5326 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/auth/user/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)    25938 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5698 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/change_list_object_tools.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1897 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/change_list_results.html
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/date_hierarchy.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/delete_selected_confirmation.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.228289 django-adminlte-ui-2.0.0/adminlteui/templates/admin/edit_inline/
+-rw-r--r--   0 runner    (1001) docker     (122)     2906 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/edit_inline/stacked.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5550 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/edit_inline/tabular.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/filter.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/adminlteui/templates/admin/includes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/includes/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/includes/object_delete_summary.html
+-rw-r--r--   0 runner    (1001) docker     (122)     7379 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/invalid_setup.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5090 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/login.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/object_history.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3829 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/search_form.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/admin/submit_line.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/adminlteui/templates/adminlte/
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/adminlte/form.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/adminlteui/templates/adminlte/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/adminlte/widgets/select.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/adminlteui/templates/registration/
+-rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/registration/logged_out.html
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/registration/password_change_done.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5828 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templates/registration/password_change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/adminlteui/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templatetags/adminlte_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templatetags/adminlte_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4638 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/templatetags/adminlte_menu.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/adminlteui/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-06 05:48:16.000000 django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    33174 2023-06-06 05:48:16.000000 django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 05:48:16.000000 django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 05:48:15.000000 django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-06 05:48:16.000000 django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-06 05:48:16.232288 django-adminlte-ui-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-06-06 05:48:04.000000 django-adminlte-ui-2.0.0/setup.py
```

### Comparing `django-adminlte-ui-1.7.2/LICENSE` & `django-adminlte-ui-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/locale/zh/LC_MESSAGES/django.mo` & `django-adminlte-ui-2.0.0/adminlteui/locale/zh/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/locale/zh/LC_MESSAGES/django.po` & `django-adminlte-ui-2.0.0/adminlteui/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/locale/zh-Hans/LC_MESSAGES/django.mo` & `django-adminlte-ui-2.0.0/adminlteui/locale/zh-Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/locale/zh-Hans/LC_MESSAGES/django.po` & `django-adminlte-ui-2.0.0/adminlteui/locale/zh-Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/css/ionicons.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/css/ionicons.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/css/ionicons.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/css/ionicons.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/fonts/ionicons.eot` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.eot`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/fonts/ionicons.svg` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.svg`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/fonts/ionicons.ttf` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.ttf`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/Ionicons/fonts/ionicons.woff` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/Ionicons/fonts/ionicons.woff`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.eot` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.svg` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/css/bootstrap-colorpicker.min.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/alpha-horizontal.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/alpha-horizontal.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/saturation.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/img/bootstrap-colorpicker/saturation.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-colorpicker/dist/js/bootstrap-colorpicker.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker.standalone.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/css/bootstrap-datepicker3.standalone.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/js/bootstrap-datepicker.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker-en-CA.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker-en-CA.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar-tn.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar-tn.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ar.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.az.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.az.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bg.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bg.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bm.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bm.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bn.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.bn.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ca.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ca.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.cs.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.cs.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.da.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.da.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.de.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.de.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.el.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.el.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-AU.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-AU.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-CA.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-CA.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-GB.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-GB.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-IE.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-IE.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-NZ.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-NZ.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-ZA.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.en-ZA.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eo.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eo.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.es.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.es.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.et.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.et.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eu.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.eu.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fa.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fa.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fi.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fi.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr-CH.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr-CH.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.fr.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.he.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.he.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hi.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hi.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hu.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hu.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hy.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.hy.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.it.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.it.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ka.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ka.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kh.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kh.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kk.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kk.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.km.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.km.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ko.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ko.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kr.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.kr.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lt.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lt.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lv.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.lv.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mk.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mk.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mn.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.mn.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl-BE.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl-BE.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.nl.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.no.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.no.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.oc.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.oc.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pl.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.pl.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs-latin.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs-latin.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.rs.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ru.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ru.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.si.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.si.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sq.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sq.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sr.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.sr.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ta.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.ta.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tg.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tg.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.th.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.th.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tk.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.tk.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uk.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uk.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-cyrl.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-cyrl.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-latn.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.uz-latn.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.vi.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.vi.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-CN.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-CN.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-TW.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-datepicker/dist/locales/bootstrap-datepicker.zh-TW.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/bootstrap-daterangepicker/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net/.bower.json` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/.bower.json`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net/License.txt` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/License.txt`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net/Readme.md` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/Readme.md`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net/bower.json` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/bower.json`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/.bower.json` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/.bower.json`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/License.txt` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/License.txt`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/Readme.md` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/Readme.md`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/bower.json` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/bower.json`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/css/dataTables.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/datatables.net-bs/js/dataTables.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/fastclick/lib/fastclick.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/fastclick/lib/fastclick.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/css/font-awesome.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/css/font-awesome.css.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/css/font-awesome.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/fonts/FontAwesome.otf` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.eot` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.svg` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.ttf` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff2` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/core.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/core.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/jquery.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/jquery.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/jquery.min.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.min.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/jquery.slim.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/dist/jquery.slim.min.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/external/sizzle/LICENSE.txt` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery/external/sizzle/dist/sizzle.min.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/jquery-slimscroll/jquery.slimscroll.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/css/select2.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/css/select2.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/css/select2.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/af.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/af.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ar.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/az.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/az.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/bg.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/bn.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/bn.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/bs.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ca.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/cs.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/da.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/da.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/de.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/de.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/dsb.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/el.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/el.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/en.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/en.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/es.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/es.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/et.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/et.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/eu.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/fa.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/fi.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/fr.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/gl.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/he.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/he.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/hi.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/hr.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/hsb.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/hu.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/hy.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/id.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/id.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/is.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/is.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/it.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/it.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ja.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ka.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ka.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/km.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/km.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ko.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/lt.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/lv.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/mk.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ms.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/nb.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ne.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ne.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/nl.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/pl.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ps.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/pt-BR.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/pt.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ro.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/ru.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/sk.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/sl.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/sq.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sq.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/sr-Cyrl.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/sr.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/sv.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/th.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/th.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/tk.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/tk.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/tr.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/uk.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/vi.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/zh-CN.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/i18n/zh-TW.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/select2.full.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.full.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/select2.full.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/select2.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/components/select2/dist/js/select2.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/components/select2/dist/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/AdminLTE.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/AdminLTE.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/AdminLTE.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/AdminLTE.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/adminlte.css.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/adminlte.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/adminlte.min.css.map` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/adminlte.min.css.map`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-bootstrap-social.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-fullcalendar.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-select2.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/alt/AdminLTE-without-plugins.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/app.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/app.css`

 * *Files 1% similar despite different names*

```diff
@@ -431,23 +431,27 @@
 input[type="password"] {
     width: 100%;
 }
 
 
 input[type="checkbox"] {
     width: auto;
-    /*height: 26px;*/
+    height: 26px;
     padding: 6px 12px;
     font-size: 14px;
     line-height: 1.42857143;
     color: #555;
     background-color: #fff;
     border: 1px solid #ccc;
 }
 
+.clearable-file-input input[type="checkbox"] {
+    height: auto;
+}
+
 .control-label {
     margin-top: 7px;
 }
 
 ul.errorlist {
     margin: 0;
     padding-left: 5px;
```

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/django.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/django.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/fontgoogle.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/fontgoogle.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/_all-skins.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/_all-skins.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/_all-skins.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/_all-skins.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-black-light.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black-light.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-black-light.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black-light.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-black.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-black.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-black.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-blue-light.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue-light.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-blue-light.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue-light.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-blue.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-blue.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-blue.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-green-light.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green-light.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-green-light.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green-light.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-green.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-green.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-green.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-purple-light.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple-light.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-purple-light.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple-light.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-purple.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-purple.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-purple.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-red-light.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red-light.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-red-light.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red-light.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-red.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-red.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-red.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-yellow-light.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow-light.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-yellow-light.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow-light.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-yellow.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/css/skins/skin-yellow.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/css/skins/skin-yellow.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/img/calendar-icons.svg` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/calendar-icons.svg`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/img/default-log.svg` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/default-log.svg`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/img/default.jpg` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/default.jpg`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/img/selector-icons.svg` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/img/selector-icons.svg`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/js/adminlte.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/adminlte.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/js/adminlte.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/adminlte.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/js/demo.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/demo.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/js/pages/dashboard.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/pages/dashboard.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/dist/js/pages/dashboard2.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/dist/js/pages/dashboard2.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/bootstrap-slider/bootstrap-slider.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-slider/bootstrap-slider.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/bootstrap-slider/slider.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-slider/slider.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.all.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/bootstrap-wysihtml5/bootstrap3-wysihtml5.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/all.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/all.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/_all.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/_all.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/aero.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/aero.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/aero.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/aero.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/aero@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/aero@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/blue.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/blue.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/blue.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/blue.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/blue@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/blue@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/flat.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/flat.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/flat.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/flat.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/flat@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/flat@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/green.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/green.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/green.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/green.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/green@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/green@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/grey.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/grey.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/grey.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/grey.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/grey@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/grey@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/orange.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/orange.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/orange.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/orange.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/orange@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/orange@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/pink.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/pink.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/pink.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/pink.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/pink@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/pink@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/purple.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/purple.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/purple.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/purple.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/purple@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/purple@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/red.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/red.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/red.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/red.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/red@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/red@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/yellow.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/yellow.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/yellow.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/yellow.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/flat/yellow@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/flat/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/futurico/futurico.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/futurico/futurico.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/futurico/futurico@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/futurico/futurico@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/icheck.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/icheck.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/icheck.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/icheck.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/_all.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/_all.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/aero.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/aero.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/blue.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/blue.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/green.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/green.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/grey.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/grey.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/line.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/line.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/line.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/line.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/line@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/line@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/orange.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/orange.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/pink.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/pink.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/purple.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/purple.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/red.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/red.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/line/yellow.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/line/yellow.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/_all.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/_all.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/aero.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/aero.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/aero.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/aero.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/aero@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/aero@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/blue.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/blue.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/blue.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/blue.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/blue@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/blue@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/green.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/green.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/green.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/green.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/green@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/green@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/grey.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/grey.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/grey.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/grey.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/grey@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/grey@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/minimal.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/minimal.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/minimal@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/minimal@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/orange.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/orange.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/orange.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/orange.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/orange@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/orange@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/pink.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/pink.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/pink.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/pink.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/pink@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/pink@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/purple.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/purple.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/purple.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/purple.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/purple@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/purple@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/red.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/red.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/red.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/red.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/red@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/red@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/yellow.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/yellow.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/minimal/yellow@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/minimal/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/polaris/polaris.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/polaris/polaris.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/polaris/polaris@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/polaris/polaris@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/_all.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/_all.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/aero.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/aero.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/aero.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/aero.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/aero@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/aero@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/blue.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/blue.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/blue.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/blue.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/blue@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/blue@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/green.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/green.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/green.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/green.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/green@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/green@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/grey.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/grey.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/grey.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/grey.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/grey@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/grey@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/orange.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/orange.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/orange.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/orange.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/orange@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/orange@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/pink.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/pink.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/pink.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/pink.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/pink@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/pink@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/purple.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/purple.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/purple.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/purple.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/purple@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/purple@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/red.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/red.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/red.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/red.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/red@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/red@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/square.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/square.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/square.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/square.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/square@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/square@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/yellow.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/yellow.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/yellow.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/yellow.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/iCheck/square/yellow@2x.png` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/iCheck/square/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.date.extensions.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.date.extensions.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.extensions.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.extensions.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.numeric.extensions.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.numeric.extensions.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.phone.extensions.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.phone.extensions.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.regex.extensions.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/jquery.inputmask.regex.extensions.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-be.json` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-be.json`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-codes.json` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/input-mask/phone-codes/phone-codes.json`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jQueryUI/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-1.2.2.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-usa-en.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-usa-en.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-world-mill-en.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/jvectormap/jquery-jvectormap-world-mill-en.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/pace/pace.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/pace/pace.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/pace/pace.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/pace/pace.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/pace/pace.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/bootstrap-slider.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/seiyria-bootstrap-slider/css/bootstrap-slider.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.css` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.css`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.js` & `django-adminlte-ui-2.0.0/adminlteui/static/admin/plugins/timepicker/bootstrap-timepicker.min.js`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/500.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/500.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/actions.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/auth/user/change_password.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/base.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/base.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-{% load i18n static adminlte_options adminlte_menu %}<!DOCTYPE html>
+{% load i18n static adminlte_core adminlte_menu %}<!DOCTYPE html>
 {% get_current_language as LANGUAGE_CODE %}{% get_current_language_bidi as LANGUAGE_BIDI %}
 
-{% get_adminlte_settings as adminlte %}
-{% get_adminlte_option 'site_logo' as adminlte_site_logo  %}
+{% get_adminlte_config_class as adminlte %}
 
 <html lang="{{ LANGUAGE_CODE|default:"en-us" }}" {% if LANGUAGE_BIDI %}dir="rtl"{% endif %}>
 <head>
     <meta charset="utf-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <title>{% block title %}{% endblock %}</title>
     <!-- Tell the browser to be responsive to screen width -->
@@ -28,113 +27,94 @@
     {% if adminlte.skin %}
         <link rel="stylesheet" href={% static "admin/dist/css/skins/skin-"|add:adminlte.skin|add:".min.css" %}>
     {% else %}
         <link rel="stylesheet" href={% static "admin/dist/css/skins/_all-skins.min.css" %}>
     {% endif %}
 
     <link rel="stylesheet" href={% static "admin/dist/css/django.css" %}>
-    {% if adminlte_site_logo.valid %}
-        <link rel="apple-touch-icon" href="{{ adminlte_site_logo.site_logo }}">
-        <link rel="icon" href="{{ adminlte_site_logo.site_logo }}">
+    {% if adminlte.site_logo %}
+        <link rel="apple-touch-icon" href="{{ adminlte.site_logo }}">
+        <link rel="icon" href="{{ adminlte.site_logo }}">
     {% else %}
         <link rel="apple-touch-icon" href="{% static "admin/dist/img/default-log.svg" %}">
         <link rel="icon" href="{% static "admin/dist/img/default-log.svg" %}">
     {% endif %}
 
     <!-- HTML5 Shim and Respond.js IE8 support of HTML5 elements and media queries -->
     <!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
     <!--[if lt IE 9]>
     <script src="//oss.maxcdn.com/html5shiv/3.7.3/html5shiv.min.js"></script>
     <script src="//oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
     <![endif]-->
     <!-- Google Font -->
     <link rel="stylesheet" href={% static "admin/dist/css/fontgoogle.css" %}>
 </head>
-<body class="hold-transition skin-{% if adminlte.skin %}{{ adminlte.skin }}{% else %}blue{% endif %} sidebar-mini fixed">
+<body class="hold-transition skin-{% if adminlte.skin %}{{ adminlte.skin }}{% else %}blue{% endif %} sidebar-mini {{ adminlte.sidebar_layout }}">
 <div class="wrapper">
     {% if not is_popup %}
         <header class="main-header">
             <!-- Logo -->
             <a href="{% url 'admin:index' %}" class="logo">
                 <!-- mini logo for sidebar mini 50x50 pixels -->
                 <span class="logo-mini">
-                {% if adminlte_site_logo.valid %}
-                    <img src="{{ adminlte_site_logo.site_logo }}" class="user-image" alt="User Image" style="width:45px;height:45px;padding:5px;">
+                {% if adminlte.site_logo %}
+                    <img src="{{ adminlte.site_logo }}" class="user-image" alt="User Image" style="width:45px;height:45px;padding:5px;">
                 {% else %}
-                    <img src={% static "admin/dist/img/default-log.svg" %} class="user-image" alt="User Image" style="width:45px;height:45px;padding:5px;">
+                    <img src="{% static "admin/dist/img/default-log.svg" %}" class="user-image" alt="User Image" style="width:45px;height:45px;padding:5px;">
                 {% endif %}
             </span>
                 <!-- logo for regular state and mobile devices -->
                 <span class="logo-lg">
-                {% if adminlte_site_logo.valid %}
-                    <img src="{{ adminlte_site_logo.site_logo }}" class="user-image" alt="User Image" style="width:45px;height:45px;padding:5px;">
+                {% if adminlte.site_logo %}
+                    <img src="{{ adminlte.site_logo }}" class="user-image" alt="User Image" style="width:45px;height:45px;padding:5px;">
                 {% else %}
-                    <img src={% static "admin/dist/img/default-log.svg" %} class="user-image" alt="User Image" style="width:45px;height:45px;padding:5px;">
+                    <img src="{% static "admin/dist/img/default-log.svg" %}" class="user-image" alt="User Image" style="width:45px;height:45px;padding:5px;">
                 {% endif %}
-                    <b>
-                    {% get_adminlte_option 'site_header' as adminlte_site_header  %}
-                        {% if adminlte_site_header.valid %}
-                            {{ adminlte_site_header.site_header }}
-                        {% else %}
-                            {{ site_header }}
-                        {% endif %}
-                </b>
+                    <b>{{ site_header }}</b>
             </span>
             </a>
             <!-- Header Navbar: style can be found in header.less -->
             <nav class="navbar navbar-static-top">
                 <!-- Sidebar toggle button-->
                 <a href="javascript:void(0)" class="sidebar-toggle" data-toggle="push-menu" role="button">
                     <span class="sr-only">Toggle navigation</span>
                 </a>
 
                 <div class="navbar-custom-menu" style="float: left;">
                     <ul class="nav navbar-nav top-menu">
-                        {% get_menu request 'top' as app_list %}
-                        {% if app_list %}
-                            {% for app in app_list %}
-                                <li class="dropdown user user-menu">
-                                    <a href="{{ app.admin_url }}">
-                                        <i class="fa {% if app.icon %} {{app.icon}} {% else %}fa-database{% endif %}"></i>
-                                        {{ app.name }}</a>
-                                </li>
-                            {% endfor %}
-                        {% endif %}
+                        {% get_menu request 'top' as menu %}
+                        {{ menu | safe }}
                     </ul>
                 </div>
 
                 <div class="navbar-custom-menu">
                     <ul class="nav navbar-nav">
                         <!-- User Account: style can be found in dropdown.less -->
                         <li class="dropdown user user-menu">
                             <a href="#" class="dropdown-toggle" data-toggle="dropdown">
-                                {% get_adminlte_option 'show_avatar' as adminlte_show_avatar  %}
-                                {% if adminlte_show_avatar.valid and adminlte_show_avatar.show_avatar == 'on' %}
-                                    {% get_adminlte_option 'avatar_field' request as adminlte_avatar_field  %}
-                                    {% if adminlte_avatar_field.valid and adminlte_avatar_field.avatar_field %}
-                                        <img src="{{ adminlte_avatar_field.avatar_field }}" class="user-image" alt="User Image" style="width: 25px; height:25px;">
+                                {% if adminlte.show_avatar %}
+                                    {% if adminlte.avatar_field %}
+                                        <img src="{% eval_obj request adminlte.avatar_field %}" class="user-image" alt="User Image" style="width: 25px; height:25px;">
                                     {% else %}
-                                        <img src={% static "admin/dist/img/default.jpg" %} class="user-image" alt="User Image">
+                                        <img src="{% static "admin/dist/img/default.jpg" %}" class="user-image" alt="User Image" style="width: 25px; height:25px;">
                                     {% endif %}
                                 {% endif %}
-                                <span class="hidden-xs">{{ request.user.username }}</span>
+                                <span class="hidden-xs">{% if adminlte.username_field %}{% eval_obj request adminlte.username_field %}{% else %}{{ request.user.username }}{% endif %}</span>
                             </a>
                             <ul class="dropdown-menu">
                                 <!-- User image -->
-                                {% get_adminlte_option 'show_avatar' as adminlte_show_avatar  %}
-                                {% if adminlte_show_avatar.valid and adminlte_show_avatar.show_avatar == 'on' %}
+                                {% if adminlte.show_avatar %}
                                     <li class="user-header">
-                                        {% get_adminlte_option 'avatar_field' request as adminlte_avatar_field  %}
-                                        {% if adminlte_avatar_field.valid and adminlte_avatar_field.avatar_field %}
-                                            <img src="{{ adminlte_avatar_field.avatar_field }}" class="img-circle" alt="User Image" style="width: 90px; height:90px;">
+                                        {% if adminlte.avatar_field %}
+                                            <img src="{% eval_obj request adminlte.avatar_field %}" class="img-circle" alt="User Image" style="width: 90px; height:90px;">
                                         {% else %}
-                                            <img src={% static "admin/dist/img/default.jpg" %} class="img-circle" alt="User Image">
+                                            <img src="{% static "admin/dist/img/default.jpg" %}" class="img-circle" alt="User Image" style="width: 90px; height:90px;">
                                         {% endif %}
                                         <p>
-                                            {{ request.user.username }} -
+                                            {% if adminlte.username_field %}{% eval_obj request adminlte.username_field %}{% else %}{{ request.user.username }}{% endif %} -
                                             {% if request.user.is_superuser %}
                                                 {% trans "Super manager" %}
                                             {% else %}
                                                 {% if request.user.groups.all %}
                                                     {% for i in request.user.groups.all %}{{ i.name }}{% endfor %}
                                                 {% else %}
                                                     {% trans 'Normal' %}
@@ -142,45 +122,29 @@
                                             {% endif %}
                                             <small>{% trans "Register time" %}： {{ request.user.date_joined }}</small>
                                         </p>
                                     </li>
                                 {% else %}
                                     <li class="user-header" style="height: auto;">
                                         <p>
-                                            {{ request.user.username }} -
+                                            {% if adminlte.username_field %}{% eval_obj request adminlte.username_field %}{% else %}{{ request.user.username }}{% endif %} -
                                             {% if request.user.is_superuser %}
                                                 {% trans "Super manager" %}
                                             {% else %}
                                                 {% if request.user.groups.all %}
                                                     {% for i in request.user.groups.all %}{{ i.name }}{% endfor %}
                                                 {% else %}
                                                     {% trans 'Normal' %}
                                                 {% endif %}
                                             {% endif %}
                                             <small>{% trans "Register time" %}： {{ request.user.date_joined }}</small>
                                         </p>
                                     </li>
                                 {% endif %}
 
-                                <!-- Menu Body -->
-                                <!--<li class="user-body">-->
-                                <!--<div class="row">-->
-                                <!--<div class="col-xs-4 text-center">-->
-                                <!--<a href="#">Followers</a>-->
-                                <!--</div>-->
-                                <!--<div class="col-xs-4 text-center">-->
-                                <!--<a href="#">Sales</a>-->
-                                <!--</div>-->
-                                <!--<div class="col-xs-4 text-center">-->
-                                <!--<a href="#">Friends</a>-->
-                                <!--</div>-->
-                                <!--</div>-->
-                                <!--&lt;!&ndash; /.row &ndash;&gt;-->
-                                <!--</li>-->
-                                <!-- Menu Footer-->
                                 <li class="user-footer">
                                     <div class="pull-left">
                                         <a  href="{% url 'admin:password_change' %}" class="btn btn-default btn-flat">{% trans 'Change password' %}</a>
                                     </div>
                                     <div class="pull-right">
                                         <a href="{% url 'admin:logout' %}" class="btn btn-default btn-flat">{% trans 'Log out' %}</a>
                                     </div>
@@ -198,132 +162,53 @@
             </nav>
         </header>
         <!-- Left side column. contains the logo and sidebar -->
         <aside class="main-sidebar">
             <!-- sidebar: style can be found in sidebar.less -->
             <section class="sidebar">
                 <!-- Sidebar user panel -->
-                {% get_adminlte_option 'show_avatar' as adminlte_show_avatar  %}
-                {% if adminlte_show_avatar.valid and adminlte_show_avatar.show_avatar == 'on' %}
+                {% if adminlte.show_avatar %}
                     <div class="user-panel">
                         <div class="pull-left image">
-                            {% get_adminlte_option 'avatar_field' request as adminlte_avatar_field  %}
-                            {% if adminlte_avatar_field.valid and adminlte_avatar_field.avatar_field %}
-                                <img src="{{ adminlte_avatar_field.avatar_field }}" class="img-circle" alt="User Image">
+                            {% if adminlte.avatar_field %}
+                                <img src="{% eval_obj request adminlte.avatar_field %}" class="img-circle" alt="User Image">
                             {% else %}
-                                <img src={% static "admin/dist/img/default.jpg" %} class="img-circle" alt="User Image">
+                                <img src="{% static "admin/dist/img/default.jpg" %}" class="img-circle" alt="User Image">
                             {% endif %}
                         </div>
                         <div class="pull-left info">
-                            <p>{{ request.user.username }}</p>
+                            <p>{% if adminlte.username_field %}{% eval_obj request adminlte.username_field %}{% else %}{{ request.user.username }}{% endif %}</p>
                             <a href="#"><i class="fa fa-circle text-success"></i> {% trans "Online" %}</a>
                         </div>
                     </div>
                 {% endif %}
                 <!-- search form -->
                 {% if adminlte.search_form %}
                     <form action="#" method="get" class="sidebar-form">
                         <div class="input-group">
                             <input type="text" name="q" class="form-control" placeholder="{% trans 'Search' %}...">
                             <span class="input-group-btn">
-                <button type="submit" name="search" id="search-btn" class="btn btn-flat"><i class="fa fa-search"></i>
-                </button>
-              </span>
+                                <button type="submit" name="search" id="search-btn" class="btn btn-flat"><i class="fa fa-search"></i>
+                                </button>
+                            </span>
                         </div>
                     </form>
                 {% endif %}
                 <!-- /.search form -->
                 <!-- sidebar menu: : style can be found in sidebar.less -->
                 <ul class="sidebar-menu tree" data-widget="tree">
 
                     <li class="header">{% trans 'MAIN NAVIGATION' %}</li>
                     <li>
                         <a id="adminIndex" href="{% url 'admin:index' %}">
                             <i class="fa fa-dashboard"></i> <span>{% trans 'Dashboard' %}</span>
                         </a>
                     </li>
-
-                    {% if adminlte.main_navigation_app %}
-
-                        {% get_menu request as app_list %}
-                        {% if app_list %}
-                            {% for app in app_list %}
-                                {% if app.app_label == adminlte.main_navigation_app %}
-                                    {% for model in app.models %}
-                                        {% if model.admin_url %}
-                                            <li>
-                                                <a href="{{ model.admin_url }}">
-                                                    <i class="fa {% if model.icon %} {{model.icon}} {% else %}fa-circle-o{% endif %}"></i> <span>{{ model.name }}</span>
-                                                </a>
-                                            </li>
-                                        {% endif %}
-                                    {% endfor %}
-                                {% endif %}
-                            {% endfor %}
-                        {% endif %}
-
-                    {% endif %}
-
-                    {% if adminlte.navigation_expanded %}
-
-                        {% get_menu request as app_list %}
-                        {% if app_list %}
-                            {% for app in app_list %}
-                                {% if not adminlte.show_apps or adminlte.show_apps and not app.app_label or app.app_label in adminlte.show_apps %}
-                                    {% if not app.app_label or app.app_label != adminlte.main_navigation_app %}
-                                        <li class="header">{{ app.name|upper }}</li>
-                                        {% for model in app.models %}
-                                            {% ifchanged %}
-                                                {% if model.admin_url %}
-                                                    <li>
-                                                        <a href="{{ model.admin_url }}">
-                                                            <i class="fa {% if model.icon %} {{model.icon}} {% else %}fa-circle-o{% endif %}"></i> <span>{{ model.name }}</span>
-                                                        </a>
-                                                    </li>
-                                                {% endif %}
-                                            {% endifchanged %}
-                                        {% endfor %}
-                                    {% endif %}
-                                {% endif %}
-                            {% endfor %}
-                        {% endif %}
-
-                    {% else %}
-
-                        {% get_menu request as app_list %}
-                        {% if app_list %}
-                            {% for app in app_list %}
-                                {% if not adminlte.show_apps or adminlte.show_apps and not app.app_label or app.app_label in adminlte.show_apps %}
-                                    {% if not app.app_label or app.app_label != adminlte.main_navigation_app %}
-                                        <li {% if not app.admin_url %}class="treeview"{% endif %}>
-                                            <a href="{% if app.admin_url %}{{app.admin_url}}{% else %}javascript:void(0){% endif %}">
-                                                <i class="fa {% if app.icon %} {{app.icon}} {% else %}fa-database{% endif %}"></i>
-                                                <span style="overflow: hidden; display: inline-block; vertical-align:top;">{{ app.name }}</span>
-                                                {% if not app.admin_url %}
-                                                    <span class="pull-right-container">
-                                  <i class="fa fa-angle-left pull-right"></i>
-                                </span>
-                                                {% endif %}
-                                            </a>
-                                            {% if not app.admin_url %}
-                                                <ul class="treeview-menu">
-                                                    {% for model in app.models %}
-                                                        {% if model.admin_url %}
-                                                            <li><a href="{{ model.admin_url }}" ><i class="fa {% if model.icon %} {{model.icon}} {% else %}fa-circle-o{% endif %}"></i>{{ model.name }}</a></li>
-                                                        {% endif %}
-                                                    {% endfor %}
-                                                </ul>
-                                            {% endif %}
-                                        </li>
-                                    {% endif %}
-                                {% endif %}
-                            {% endfor %}
-                        {% endif %}
-
-                    {% endif %}
+                    {% get_menu request as menu %}
+                    {{ menu | safe }}
                 </ul>
             </section>
             <!-- /.sidebar -->
         </aside>
     {% endif %}
     <!-- Content Wrapper. Contains page content -->
     <div class="content-wrapper" {% if is_popup %}style="margin-left:0px; padding-top: 0px;"{% endif %}>
@@ -555,49 +440,78 @@
 {% if adminlte.demo %}
     <script src={% static "admin/dist/js/demo.js" %}></script>
 {% endif %}
 <script>
     // use js control active status of siderbar-menu
     $(function() {
         var menuActions = document.querySelectorAll('.sidebar-menu a')
+        var pathname = document.querySelector('#adminIndex').pathname
         for (var i in menuActions) {
-            var pathname = document.querySelector('#adminIndex').pathname
-
             try {
                 if (window.location.pathname === pathname) {
                     menuActions[i].parentNode.setAttribute('class', 'active')
                     break
                 }
 
                 if (window.location.href.indexOf(menuActions[i].href) !== -1) {
                     if (menuActions[i].href===window.location.origin + pathname) {
                         continue
                     }
                     console.log('menu matched.', window.location.href, menuActions[i].href);
                     menuActions[i].parentNode.setAttribute('class', 'active');
-                    if (menuActions[i].parentNode.parentNode.getAttribute('class') !== 'sidebar-menu') {
-                        menuActions[i].parentNode.parentNode.setAttribute('class', 'treeview-menu menu-open');
-                        menuActions[i].parentNode.parentNode.parentNode.setAttribute('class', 'treeview active');
+
+                    let parent = menuActions[i].parentNode;
+                    while (true) {
+                        if (parent.parentNode.getAttribute('class') !== 'sidebar-menu tree') {
+                            if (parent.parentNode.getAttribute('class').indexOf('treeview-menu') !== -1) {
+                                parent.parentNode.setAttribute('class', 'treeview-menu menu-open');
+                                parent.parentNode.parentNode.setAttribute('class', 'treeview active');
+                            }
+                            parent = parent.parentNode;
+                        } else {
+                            break
+                        }
                     }
                     break
                 }
             } catch (e) {
                 console.log(window.location.href, menuActions[i].href, e)
             }
         }
 
         var topMenuActions = document.querySelectorAll('.top-menu a')
         for (var j in topMenuActions) {
             if (window.location.href.indexOf(topMenuActions[j].href) !== -1) {
                 topMenuActions[j].parentNode.setAttribute('class', 'active');
+                if (topMenuActions[j].parentNode.parentNode.getAttribute('class') === 'dropdown-menu') {
+                    topMenuActions[j].parentNode.parentNode.parentNode.setAttribute('class', 'dropdown active');
+                }
                 console.log('top menu matched.', window.location.href, topMenuActions[j].href);
             }
         }
-
-
     })
 </script>
 
+<script>
+    // sidebar push menu control
+    $(function () {
+        $("body")
+            .on("expanded.pushMenu", function() {
+                localStorage.setItem('sidebarStatus', 'expanded')
+            })
+            .on("collapsed.pushMenu", function() {
+            localStorage.setItem('sidebarStatus', 'collapsed')
+        });
+        let sidebarStatus = localStorage.getItem('sidebarStatus');
+        console.log(sidebarStatus)
+        if (sidebarStatus === 'collapsed') {
+            $('body').addClass('sidebar-collapse');
+        } else {
+            $('body').removeClass('sidebar-collapse');
+        }
+    });
+</script>
+
 {% block extrajs %}{% endblock %}
 
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,112 +1,74 @@
-{% load i18n static adminlte_options adminlte_menu %}
+{% load i18n static adminlte_core adminlte_menu %}
  {% get_current_language as LANGUAGE_CODE %}{% get_current_language_bidi as
-LANGUAGE_BIDI %} {% get_adminlte_settings as adminlte %} {% get_adminlte_option
-'site_logo' as adminlte_site_logo %}
+LANGUAGE_BIDI %} {% get_adminlte_config_class as adminlte %}
  }}" {% if LANGUAGE_BIDI %}dir="rtl"{% endif %}>
 
 
 
 admin/components/bootstrap/dist/css/bootstrap.min.css" %}>
 admin/components/font-awesome/css/font-awesome.min.css" %}>
 admin/components/Ionicons/css/ionicons.min.css" %}> {% block extrastyle %} {%
 endblock %} {% block extrahead %} {% endblock %}
 admin/dist/css/AdminLTE.min.css" %}>  {% if adminlte.skin %}
 admin/dist/css/skins/skin-"|add:adminlte.skin|add:".min.css" %}> {% else %}
 admin/dist/css/skins/_all-skins.min.css" %}> {% endif %}
-admin/dist/css/django.css" %}> {% if adminlte_site_logo.valid %}
+admin/dist/css/django.css" %}> {% if adminlte.site_logo %}
 
  {% else %}
 ist/img/default-log.svg" %}">
 ist/img/default-log.svg" %}"> {% endif %}
 admin/dist/css/fontgoogle.css" %}>
-{% if not is_popup %}   __{%_if_adminlte_site_logo.valid_%}_[User_Image]_{%
-else_%}_admin/dist/img/default-log.svg"_%}_class="user-image"_alt="User_Image"
-style="width:45px;height:45px;padding:5px;">_{%_endif_%}____{%_if
-adminlte_site_logo.valid_%}_[User_Image]_{%_else_%}_admin/dist/img/default-
-log.svg"_%}_class="user-image"_alt="User_Image"_style="width:45px;height:
-45px;padding:5px;">_{%_endif_%}_{%_get_adminlte_option_'site_header'_as
-adminlte_site_header_%}_{%_if_adminlte_site_header.valid_%}_{
-{_adminlte_site_header.site_header_}}_{%_else_%}_{{_site_header_}}_{%_endif_%}
-Toggle_navigation
-    * {% get_menu request 'top' as app_list %} {% if app_list %} {% for app in
-      app_list %}
-    *  {{_app.name_}}
-    * {% endfor %} {% endif %}
-    * {%_get_adminlte_option_'show_avatar'_as_adminlte_show_avatar_%}_{%_if
-      adminlte_show_avatar.valid_and_adminlte_show_avatar.show_avatar_==_'on'
-      %}_{%_get_adminlte_option_'avatar_field'_request_as_adminlte_avatar_field
-      %}_{%_if_adminlte_avatar_field.valid_and
-      adminlte_avatar_field.avatar_field_%}_[User_Image]_{%_else_%}_admin/dist/
-      img/default.jpg"_%}_class="user-image"_alt="User_Image">_{%_endif_%}_{%
-      endif_%}_{{_request.user.username_}}
-          o  {% get_adminlte_option 'show_avatar' as adminlte_show_avatar %} {%
-            if adminlte_show_avatar.valid and adminlte_show_avatar.show_avatar
-            == 'on' %}
-          o {% get_adminlte_option 'avatar_field' request as
-            adminlte_avatar_field %} {% if adminlte_avatar_field.valid and
-            adminlte_avatar_field.avatar_field %} [User Image] {% else %}
-            admin/dist/img/default.jpg" %} class="img-circle" alt="User Image">
-            {% endif %}
-            {{ request.user.username }} - {% if request.user.is_superuser %} {%
-            trans "Super manager" %} {% else %} {% if request.user.groups.all
-            %} {% for i in request.user.groups.all %}{{ i.name }}{% endfor %}
-            {% else %} {% trans 'Normal' %} {% endif %} {% endif %} {% trans
-            "Register time" %}ï¼ {{ request.user.date_joined }}
+{% if not is_popup %}   __{%_if_adminlte.site_logo_%}_[User_Image]_{%_else_%}
+ist/img/default-log.svg"_%}"_class="user-image"_alt="User_Image"_style="width:
+45px;height:45px;padding:5px;">_{%_endif_%}____{%_if_adminlte.site_logo_%}_
+[User_Image]_{%_else_%}_ist/img/default-log.svg"_%}"_class="user-image"
+alt="User_Image"_style="width:45px;height:45px;padding:5px;">_{%_endif_%}_{
+{_site_header_}}_    Toggle_navigation
+    * {% get_menu request 'top' as menu %} {{ menu | safe }}
+    * {%_if_adminlte.show_avatar_%}_{%_if_adminlte.avatar_field_%}_[User_Image]
+      {%_else_%}_ist/img/default.jpg"_%}"_class="user-image"_alt="User_Image"
+      style="width:_25px;_height:25px;">_{%_endif_%}_{%_endif_%}_{%_if
+      adminlte.username_field_%}{%_eval_obj_request_adminlte.username_field_%}
+      {%_else_%}{{_request.user.username_}}{%_endif_%}
+          o  {% if adminlte.show_avatar %}
+          o {% if adminlte.avatar_field %} [User Image] {% else %} ist/img/
+            default.jpg" %}" class="img-circle" alt="User Image" style="width:
+            90px; height:90px;"> {% endif %}
+            {% if adminlte.username_field %}{% eval_obj request
+            adminlte.username_field %}{% else %}{{ request.user.username }}{%
+            endif %} - {% if request.user.is_superuser %} {% trans "Super
+            manager" %} {% else %} {% if request.user.groups.all %} {% for i in
+            request.user.groups.all %}{{ i.name }}{% endfor %} {% else %} {%
+            trans 'Normal' %} {% endif %} {% endif %} {% trans "Register time"
+            %}ï¼ {{ request.user.date_joined }}
           o {% else %}
-          o {{ request.user.username }} - {% if request.user.is_superuser %} {%
-            trans "Super manager" %} {% else %} {% if request.user.groups.all
-            %} {% for i in request.user.groups.all %}{{ i.name }}{% endfor %}
-            {% else %} {% trans 'Normal' %} {% endif %} {% endif %} {% trans
-            "Register time" %}ï¼ {{ request.user.date_joined }}
+          o {% if adminlte.username_field %}{% eval_obj request
+            adminlte.username_field %}{% else %}{{ request.user.username }}{%
+            endif %} - {% if request.user.is_superuser %} {% trans "Super
+            manager" %} {% else %} {% if request.user.groups.all %} {% for i in
+            request.user.groups.all %}{{ i.name }}{% endfor %} {% else %} {%
+            trans 'Normal' %} {% endif %} {% endif %} {% trans "Register time"
+            %}ï¼ {{ request.user.date_joined }}
           o {% endif %}
           o {%_trans_'Change_password'_%}
             {%_trans_'Log_out'_%}
     * {% if adminlte.demo %}  {% endif %}
-       {% get_adminlte_option 'show_avatar' as adminlte_show_avatar %} {% if
-adminlte_show_avatar.valid and adminlte_show_avatar.show_avatar == 'on' %}
-{% get_adminlte_option 'avatar_field' request as adminlte_avatar_field %} {% if
-adminlte_avatar_field.valid and adminlte_avatar_field.avatar_field %} [User
-Image] {% else %}
-admin/dist/img/default.jpg" %} class="img-circle" alt="User Image"> {% endif %}
-{{ request.user.username }}
+       {% if adminlte.show_avatar %}
+{% if adminlte.avatar_field %} [User Image] {% else %}
+ist/img/default.jpg" %}" class="img-circle" alt="User Image"> {% endif %}
+{% if adminlte.username_field %}{% eval_obj request adminlte.username_field %}
+{% else %}{{ request.user.username }}{% endif %}
  {%_trans_"Online"_%}
 {% endif %}  {% if adminlte.search_form %}
 [q                   ]
 {% endif %}
     * {% trans 'MAIN NAVIGATION' %}
     *  {%_trans_'Dashboard'_%}
-    * {% if adminlte.main_navigation_app %} {% get_menu request as app_list %}
-      {% if app_list %} {% for app in app_list %} {% if app.app_label ==
-      adminlte.main_navigation_app %} {% for model in app.models %} {% if
-      model.admin_url %}
-    *  {{_model.name_}}
-    * {% endif %} {% endfor %} {% endif %} {% endfor %} {% endif %} {% endif %}
-      {% if adminlte.navigation_expanded %} {% get_menu request as app_list %}
-      {% if app_list %} {% for app in app_list %} {% if not adminlte.show_apps
-      or adminlte.show_apps and not app.app_label or app.app_label in
-      adminlte.show_apps %} {% if not app.app_label or app.app_label !=
-      adminlte.main_navigation_app %}
-    * {{ app.name|upper }}
-    * {% for model in app.models %} {% ifchanged %} {% if model.admin_url %}
-    *  {{_model.name_}}
-    * {% endif %} {% endifchanged %} {% endfor %} {% endif %} {% endif %} {%
-      endfor %} {% endif %} {% else %} {% get_menu request as app_list %} {% if
-      app_list %} {% for app in app_list %} {% if not adminlte.show_apps or
-      adminlte.show_apps and not app.app_label or app.app_label in
-      adminlte.show_apps %} {% if not app.app_label or app.app_label !=
-      adminlte.main_navigation_app %}
-    * % if not app.admin_url %}class="treeview"{% endif %}>
-       {{_app.name_}}_{%_if_not_app.admin_url_%}____{%_endif_%}
-       {% if not app.admin_url %}
-          o {% for model in app.models %} {% if model.admin_url %}
-          o {{_model.name_}}
-          o {% endif %} {% endfor %}
-    * {% endif %}
-{% endif %} {% endif %} {% endfor %} {% endif %} {% endif %}
+    * {% get_menu request as menu %} {{ menu | safe }}
    {% endif %}
 % if is_popup %}style="margin-left:0px; padding-top: 0px;"{% endif %}>  {%
 block page_content %} {% endblock %}
  {% if not is_popup %}  {% block footer %} {% endblock %}
 **** Recent Activity ****
     * ***_Langdon's_Birthday_***
       Will_be_23_on_April_24th
```

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/base_site.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/base_site.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,77 @@
 {% extends 'admin/base.html' %}
-{% load i18n adminlte_options %}
-{% block title %}{{ title }} |
-{% get_adminlte_option 'site_title' as adminlte_site_title %}
-{% if adminlte_site_title.valid %}
-{{ adminlte_site_title.site_title }}
-{% else %}
-{{ site_title|default:_('Django site admin') }}
-{% endif %}
+{% load i18n adminlte_core %}
+{% block title %}
+    {{ title }} | {{ site_title|default:_('Django site admin') }}
 {% endblock %}
 {% block page_content %}
 
-<body class="{% if is_popup %}popup {% endif %}{% block bodyclass %}{% endblock %}"
-      data-admin-utc-offset="{% now "Z" %}">
+    <body class="{% if is_popup %}popup {% endif %}{% block bodyclass %}{% endblock %}"
+          data-admin-utc-offset="{% now "Z" %}">
 
-<!-- Container -->
-<div id="container">
-    {% if not is_popup %}
-    <section class="content-header">
-        <h1>{% block content_title %}{% endblock %}</h1>
-        {% block breadcrumbs %}{% endblock %}
-    </section>
-    {% endif %}
-
-    <!-- Content -->
-    <section id="content" class="content">
-        {% block messages %}
-        {% if messages %}
-        {% for message in messages %}
-        {% if message.tags == 'success' %}
-        <div class="alert alert-success alert-dismissible">
-            <button type="button" class="close" data-dismiss="alert" aria-hidden="true">×</button>
-            <h5><i class="icon fa fa-check"></i>{{ message|capfirst }}</h5>
-        </div>
-        {% elif message.tags == 'error' %}
-        <div class="alert alert-danger alert-dismissible">
-            <button type="button" class="close" data-dismiss="alert" aria-hidden="true">×</button>
-            <h5><i class="icon fa fa-ban"></i>{{ message|capfirst }}</h5>
-        </div>
-        {% elif message.tags == 'warning' %}
-        <div class="alert alert-warning alert-dismissible">
-            <button type="button" class="close" data-dismiss="alert" aria-hidden="true">×</button>
-            <h5><i class="icon fa fa-warning"></i>{{ message|capfirst }}</h5>
-        </div>
-        {% elif message.tags == 'info' %}
-        <div class="alert alert-info alert-dismissible">
-            <button type="button" class="close" data-dismiss="alert" aria-hidden="true">×</button>
-            <h5><i class="icon fa fa-info"></i>{{ message|capfirst }}</h5>
-        </div>
+    <!-- Container -->
+    <div id="container">
+        {% if not is_popup %}
+            <section class="content-header">
+                <h1>{% block content_title %}{% endblock %}</h1>
+                {% block breadcrumbs %}{% endblock %}
+            </section>
         {% endif %}
-        {% endfor %}
-        {% endif %}
-        {% endblock messages %}
-        <div class="row">
-            <div class="col-md-12">
-                {% block content %} {% endblock %}
+
+        <!-- Content -->
+        <section id="content" class="content">
+            {% block messages %}
+                {% if messages %}
+                    {% for message in messages %}
+                        {% if message.tags == 'success' %}
+                            <div class="alert alert-success alert-dismissible">
+                                <button type="button" class="close" data-dismiss="alert" aria-hidden="true">×</button>
+                                <h5><i class="icon fa fa-check"></i>{{ message|capfirst }}</h5>
+                            </div>
+                        {% elif message.tags == 'error' %}
+                            <div class="alert alert-danger alert-dismissible">
+                                <button type="button" class="close" data-dismiss="alert" aria-hidden="true">×</button>
+                                <h5><i class="icon fa fa-ban"></i>{{ message|capfirst }}</h5>
+                            </div>
+                        {% elif message.tags == 'warning' %}
+                            <div class="alert alert-warning alert-dismissible">
+                                <button type="button" class="close" data-dismiss="alert" aria-hidden="true">×</button>
+                                <h5><i class="icon fa fa-warning"></i>{{ message|capfirst }}</h5>
+                            </div>
+                        {% elif message.tags == 'info' %}
+                            <div class="alert alert-info alert-dismissible">
+                                <button type="button" class="close" data-dismiss="alert" aria-hidden="true">×</button>
+                                <h5><i class="icon fa fa-info"></i>{{ message|capfirst }}</h5>
+                            </div>
+                        {% endif %}
+                    {% endfor %}
+                {% endif %}
+            {% endblock messages %}
+            <div class="row">
+                <div class="col-md-12">
+                    {% block content %} {% endblock %}
+                </div>
             </div>
-        </div>
-    </section>
-    <!-- END Content -->
+        </section>
+        <!-- END Content -->
 
-</div>
-<!-- END Container -->
+    </div>
+    <!-- END Container -->
 
 {% endblock %}
 
 {% block footer %}
-<div class="pull-right hidden-xs">
-    <b>Adminlte Version</b> 2.4.18
-</div>
-<strong>
-Copyright &copy; {% now 'Y' %}
-{% if adminlte.copyright %}
-    {{ adminlte.copyright }}.
-{% else %}
-    {% get_adminlte_version as adminlte_version %}
-    <a href="https://github.com/wuyue92tree/django-adminlte-ui/tree/{{ adminlte_version }}">django-adminlte-ui {{ adminlte_version }}</a>.
-{% endif %}
-</strong> All rights reserved.
+    <div class="pull-right hidden-xs">
+        <b>Adminlte Version</b> 2.4.18
+    </div>
+    <strong>
+        Copyright &copy; {% now 'Y' %}
+        {% if adminlte.copyright %}
+            {{ adminlte.copyright }}.
+        {% else %}
+            {% get_adminlte_version as adminlte_version %}
+            <a href="https://github.com/wuyue92tree/django-adminlte-ui/tree/{{ adminlte_version }}">django-adminlte-ui {{ adminlte_version }}</a>.
+        {% endif %}
+    </strong> All rights reserved.
 {% endblock %}
 
 {% block extrajs %} {% endblock %}
```

#### html2text {}

```diff
@@ -1,12 +1,10 @@
-{% extends 'admin/base.html' %} {% load i18n adminlte_options %} {% block title
-%}{{ title }} | {% get_adminlte_option 'site_title' as adminlte_site_title %}
-{% if adminlte_site_title.valid %} {{ adminlte_site_title.site_title }} {% else
-%} {{ site_title|default:_('Django site admin') }} {% endif %} {% endblock %}
-{% block page_content %}
+{% extends 'admin/base.html' %} {% load i18n adminlte_core %} {% block title %}
+{{ title }} | {{ site_title|default:_('Django site admin') }} {% endblock %} {%
+block page_content %}
  %}">
 {% if not is_popup %}
 ****** {% block content_title %}{% endblock %} ******
 {% block breadcrumbs %}{% endblock %}  {% endif %}   {% block messages %} {% if
 messages %} {% for message in messages %} {% if message.tags == 'success' %}
 Ã
 {{ message|capfirst }}
```

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/change_form.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/change_list.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/change_list_results.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/change_list_results.html`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     {% for item in result_hidden_fields %}{{ item }}{% endfor %}
 </div>
 {% endif %}
 {% if results %}
 
 <div class="row">
     <div class="col-sm-12">
-        <table id="example2" class="table table-bordered table-hover dataTable" role="grid" aria-describedby="example2_info">
+        <table id="result_list" class="table table-bordered table-hover dataTable" role="grid" aria-describedby="example2_info">
             <thead>
             <tr role="row">
                 {% for header in result_headers %}
                 <th {% if header.sortable %}
                     {% if header.sorted %}
                     {% if header.ascending %}
                     class="sorting_asc"
```

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/date_hierarchy.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/delete_confirmation.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/delete_selected_confirmation.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/edit_inline/stacked.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/edit_inline/tabular.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/filter.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/includes/fieldset.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/index.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/invalid_setup.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/invalid_setup.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/login.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/login.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-{% load i18n static adminlte_options %}<!DOCTYPE html>
+{% load i18n static adminlte_core %}<!DOCTYPE html>
 {% get_current_language as LANGUAGE_CODE %}{% get_current_language_bidi as LANGUAGE_BIDI %}
+{% get_adminlte_config_class as adminlte %}
 <html lang="{{ LANGUAGE_CODE|default:"en-us" }}" {% if LANGUAGE_BIDI %}dir="rtl"{% endif %}>
 <head>
     <!-- Current language: {{ LANGUAGE_CODE }} -->
     <meta charset="utf-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <title>
-        {% get_adminlte_option 'site_title' as adminlte_site_title %}
-        {% if adminlte_site_title.valid %}
-            {{ adminlte_site_title.site_title }}
-        {% else %}
-            {{ site_title|default:_('Django site admin') }}
-        {% endif %}
-        | {% trans "Log in" %}
+        {{ site_title|default:_('Django site admin') }} | {% trans "Log in" %}
     </title>
     <!-- Tell the browser to be responsive to screen width -->
     <meta content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no" name="viewport">
     <!-- Bootstrap -->
     <link rel="stylesheet" href={% static "admin/components/bootstrap/dist/css/bootstrap.min.css" %}>
     <!-- Font Awesome -->
     <link rel="stylesheet" href={% static "admin/components/font-awesome/css/font-awesome.min.css" %}>
@@ -37,31 +32,23 @@
     <link rel="stylesheet" href={% static "admin/dist/css/fontgoogle.css" %}>
 </head>
 <body class="hold-transition login-page">
 
 <div class="login-box">
     <div class="login-logo">
         <a href="/">
-            <b>
-                {% get_adminlte_option 'site_header' as adminlte_site_header  %}
-                {% if adminlte_site_header.valid %}
-                    {{ adminlte_site_header.site_header }}
-                {% else %}
-                    {{ site_header }}
-                {% endif %}
-            </b>
+            <b>{{ site_header }}</b>
         </a>
     </div>
 
     <!-- /.login-logo -->
     <div class="login-box-body">
         <p class="login-box-msg">
-            {% get_adminlte_option 'welcome_sign' as adminlte_welcome_sign  %}
-            {% if adminlte_welcome_sign.valid %}
-                {{ adminlte_welcome_sign.welcome_sign }}
+            {% if adminlte.welcome_sign %}
+                {{ adminlte.welcome_sign }}
             {% else %}
                 {% trans 'Login and Enjoy' %}
             {% endif %}
         </p>
         <form action="{{ app_path }}" method="post">
             {% csrf_token %}
             {% if form.errors %}
```

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/object_history.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/pagination.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/search_form.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/admin/submit_line.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/adminlte/form.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/adminlte/form.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/registration/logged_out.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/registration/logged_out.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-{% load i18n static adminlte_options %}<!DOCTYPE html>
+{% load i18n static adminlte_core %}<!DOCTYPE html>
 {% get_current_language as LANGUAGE_CODE %}{% get_current_language_bidi as LANGUAGE_BIDI %}
+{% get_adminlte_config_class as adminlte %}
 <html lang="{{ LANGUAGE_CODE|default:"en-us" }}" {% if LANGUAGE_BIDI %}dir="rtl"{% endif %}>
 <head>
     <!-- Current language: {{ LANGUAGE_CODE }} -->
     <meta charset="utf-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <title>
-        {% get_adminlte_option 'site_title' as adminlte_site_title %}
-        {% if adminlte_site_title.valid %}
-        {{ adminlte_site_title.site_title }}
-        {% else %}
-        {{ site_title|default:_('Django site admin') }}
-        {% endif %}
-        | {% trans 'Log in again' %}
+        {{ site_title|default:_('Django site admin') }} | {% trans 'Log in again' %}
     </title>
     <!-- Tell the browser to be responsive to screen width -->
     <meta content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no" name="viewport">
     <!-- Bootstrap -->
     <link rel="stylesheet" href={% static "admin/components/bootstrap/dist/css/bootstrap.min.css" %}>
     <!-- Font Awesome -->
     <link rel="stylesheet" href={% static "admin/components/font-awesome/css/font-awesome.min.css" %}>
@@ -35,31 +30,23 @@
     <link rel="stylesheet" href={% static "admin/dist/css/fontgoogle.css" %}>
 </head>
 <body class="hold-transition login-page">
 
 <div class="login-box">
     <div class="login-logo">
         <a href="/">
-            <b>
-                {% get_adminlte_option 'site_header' as adminlte_site_header  %}
-                {% if adminlte_site_header.valid %}
-                {{ adminlte_site_header.site_header }}
-                {% else %}
-                {{ site_header }}
-                {% endif %}
-            </b>
+            <b>{{ site_header }}</b>
         </a>
     </div>
 
     <!-- /.login-logo -->
     <div class="login-box-body">
         <p class="login-box-msg">
-            {% get_adminlte_option 'welcome_sign' as adminlte_welcome_sign  %}
-            {% if adminlte_welcome_sign.valid %}
-            {{ adminlte_welcome_sign.welcome_sign }}
+            {% if adminlte.welcome_sign %}
+            {{ adminlte.welcome_sign }}
             {% else %}
             {% trans 'Login and Enjoy' %}
             {% endif %}
         </p>
         <p class="text-center">{% trans "Thanks for spending some quality time with the Web site today." %}</p>
 
         <p class="text-center"><a class="btn btn-primary" href="{% url 'admin:index' %}">{% trans 'Log in again' %}</a></p>
```

#### html2text {}

```diff
@@ -1,21 +1,18 @@
-{% load i18n static adminlte_options %}
+{% load i18n static adminlte_core %}
  {% get_current_language as LANGUAGE_CODE %}{% get_current_language_bidi as
-LANGUAGE_BIDI %}
+LANGUAGE_BIDI %} {% get_adminlte_config_class as adminlte %}
  }}" {% if LANGUAGE_BIDI %}dir="rtl"{% endif %}>
 
 
 
 
 admin/components/bootstrap/dist/css/bootstrap.min.css" %}>
 admin/components/font-awesome/css/font-awesome.min.css" %}>
 admin/components/Ionicons/css/ionicons.min.css" %}>
 admin/dist/css/AdminLTE.min.css" %}>
 admin/dist/css/fontgoogle.css" %}>
-{%_get_adminlte_option_'site_header'_as_adminlte_site_header_%}_{%_if
-adminlte_site_header.valid_%}_{{_adminlte_site_header.site_header_}}_{%_else_%}
-{{_site_header_}}_{%_endif_%}
-{% get_adminlte_option 'welcome_sign' as adminlte_welcome_sign %} {% if
-adminlte_welcome_sign.valid %} {{ adminlte_welcome_sign.welcome_sign }} {% else
-%} {% trans 'Login and Enjoy' %} {% endif %}
+{{_site_header_}}
+{% if adminlte.welcome_sign %} {{ adminlte.welcome_sign }} {% else %} {% trans
+'Login and Enjoy' %} {% endif %}
 {% trans "Thanks for spending some quality time with the Web site today." %}
 {%_trans_'Log_in_again'_%}
```

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/registration/password_change_done.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/templates/registration/password_change_form.html` & `django-adminlte-ui-2.0.0/adminlteui/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/adminlteui/widgets.py` & `django-adminlte-ui-2.0.0/adminlteui/widgets.py`

 * *Files identical despite different names*

### Comparing `django-adminlte-ui-1.7.2/django_adminlte_ui.egg-info/SOURCES.txt` & `django-adminlte-ui-2.0.0/django_adminlte_ui.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,24 @@
 MANIFEST.in
 README.md
 README.rst
 setup.py
 adminlteui/__init__.py
 adminlteui/admin.py
 adminlteui/apps.py
+adminlteui/core.py
 adminlteui/models.py
 adminlteui/tests.py
 adminlteui/views.py
 adminlteui/widgets.py
 adminlteui/__pycache__/__init__.cpython-39.pyc
 adminlteui/locale/zh-Hans/LC_MESSAGES/django.mo
 adminlteui/locale/zh-Hans/LC_MESSAGES/django.po
 adminlteui/locale/zh/LC_MESSAGES/django.mo
 adminlteui/locale/zh/LC_MESSAGES/django.po
-adminlteui/migrations/0001_initial.py
-adminlteui/migrations/0002_options_valid.py
-adminlteui/migrations/0003_menu.py
-adminlteui/migrations/0004_auto_20190708_1832.py
-adminlteui/migrations/0005_menu_priority_level.py
 adminlteui/migrations/__init__.py
 adminlteui/static/admin/components/Ionicons/css/ionicons.css
 adminlteui/static/admin/components/Ionicons/css/ionicons.min.css
 adminlteui/static/admin/components/Ionicons/fonts/ionicons.eot
 adminlteui/static/admin/components/Ionicons/fonts/ionicons.svg
 adminlteui/static/admin/components/Ionicons/fonts/ionicons.ttf
 adminlteui/static/admin/components/Ionicons/fonts/ionicons.woff
@@ -469,32 +465,27 @@
 adminlteui/templates/admin/index.html
 adminlteui/templates/admin/invalid_setup.html
 adminlteui/templates/admin/login.html
 adminlteui/templates/admin/object_history.html
 adminlteui/templates/admin/pagination.html
 adminlteui/templates/admin/search_form.html
 adminlteui/templates/admin/submit_line.html
-adminlteui/templates/admin/tree_change_list_results.html
 adminlteui/templates/admin/auth/user/add_form.html
 adminlteui/templates/admin/auth/user/change_password.html
 adminlteui/templates/admin/edit_inline/stacked.html
 adminlteui/templates/admin/edit_inline/tabular.html
 adminlteui/templates/admin/includes/fieldset.html
 adminlteui/templates/admin/includes/object_delete_summary.html
 adminlteui/templates/adminlte/form.html
-adminlteui/templates/adminlte/general_option.html
-adminlteui/templates/adminlte/menu_change_form.html
-adminlteui/templates/adminlte/menu_change_list.html
 adminlteui/templates/adminlte/widgets/select.html
 adminlteui/templates/registration/logged_out.html
 adminlteui/templates/registration/password_change_done.html
 adminlteui/templates/registration/password_change_form.html
 adminlteui/templatetags/__init__.py
+adminlteui/templatetags/adminlte_core.py
 adminlteui/templatetags/adminlte_list.py
 adminlteui/templatetags/adminlte_menu.py
-adminlteui/templatetags/adminlte_options.py
 django_adminlte_ui.egg-info/PKG-INFO
 django_adminlte_ui.egg-info/SOURCES.txt
 django_adminlte_ui.egg-info/dependency_links.txt
 django_adminlte_ui.egg-info/not-zip-safe
-django_adminlte_ui.egg-info/requires.txt
 django_adminlte_ui.egg-info/top_level.txt
```

### Comparing `django-adminlte-ui-1.7.2/setup.py` & `django-adminlte-ui-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,11 +15,9 @@
     maintainer='wuyue',
     maintainer_email='wuyue92tree@163.com',
     license='MIT',
     packages=find_packages(exclude=('tests', 'tests.*')),
     include_package_data=True,
     zip_safe=False,
     entry_points={},
-    install_requires=[
-        'django-treebeard>=4.5.1'
-    ],
+    install_requires=[],
 )
```

