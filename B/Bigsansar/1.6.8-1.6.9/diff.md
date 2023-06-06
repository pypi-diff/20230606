# Comparing `tmp/Bigsansar-1.6.8.tar.gz` & `tmp/Bigsansar-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-1.6.8.tar", last modified: Mon Jun  5 06:56:29 2023, max compression
+gzip compressed data, was "Bigsansar-1.6.9.tar", last modified: Tue Jun  6 05:41:58 2023, max compression
```

## Comparing `Bigsansar-1.6.8.tar` & `Bigsansar-1.6.9.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.390554 Bigsansar-1.6.8/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.290553 Bigsansar-1.6.8/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4552 2023-06-05 06:56:29.000000 Bigsansar-1.6.8/Bigsansar.egg-info/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4913 2023-06-05 06:56:29.000000 Bigsansar-1.6.8/Bigsansar.egg-info/SOURCES.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-06-05 06:56:29.000000 Bigsansar-1.6.8/Bigsansar.egg-info/dependency_links.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-06-05 06:56:29.000000 Bigsansar-1.6.8/Bigsansar.egg-info/entry_points.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       98 2023-06-05 06:56:29.000000 Bigsansar-1.6.8/Bigsansar.egg-info/requires.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-06-05 06:56:29.000000 Bigsansar-1.6.8/Bigsansar.egg-info/top_level.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-29 06:46:12.000000 Bigsansar-1.6.8/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4552 2023-06-05 06:56:29.380554 Bigsansar-1.6.8/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3982 2023-06-05 06:46:51.000000 Bigsansar-1.6.8/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.310553 Bigsansar-1.6.8/bigsansar/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.310553 Bigsansar-1.6.8/bigsansar/contrib/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.310553 Bigsansar-1.6.8/bigsansar/contrib/account/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/account/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/account/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/account/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.310553 Bigsansar-1.6.8/bigsansar/contrib/account/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/account/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/account/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/account/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.310553 Bigsansar-1.6.8/bigsansar/contrib/account/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/account/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/account/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/account/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.320553 Bigsansar-1.6.8/bigsansar/contrib/advance/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.6.8/bigsansar/contrib/advance/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      291 2023-05-13 03:12:35.000000 Bigsansar-1.6.8/bigsansar/contrib/advance/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      202 2023-05-08 12:23:18.000000 Bigsansar-1.6.8/bigsansar/contrib/advance/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.320553 Bigsansar-1.6.8/bigsansar/contrib/advance/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1000 2023-05-08 12:29:40.000000 Bigsansar-1.6.8/bigsansar/contrib/advance/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-05-13 02:56:41.000000 Bigsansar-1.6.8/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1050 2023-05-13 03:08:43.000000 Bigsansar-1.6.8/bigsansar/contrib/advance/migrations/0003_javascript.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      386 2023-05-13 03:14:07.000000 Bigsansar-1.6.8/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.6.8/bigsansar/contrib/advance/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2023-05-13 04:58:52.000000 Bigsansar-1.6.8/bigsansar/contrib/advance/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-05-08 12:18:38.000000 Bigsansar-1.6.8/bigsansar/contrib/advance/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-05-08 12:18:38.000000 Bigsansar-1.6.8/bigsansar/contrib/advance/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.320553 Bigsansar-1.6.8/bigsansar/contrib/blogs/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/blogs/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      616 2023-06-05 06:41:08.000000 Bigsansar-1.6.8/bigsansar/contrib/blogs/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/blogs/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      261 2023-06-05 06:44:01.000000 Bigsansar-1.6.8/bigsansar/contrib/blogs/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.340553 Bigsansar-1.6.8/bigsansar/contrib/blogs/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2261 2023-05-29 10:57:40.000000 Bigsansar-1.6.8/bigsansar/contrib/blogs/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-06-02 13:13:53.000000 Bigsansar-1.6.8/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 10:57:14.000000 Bigsansar-1.6.8/bigsansar/contrib/blogs/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2152 2023-06-02 13:13:06.000000 Bigsansar-1.6.8/bigsansar/contrib/blogs/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.340553 Bigsansar-1.6.8/bigsansar/contrib/blogs/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-20 12:33:35.000000 Bigsansar-1.6.8/bigsansar/contrib/blogs/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1525 2023-06-05 06:21:13.000000 Bigsansar-1.6.8/bigsansar/contrib/blogs/templatetags/blogs.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/blogs/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/blogs/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.340553 Bigsansar-1.6.8/bigsansar/contrib/sites/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/sites/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1733 2023-06-02 12:05:41.000000 Bigsansar-1.6.8/bigsansar/contrib/sites/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/sites/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3579 2023-06-03 02:16:10.000000 Bigsansar-1.6.8/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.340553 Bigsansar-1.6.8/bigsansar/contrib/sites/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1847 2023-05-02 12:46:38.000000 Bigsansar-1.6.8/bigsansar/contrib/sites/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:46:31.000000 Bigsansar-1.6.8/bigsansar/contrib/sites/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1899 2023-05-17 10:15:27.000000 Bigsansar-1.6.8/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.340553 Bigsansar-1.6.8/bigsansar/contrib/sites/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/sites/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/sites/templatetags/pages.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/sites/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/contrib/sites/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.350554 Bigsansar-1.6.8/bigsansar/core/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/core/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/core/host.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    10679 2023-05-27 06:38:55.000000 Bigsansar-1.6.8/bigsansar/core/init.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/main.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.350554 Bigsansar-1.6.8/bigsansar/management/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.350554 Bigsansar-1.6.8/bigsansar/management/commands/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/management/commands/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.6.8/bigsansar/management/commands/createuser.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.350554 Bigsansar-1.6.8/bigsansar/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.350554 Bigsansar-1.6.8/bigsansar/static/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/static/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.280553 Bigsansar-1.6.8/bigsansar/static/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.280553 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.280553 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.350554 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.350554 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1258 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1165 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.370554 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1337 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1654 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1209 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1078 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1514 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1049 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1084 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1103 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      960 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1051 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1250 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1166 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1106 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1195 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1229 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1047 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1064 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1120 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1151 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1178 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1564 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1173 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1206 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1538 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1067 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      916 2021-03-31 11:22:53.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13371 2021-03-31 14:36:18.000000 Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/static/logo.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-05 06:56:29.380554 Bigsansar-1.6.8/bigsansar/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/templates/404.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/templates/acc_active_email.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1521 2023-05-05 10:08:59.000000 Bigsansar-1.6.8/bigsansar/templates/base.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1931 2023-06-05 06:55:58.000000 Bigsansar-1.6.8/bigsansar/templates/blog_preview.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/templates/default.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/templates/defaultpage.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/templates/parking.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-05-20 05:28:14.000000 Bigsansar-1.6.8/bigsansar/templates/sitemap.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.8/bigsansar/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1155 2023-05-20 14:08:47.000000 Bigsansar-1.6.8/bigsansar/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4479 2023-06-05 06:54:06.000000 Bigsansar-1.6.8/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-06-05 06:56:29.390554 Bigsansar-1.6.8/setup.cfg
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1712 2023-06-05 06:56:08.000000 Bigsansar-1.6.8/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:58.054339 Bigsansar-1.6.9/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.964339 Bigsansar-1.6.9/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4552 2023-06-06 05:41:57.000000 Bigsansar-1.6.9/Bigsansar.egg-info/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4913 2023-06-06 05:41:57.000000 Bigsansar-1.6.9/Bigsansar.egg-info/SOURCES.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-06-06 05:41:57.000000 Bigsansar-1.6.9/Bigsansar.egg-info/dependency_links.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-06-06 05:41:57.000000 Bigsansar-1.6.9/Bigsansar.egg-info/entry_points.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       98 2023-06-06 05:41:57.000000 Bigsansar-1.6.9/Bigsansar.egg-info/requires.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-06-06 05:41:57.000000 Bigsansar-1.6.9/Bigsansar.egg-info/top_level.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-29 06:46:12.000000 Bigsansar-1.6.9/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4552 2023-06-06 05:41:58.044339 Bigsansar-1.6.9/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3982 2023-06-05 06:46:51.000000 Bigsansar-1.6.9/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.964339 Bigsansar-1.6.9/bigsansar/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.964339 Bigsansar-1.6.9/bigsansar/contrib/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.974339 Bigsansar-1.6.9/bigsansar/contrib/account/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/account/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/account/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/account/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.974339 Bigsansar-1.6.9/bigsansar/contrib/account/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/account/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/account/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/account/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.974339 Bigsansar-1.6.9/bigsansar/contrib/account/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/account/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/account/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/account/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.984339 Bigsansar-1.6.9/bigsansar/contrib/advance/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.6.9/bigsansar/contrib/advance/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      291 2023-05-13 03:12:35.000000 Bigsansar-1.6.9/bigsansar/contrib/advance/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      202 2023-05-08 12:23:18.000000 Bigsansar-1.6.9/bigsansar/contrib/advance/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.984339 Bigsansar-1.6.9/bigsansar/contrib/advance/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1000 2023-05-08 12:29:40.000000 Bigsansar-1.6.9/bigsansar/contrib/advance/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-05-13 02:56:41.000000 Bigsansar-1.6.9/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1050 2023-05-13 03:08:43.000000 Bigsansar-1.6.9/bigsansar/contrib/advance/migrations/0003_javascript.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      386 2023-05-13 03:14:07.000000 Bigsansar-1.6.9/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.6.9/bigsansar/contrib/advance/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2023-05-13 04:58:52.000000 Bigsansar-1.6.9/bigsansar/contrib/advance/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-05-08 12:18:38.000000 Bigsansar-1.6.9/bigsansar/contrib/advance/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-05-08 12:18:38.000000 Bigsansar-1.6.9/bigsansar/contrib/advance/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.984339 Bigsansar-1.6.9/bigsansar/contrib/blogs/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/blogs/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      807 2023-06-06 05:38:32.000000 Bigsansar-1.6.9/bigsansar/contrib/blogs/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/blogs/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      261 2023-06-05 06:44:01.000000 Bigsansar-1.6.9/bigsansar/contrib/blogs/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.994339 Bigsansar-1.6.9/bigsansar/contrib/blogs/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2261 2023-05-29 10:57:40.000000 Bigsansar-1.6.9/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-06-02 13:13:53.000000 Bigsansar-1.6.9/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 10:57:14.000000 Bigsansar-1.6.9/bigsansar/contrib/blogs/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2152 2023-06-02 13:13:06.000000 Bigsansar-1.6.9/bigsansar/contrib/blogs/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.994339 Bigsansar-1.6.9/bigsansar/contrib/blogs/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-20 12:33:35.000000 Bigsansar-1.6.9/bigsansar/contrib/blogs/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1525 2023-06-05 06:21:13.000000 Bigsansar-1.6.9/bigsansar/contrib/blogs/templatetags/blogs.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/blogs/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.994339 Bigsansar-1.6.9/bigsansar/contrib/sites/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/sites/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2316 2023-06-06 05:41:11.000000 Bigsansar-1.6.9/bigsansar/contrib/sites/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/sites/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3579 2023-06-03 02:16:10.000000 Bigsansar-1.6.9/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.994339 Bigsansar-1.6.9/bigsansar/contrib/sites/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1847 2023-05-02 12:46:38.000000 Bigsansar-1.6.9/bigsansar/contrib/sites/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:46:31.000000 Bigsansar-1.6.9/bigsansar/contrib/sites/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1899 2023-05-17 10:15:27.000000 Bigsansar-1.6.9/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.994339 Bigsansar-1.6.9/bigsansar/contrib/sites/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/sites/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/sites/templatetags/pages.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/sites/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/contrib/sites/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.994339 Bigsansar-1.6.9/bigsansar/core/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/core/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/core/host.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    10679 2023-05-27 06:38:55.000000 Bigsansar-1.6.9/bigsansar/core/init.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/main.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.994339 Bigsansar-1.6.9/bigsansar/management/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.994339 Bigsansar-1.6.9/bigsansar/management/commands/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/management/commands/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.6.9/bigsansar/management/commands/createuser.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.994339 Bigsansar-1.6.9/bigsansar/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:58.004339 Bigsansar-1.6.9/bigsansar/static/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/static/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.964339 Bigsansar-1.6.9/bigsansar/static/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.964339 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:57.964339 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:58.004339 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:58.014339 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1258 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1165 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:58.044339 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1337 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1654 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1209 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1078 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1514 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1049 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1084 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1103 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      960 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1051 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1250 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1166 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1106 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1195 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1229 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1047 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1064 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1120 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1151 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1178 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1564 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1173 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1206 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1538 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1067 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      916 2021-03-31 11:22:53.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13371 2021-03-31 14:36:18.000000 Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/static/logo.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-06 05:41:58.044339 Bigsansar-1.6.9/bigsansar/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/templates/404.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/templates/acc_active_email.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1521 2023-05-05 10:08:59.000000 Bigsansar-1.6.9/bigsansar/templates/base.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1931 2023-06-05 06:55:58.000000 Bigsansar-1.6.9/bigsansar/templates/blog_preview.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/templates/default.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/templates/defaultpage.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/templates/parking.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-06-06 04:42:17.000000 Bigsansar-1.6.9/bigsansar/templates/sitemap.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.9/bigsansar/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1155 2023-05-20 14:08:47.000000 Bigsansar-1.6.9/bigsansar/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4479 2023-06-05 06:54:06.000000 Bigsansar-1.6.9/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-06-06 05:41:58.054339 Bigsansar-1.6.9/setup.cfg
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1712 2023-06-06 05:41:35.000000 Bigsansar-1.6.9/setup.py
```

### Comparing `Bigsansar-1.6.8/Bigsansar.egg-info/PKG-INFO` & `Bigsansar-1.6.9/Bigsansar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.6.8
+Version: 1.6.9
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 1.6.8 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 1.6.9 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 bigsansar.com Author: Bikash Pokhrel Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN Project-URL: Bug Tracker, https://github.com/pokhrelb9/
 bigsansar/issues Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django
 flatpages Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `Bigsansar-1.6.8/Bigsansar.egg-info/SOURCES.txt` & `Bigsansar-1.6.9/Bigsansar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/LICENSE` & `Bigsansar-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/PKG-INFO` & `Bigsansar-1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.6.8
+Version: 1.6.9
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 1.6.8 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 1.6.9 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 bigsansar.com Author: Bikash Pokhrel Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN Project-URL: Bug Tracker, https://github.com/pokhrelb9/
 bigsansar/issues Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django
 flatpages Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `Bigsansar-1.6.8/README.md` & `Bigsansar-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/contrib/account/forms.py` & `Bigsansar-1.6.9/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/contrib/account/migrations/0001_initial.py` & `Bigsansar-1.6.9/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/contrib/account/models.py` & `Bigsansar-1.6.9/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/contrib/advance/migrations/0001_initial.py` & `Bigsansar-1.6.9/bigsansar/contrib/advance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/contrib/advance/migrations/0003_javascript.py` & `Bigsansar-1.6.9/bigsansar/contrib/advance/migrations/0003_javascript.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/contrib/advance/models.py` & `Bigsansar-1.6.9/bigsansar/contrib/advance/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/contrib/blogs/migrations/0001_initial.py` & `Bigsansar-1.6.9/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/contrib/blogs/models.py` & `Bigsansar-1.6.9/bigsansar/contrib/blogs/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/contrib/blogs/templatetags/blogs.py` & `Bigsansar-1.6.9/bigsansar/contrib/blogs/templatetags/blogs.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/contrib/sites/admin.py` & `Bigsansar-1.6.9/bigsansar/contrib/sites/admin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.contrib import admin
 from django.contrib.admin import SimpleListFilter
 from django.utils.translation import gettext_lazy as _
 from bigsansar.contrib.sites.forms import create_domainform, customaddpageform, custompageform
 from bigsansar.contrib.sites.models import domains, pages
+from django.contrib.auth.models import User
 
 
 # Register your models here.
 
 
 class domain_filter(SimpleListFilter):
     title = _('Domains')  # a label for our filter
@@ -23,29 +24,42 @@
         if self.value():
             return queryset.filter(domain=self.value())
 
 
 class domainadmin(admin.ModelAdmin):
     form = create_domainform
     list_display = ['domain', 'publish_date', 'visitor']
+    search_fields = ['domain']
+
+    def get_queryset(self, request):
+        qs = super().get_queryset(request)
+        if request.user.is_superuser:
+            return qs
+        return qs.filter(user=request.user)
+    
+    def formfield_for_foreignkey(self, db_field, request, **kwargs):
+        if db_field.name == "user":
+            kwargs["queryset"] = User.objects.filter(username=request.user.username)
+        return super().formfield_for_foreignkey(db_field, request, **kwargs)
 
 
 class pageadmin(admin.ModelAdmin):
     add_form = customaddpageform
     form = custompageform
     prepopulated_fields = {"slug": ("title",)}
     list_display = ['slug', 'domain', 'publish_date', 'visitor']
     list_filter = (domain_filter,)
+    search_fields = ['slug']
 
     def get_form(self, request, obj=None, **kwargs):
         """
         Use special form during foo creation
         """
         defaults = {}
         if obj is None:
             defaults['form'] = self.add_form
         defaults.update(kwargs)
         return super().get_form(request, obj, **defaults)
-
+        
 
 admin.site.register(domains, domainadmin)
 admin.site.register(pages, pageadmin)
```

### Comparing `Bigsansar-1.6.8/bigsansar/contrib/sites/forms.py` & `Bigsansar-1.6.9/bigsansar/contrib/sites/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/contrib/sites/migrations/0001_initial.py` & `Bigsansar-1.6.9/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/contrib/sites/models.py` & `Bigsansar-1.6.9/bigsansar/contrib/sites/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/core/__init__.py` & `Bigsansar-1.6.9/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/core/init.py` & `Bigsansar-1.6.9/bigsansar/core/init.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/management/commands/createuser.py` & `Bigsansar-1.6.9/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js` & `Bigsansar-1.6.9/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/logo.png` & `Bigsansar-1.6.9/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/static/style.css` & `Bigsansar-1.6.9/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/templates/404.html` & `Bigsansar-1.6.9/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/templates/base.html` & `Bigsansar-1.6.9/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/templates/blog_preview.html` & `Bigsansar-1.6.9/bigsansar/templates/blog_preview.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/templates/default.html` & `Bigsansar-1.6.9/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/templates/defaultpage.html` & `Bigsansar-1.6.9/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/templates/parking.html` & `Bigsansar-1.6.9/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/urls.py` & `Bigsansar-1.6.9/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/bigsansar/views.py` & `Bigsansar-1.6.9/bigsansar/views.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.8/setup.py` & `Bigsansar-1.6.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="1.6.8",
+    version="1.6.9",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bigsansar.com",
     project_urls={
```

