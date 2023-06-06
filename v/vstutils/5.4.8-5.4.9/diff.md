# Comparing `tmp/vstutils-5.4.8.tar.gz` & `tmp/vstutils-5.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstutils-5.4.8.tar", last modified: Thu May 25 15:50:43 2023, max compression
+gzip compressed data, was "vstutils-5.4.9.tar", last modified: Fri May 26 06:06:53 2023, max compression
```

## Comparing `vstutils-5.4.8.tar` & `vstutils-5.4.9.tar`

### file list

```diff
@@ -1,252 +1,253 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.759326 vstutils-5.4.8/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.4.8/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.4.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.4.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4459 2023-05-25 15:50:43.759326 vstutils-5.4.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2393 2022-12-19 05:43:06.000000 vstutils-5.4.8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-25 10:44:35.000000 vstutils-5.4.8/requirements-doc.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.4.8/requirements-git.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.4.8/requirements-ldap.txt
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-13 04:11:10.000000 vstutils-5.4.8/requirements-prod.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-03-18 02:33:32.000000 vstutils-5.4.8/requirements-rpc.txt
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-03-29 01:47:58.000000 vstutils-5.4.8/requirements-stubs.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-13 04:11:10.000000 vstutils-5.4.8/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-05-13 04:11:10.000000 vstutils-5.4.8/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-05-25 15:50:43.759326 vstutils-5.4.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    16893 2023-04-13 03:48:29.000000 vstutils-5.4.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.715326 vstutils-5.4.8/vstutils/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.723326 vstutils-5.4.8/vstutils/api/
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15370 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/api/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/api/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    13063 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/api/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    28141 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)    24054 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/api/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/api/decorators.pyi
--rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/doc_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    18802 2023-02-07 05:18:57.000000 vstutils-5.4.8/vstutils/api/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)    51728 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/api/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    11754 2023-05-13 04:11:10.000000 vstutils-5.4.8/vstutils/api/filter_backends.py
--rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2531 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/health.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.723326 vstutils-5.4.8/vstutils/api/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/migrations/0002_two_factor.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/migrations/0003_tfa_indexes.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/migrations/0004_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/migrations/0005_db_translations.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/migrations/0006_fix_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4591 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/api/models.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/renderers.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/responses.py
--rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/responses.pyi
--rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/api/routers.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/api/routers.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.723326 vstutils-5.4.8/vstutils/api/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/api/schema/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/api/schema/info.py
--rw-rw-rw-   0 root         (0) root         (0)    26465 2023-03-17 01:28:59.000000 vstutils-5.4.8/vstutils/api/schema/inspectors.py
--rw-rw-rw-   0 root         (0) root         (0)     9648 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/api/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/schema/views.py
--rw-rw-rw-   0 root         (0) root         (0)     7340 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/throttling.py
--rw-rw-rw-   0 root         (0) root         (0)    10784 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/api/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     5660 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/views.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1363 2023-02-20 07:13:28.000000 vstutils-5.4.8/vstutils/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-02-13 06:24:20.000000 vstutils-5.4.8/vstutils/asgi_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     4232 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/auth.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/celery_beat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.703326 vstutils-5.4.8/vstutils/doc_themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.727326 vstutils-5.4.8/vstutils/doc_themes/vst-sphinx-theme/
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/doc_themes/vst-sphinx-theme/layout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.727326 vstutils-5.4.8/vstutils/doc_themes/vst-sphinx-theme/static/
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-25 15:50:43.763326 vstutils-5.4.8/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/doc_themes/vst-sphinx-theme/theme.conf
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/environment.pyi
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.727326 vstutils-5.4.8/vstutils/gui/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/gui/context.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/gui/pwa_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/gui/views.py
--rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/ldap_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.727326 vstutils-5.4.8/vstutils/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.727326 vstutils-5.4.8/vstutils/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7832 2023-03-16 06:05:23.000000 vstutils-5.4.8/vstutils/management/commands/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/management/commands/celery_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/management/commands/dockermigrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/management/commands/dockerrun.py
--rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/management/commands/newproject.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/management/commands/run_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/management/commands/runrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.4.8/vstutils/management/commands/runserver.py
--rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/management/commands/web.py
--rw-rw-rw-   0 root         (0) root         (0)    10646 2023-02-13 06:24:20.000000 vstutils-5.4.8/vstutils/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.731326 vstutils-5.4.8/vstutils/models/
--rw-rw-rw-   0 root         (0) root         (0)    10704 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25308 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4130 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/models/cent_notify.py
--rw-rw-rw-   0 root         (0) root         (0)    11620 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/models/custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/models/custom_model.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/models/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7971 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/models/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/models/model.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/models/queryset.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/settings.ini
--rw-rw-rw-   0 root         (0) root         (0)    54947 2023-04-13 03:48:29.000000 vstutils-5.4.8/vstutils/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.703326 vstutils-5.4.8/vstutils/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.743326 vstutils-5.4.8/vstutils/static/bundle/
--rw-r--r--   0 root         (0) root         (0)      155 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/157.chunk.js
--rw-r--r--   0 root         (0) root         (0)   126295 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/281.chunk.js
--rw-r--r--   0 root         (0) root         (0)      171 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/281.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1553 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/296.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/296.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   136100 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/345.chunk.js
--rw-r--r--   0 root         (0) root         (0)    15726 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/368.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1066719 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/421.js
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/421.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      321 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/463.chunk.js
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/564.chunk.js
--rw-r--r--   0 root         (0) root         (0)    38336 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/618.js
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/618.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2235 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/683.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/683.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    71086 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/686.js
--rw-r--r--   0 root         (0) root         (0)   536206 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/742.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/742.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    89997 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/755.js
--rw-r--r--   0 root         (0) root         (0)      476 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/755.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   355788 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/826.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/826.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   177828 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/844.js
--rw-r--r--   0 root         (0) root         (0)  1798980 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/959.js
--rw-r--r--   0 root         (0) root         (0)     2191 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/959.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    77026 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/app_loader.js
--rw-r--r--   0 root         (0) root         (0)   303656 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/base.js
--rw-r--r--   0 root         (0) root         (0)    16276 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
--rw-r--r--   0 root         (0) root         (0)   101648 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
--rw-r--r--   0 root         (0) root         (0)      748 2023-05-25 15:50:43.000000 vstutils-5.4.8/vstutils/static/bundle/output.json
--rw-r--r--   0 root         (0) root         (0)     3597 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/spa.js
--rw-r--r--   0 root         (0) root         (0)   432625 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/vstutils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.743326 vstutils-5.4.8/vstutils/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/static/img/anonymous.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.743326 vstutils-5.4.8/vstutils/static/img/logo/
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/static/img/logo/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/static_files.py
--rw-rw-rw-   0 root         (0) root         (0)     5181 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.743326 vstutils-5.4.8/vstutils/templates/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.4.8/vstutils/templates/400.html
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.4.8/vstutils/templates/403.html
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.4.8/vstutils/templates/404.html
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.4.8/vstutils/templates/500.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.743326 vstutils-5.4.8/vstutils/templates/auth/
--rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/auth/base.html
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/auth/language_selector.html
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/auth/login.html
--rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/auth/tfa.html
--rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.4.8/vstutils/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.4.8/vstutils/templates/base_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.747326 vstutils-5.4.8/vstutils/templates/configs/
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/configs/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.747326 vstutils-5.4.8/vstutils/templates/drf-yasg/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/drf-yasg/swagger-ui.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.4.8/vstutils/templates/go_back_button.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.747326 vstutils-5.4.8/vstutils/templates/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/gui/base.html
--rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/gui/gui.html
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/gui/manifest.json
--rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/gui/offline.html
--rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/gui/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.751326 vstutils-5.4.8/vstutils/templates/newproject/
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/.coveragerc.template
--rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/.gitignore.template
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/.pep8.template
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/MANIFEST.in.template
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/README.rst.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.751326 vstutils-5.4.8/vstutils/templates/newproject/frontend_src/
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/frontend_src/.babelrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/frontend_src/.editorconfig.template
--rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/frontend_src/.prettierrc.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.751326 vstutils-5.4.8/vstutils/templates/newproject/frontend_src/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/frontend_src/app/index.js.template
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/package.json.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.751326 vstutils-5.4.8/vstutils/templates/newproject/project_name/
--rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/project_name/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/project_name/__main__.py.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.751326 vstutils-5.4.8/vstutils/templates/newproject/project_name/models/
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/project_name/models/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/project_name/settings.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/project_name/settings.py.template
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/project_name/web.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/project_name/wsgi.py.template
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/requirements-test.txt.template
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/requirements.txt.template
--rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/setup.cfg.template
--rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.4.8/vstutils/templates/newproject/setup.py.template
--rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/test.py.template
--rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/tox.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/tox_build.ini.template
--rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/webpack.config.js.default.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.755326 vstutils-5.4.8/vstutils/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/registration/base.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/registration/base_agreements.html
--rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.4.8/vstutils/templates/registration/confirm_email.html
--rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/registration/user_registration.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.755326 vstutils-5.4.8/vstutils/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/rest_framework/admin.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/rest_framework/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.755326 vstutils-5.4.8/vstutils/templates/vst_inclusion_tags/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.755326 vstutils-5.4.8/vstutils/templates/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/widgets/agreement_widget.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.755326 vstutils-5.4.8/vstutils/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/templatetags/request_static.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templatetags/translation.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templatetags/vst_gravatar.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/templatetags/vst_html_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templatetags/vstconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)    17731 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.755326 vstutils-5.4.8/vstutils/translations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/translations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16196 2023-03-15 02:43:46.000000 vstutils-5.4.8/vstutils/translations/cn.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/translations/en.py
--rw-rw-rw-   0 root         (0) root         (0)    23941 2023-03-15 02:43:46.000000 vstutils-5.4.8/vstutils/translations/ru.py
--rw-rw-rw-   0 root         (0) root         (0)    18983 2023-03-15 02:43:46.000000 vstutils-5.4.8/vstutils/translations/vi.py
--rw-rw-rw-   0 root         (0) root         (0)     2721 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    44730 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/web.ini
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.719326 vstutils-5.4.8/vstutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4459 2023-05-25 15:50:43.000000 vstutils-5.4.8/vstutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7644 2023-05-25 15:50:43.000000 vstutils-5.4.8/vstutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-25 15:50:43.000000 vstutils-5.4.8/vstutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-05-25 15:50:43.000000 vstutils-5.4.8/vstutils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1941 2023-05-25 15:50:43.000000 vstutils-5.4.8/vstutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-25 15:50:43.000000 vstutils-5.4.8/vstutils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.424696 vstutils-5.4.9/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.4.9/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.4.9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.4.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4459 2023-05-26 06:06:53.424696 vstutils-5.4.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2393 2022-12-19 05:43:06.000000 vstutils-5.4.9/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-25 10:44:35.000000 vstutils-5.4.9/requirements-doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.4.9/requirements-git.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.4.9/requirements-ldap.txt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-13 04:11:10.000000 vstutils-5.4.9/requirements-prod.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-03-18 02:33:32.000000 vstutils-5.4.9/requirements-rpc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-03-29 01:47:58.000000 vstutils-5.4.9/requirements-stubs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-13 04:11:10.000000 vstutils-5.4.9/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-05-26 04:04:11.000000 vstutils-5.4.9/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-05-26 06:06:53.424696 vstutils-5.4.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    16893 2023-04-13 03:48:29.000000 vstutils-5.4.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.384695 vstutils-5.4.9/vstutils/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-26 00:26:03.000000 vstutils-5.4.9/vstutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.392696 vstutils-5.4.9/vstutils/api/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15370 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/api/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/api/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    13063 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/api/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    28220 2023-05-26 03:10:25.000000 vstutils-5.4.9/vstutils/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    24054 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/api/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/api/decorators.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/doc_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    18802 2023-02-07 05:18:57.000000 vstutils-5.4.9/vstutils/api/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    51728 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/api/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    11754 2023-05-13 04:11:10.000000 vstutils-5.4.9/vstutils/api/filter_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2531 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/health.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.392696 vstutils-5.4.9/vstutils/api/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/migrations/0002_two_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/migrations/0003_tfa_indexes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/migrations/0004_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/migrations/0005_db_translations.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/migrations/0006_fix_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4591 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/renderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/responses.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/api/routers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/api/routers.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.396695 vstutils-5.4.9/vstutils/api/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/api/schema/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/api/schema/info.py
+-rw-rw-rw-   0 root         (0) root         (0)    26465 2023-03-17 01:28:59.000000 vstutils-5.4.9/vstutils/api/schema/inspectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     9648 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/api/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/schema/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     7340 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/throttling.py
+-rw-rw-rw-   0 root         (0) root         (0)    10784 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/api/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5660 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/api/views.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2695 2023-05-26 04:04:11.000000 vstutils-5.4.9/vstutils/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-02-13 06:24:20.000000 vstutils-5.4.9/vstutils/asgi_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4232 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/auth.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/celery_beat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.376695 vstutils-5.4.9/vstutils/doc_themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.396695 vstutils-5.4.9/vstutils/doc_themes/vst-sphinx-theme/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/doc_themes/vst-sphinx-theme/layout.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.396695 vstutils-5.4.9/vstutils/doc_themes/vst-sphinx-theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-26 06:06:53.432696 vstutils-5.4.9/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/doc_themes/vst-sphinx-theme/theme.conf
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/environment.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.396695 vstutils-5.4.9/vstutils/gui/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3467 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/gui/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/gui/pwa_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/gui/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/ldap_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.396695 vstutils-5.4.9/vstutils/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.396695 vstutils-5.4.9/vstutils/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7832 2023-03-16 06:05:23.000000 vstutils-5.4.9/vstutils/management/commands/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/management/commands/celery_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/management/commands/dockermigrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/management/commands/dockerrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/management/commands/newproject.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/management/commands/run_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/management/commands/runrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.4.9/vstutils/management/commands/runserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/management/commands/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    10646 2023-02-13 06:24:20.000000 vstutils-5.4.9/vstutils/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.400696 vstutils-5.4.9/vstutils/models/
+-rw-rw-rw-   0 root         (0) root         (0)    10704 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25308 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/models/cent_notify.py
+-rw-rw-rw-   0 root         (0) root         (0)    11620 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/models/custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2534 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/models/custom_model.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/models/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7971 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/models/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/models/queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/settings.ini
+-rw-rw-rw-   0 root         (0) root         (0)    55118 2023-05-26 04:17:32.000000 vstutils-5.4.9/vstutils/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-26 00:26:03.000000 vstutils-5.4.9/vstutils/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.376695 vstutils-5.4.9/vstutils/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.408696 vstutils-5.4.9/vstutils/static/bundle/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/157.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   126295 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/281.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      171 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/281.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/296.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/296.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   136100 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/345.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    15726 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/368.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1066719 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/421.js
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/421.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      321 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/463.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/564.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    38336 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/618.js
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/618.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/683.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/683.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    71086 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/686.js
+-rw-r--r--   0 root         (0) root         (0)   536206 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/742.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/742.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    89997 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/755.js
+-rw-r--r--   0 root         (0) root         (0)      476 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/755.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   355788 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/826.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/826.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   177828 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/844.js
+-rw-r--r--   0 root         (0) root         (0)  1798980 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/959.js
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/959.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    77026 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/app_loader.js
+-rw-r--r--   0 root         (0) root         (0)   303656 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/base.js
+-rw-r--r--   0 root         (0) root         (0)    16276 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
+-rw-r--r--   0 root         (0) root         (0)   101648 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
+-rw-r--r--   0 root         (0) root         (0)      748 2023-05-26 06:06:53.000000 vstutils-5.4.9/vstutils/static/bundle/output.json
+-rw-r--r--   0 root         (0) root         (0)     3597 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/spa.js
+-rw-r--r--   0 root         (0) root         (0)   432625 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils/static/bundle/vstutils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.408696 vstutils-5.4.9/vstutils/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/static/img/anonymous.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.412696 vstutils-5.4.9/vstutils/static/img/logo/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/static/img/logo/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/static_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     5181 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.412696 vstutils-5.4.9/vstutils/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.4.9/vstutils/templates/400.html
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.4.9/vstutils/templates/403.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.4.9/vstutils/templates/404.html
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.4.9/vstutils/templates/500.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.412696 vstutils-5.4.9/vstutils/templates/auth/
+-rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/auth/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/auth/language_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/auth/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/auth/tfa.html
+-rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.4.9/vstutils/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.4.9/vstutils/templates/base_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.412696 vstutils-5.4.9/vstutils/templates/configs/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/configs/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.412696 vstutils-5.4.9/vstutils/templates/drf-yasg/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/drf-yasg/swagger-ui.html
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.4.9/vstutils/templates/go_back_button.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.412696 vstutils-5.4.9/vstutils/templates/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/gui/base.html
+-rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/gui/gui.html
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/gui/manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/gui/offline.html
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/gui/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.416696 vstutils-5.4.9/vstutils/templates/newproject/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/.coveragerc.template
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/.gitignore.template
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/.pep8.template
+-rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/MANIFEST.in.template
+-rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/README.rst.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.416696 vstutils-5.4.9/vstutils/templates/newproject/frontend_src/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/frontend_src/.babelrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/frontend_src/.editorconfig.template
+-rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/frontend_src/.prettierrc.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.416696 vstutils-5.4.9/vstutils/templates/newproject/frontend_src/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/frontend_src/app/index.js.template
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/package.json.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.420696 vstutils-5.4.9/vstutils/templates/newproject/project_name/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/project_name/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/project_name/__main__.py.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.420696 vstutils-5.4.9/vstutils/templates/newproject/project_name/models/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/project_name/models/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/project_name/settings.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/project_name/settings.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/project_name/web.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/project_name/wsgi.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/requirements-test.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/requirements.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/setup.cfg.template
+-rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.4.9/vstutils/templates/newproject/setup.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/test.py.template
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/tox.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/tox_build.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/newproject/webpack.config.js.default.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.420696 vstutils-5.4.9/vstutils/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/registration/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/registration/base_agreements.html
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.4.9/vstutils/templates/registration/confirm_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/registration/user_registration.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.420696 vstutils-5.4.9/vstutils/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/rest_framework/admin.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/rest_framework/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.420696 vstutils-5.4.9/vstutils/templates/vst_inclusion_tags/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
+-rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.420696 vstutils-5.4.9/vstutils/templates/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templates/widgets/agreement_widget.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.420696 vstutils-5.4.9/vstutils/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/templatetags/request_static.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templatetags/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templatetags/vst_gravatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.4.9/vstutils/templatetags/vst_html_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/templatetags/vstconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)    17731 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.424696 vstutils-5.4.9/vstutils/translations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/translations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16196 2023-03-15 02:43:46.000000 vstutils-5.4.9/vstutils/translations/cn.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/translations/en.py
+-rw-rw-rw-   0 root         (0) root         (0)    23941 2023-03-15 02:43:46.000000 vstutils-5.4.9/vstutils/translations/ru.py
+-rw-rw-rw-   0 root         (0) root         (0)    18983 2023-03-15 02:43:46.000000 vstutils-5.4.9/vstutils/translations/vi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2721 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    44730 2023-05-25 10:44:35.000000 vstutils-5.4.9/vstutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-06 06:25:26.000000 vstutils-5.4.9/vstutils/web.ini
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.4.9/vstutils/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 06:06:53.388696 vstutils-5.4.9/vstutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4459 2023-05-26 06:06:53.000000 vstutils-5.4.9/vstutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7664 2023-05-26 06:06:53.000000 vstutils-5.4.9/vstutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-26 06:06:53.000000 vstutils-5.4.9/vstutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-26 06:06:53.000000 vstutils-5.4.9/vstutils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 06:05:41.000000 vstutils-5.4.9/vstutils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-05-26 06:06:53.000000 vstutils-5.4.9/vstutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-26 06:06:53.000000 vstutils-5.4.9/vstutils.egg-info/top_level.txt
```

### Comparing `vstutils-5.4.8/LICENSE` & `vstutils-5.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/MANIFEST.in` & `vstutils-5.4.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/NOTICE` & `vstutils-5.4.9/NOTICE`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/PKG-INFO` & `vstutils-5.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.4.8
+Version: 5.4.9
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.4.8/README.rst` & `vstutils-5.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/setup.cfg` & `vstutils-5.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/setup.py` & `vstutils-5.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/actions.py` & `vstutils-5.4.9/vstutils/api/actions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/admin.py` & `vstutils-5.4.9/vstutils/api/admin.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/auth.py` & `vstutils-5.4.9/vstutils/api/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/base.py` & `vstutils-5.4.9/vstutils/api/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -502,14 +502,16 @@
     def check_etag(self, request, model_class=None):
         if request.method == "GET":
             header = request.headers.get("If-None-Match", None)
             if not header:
                 return
             data = self._get_etag(model_class or self.model_class, request)
             header = str(header)
+            if header[:2] in ('W/', "w/"):
+                header = header[2:]
             if header[0] != '"':
                 header = f'"{header}"'
             if data == header:
                 raise self.NotModifiedException("")
         # TODO: Workflow with ETag on PUT/PATCH/DELETE
 
     def finalize_response(self, request: Request, response: RestResponse, *args, **kwargs) -> RestResponse:
```

### Comparing `vstutils-5.4.8/vstutils/api/decorators.py` & `vstutils-5.4.9/vstutils/api/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/decorators.pyi` & `vstutils-5.4.9/vstutils/api/decorators.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/doc_generator.py` & `vstutils-5.4.9/vstutils/api/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/endpoint.py` & `vstutils-5.4.9/vstutils/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/fields.py` & `vstutils-5.4.9/vstutils/api/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/filter_backends.py` & `vstutils-5.4.9/vstutils/api/filter_backends.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/filters.py` & `vstutils-5.4.9/vstutils/api/filters.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/health.py` & `vstutils-5.4.9/vstutils/api/health.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/meta.py` & `vstutils-5.4.9/vstutils/api/meta.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/metrics.py` & `vstutils-5.4.9/vstutils/api/metrics.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/migrations/0001_initial.py` & `vstutils-5.4.9/vstutils/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/migrations/0002_two_factor.py` & `vstutils-5.4.9/vstutils/api/migrations/0002_two_factor.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/migrations/0003_tfa_indexes.py` & `vstutils-5.4.9/vstutils/api/migrations/0003_tfa_indexes.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/migrations/0004_user_settings.py` & `vstutils-5.4.9/vstutils/api/migrations/0004_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/migrations/0005_db_translations.py` & `vstutils-5.4.9/vstutils/api/migrations/0005_db_translations.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/migrations/0006_fix_user_settings.py` & `vstutils-5.4.9/vstutils/api/migrations/0006_fix_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/models.py` & `vstutils-5.4.9/vstutils/api/models.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/pagination.py` & `vstutils-5.4.9/vstutils/api/pagination.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/parsers.py` & `vstutils-5.4.9/vstutils/api/parsers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/permissions.py` & `vstutils-5.4.9/vstutils/api/permissions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/renderers.py` & `vstutils-5.4.9/vstutils/api/renderers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/responses.py` & `vstutils-5.4.9/vstutils/api/responses.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/responses.pyi` & `vstutils-5.4.9/vstutils/api/responses.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/routers.py` & `vstutils-5.4.9/vstutils/api/routers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/routers.pyi` & `vstutils-5.4.9/vstutils/api/routers.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/schema/generators.py` & `vstutils-5.4.9/vstutils/api/schema/generators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/schema/info.py` & `vstutils-5.4.9/vstutils/api/schema/info.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/schema/inspectors.py` & `vstutils-5.4.9/vstutils/api/schema/inspectors.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/schema/schema.py` & `vstutils-5.4.9/vstutils/api/schema/schema.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/serializers.py` & `vstutils-5.4.9/vstutils/api/serializers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/throttling.py` & `vstutils-5.4.9/vstutils/api/throttling.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/validators.py` & `vstutils-5.4.9/vstutils/api/validators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/api/views.py` & `vstutils-5.4.9/vstutils/api/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/asgi.py` & `vstutils-5.4.9/vstutils/asgi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,38 @@
 import os
 import posixpath
 
 from django.conf import settings
 from django.core.asgi import get_asgi_application
 from django.contrib.staticfiles import finders
-from fastapi import FastAPI
+from fastapi import FastAPI, Request
 from fastapi.responses import PlainTextResponse, FileResponse
 from fastapi.middleware.gzip import GZipMiddleware
+from fastapi.middleware.cors import CORSMiddleware
 from fastapi.staticfiles import StaticFiles
+from starlette.staticfiles import NotModifiedResponse
+
+from .signals import before_mount_app
 
 
 NOT_FOUND_RESPONSE = PlainTextResponse('Not found', status_code=404)
 static_app = FastAPI(openapi_url=None, docs_url=None, redoc_url=None)
 static_app.add_middleware(GZipMiddleware)
 
 application = FastAPI(openapi_url=None, docs_url=None, redoc_url=None)
 application.mount(settings.STATIC_URL, static_app)
+application.add_middleware(
+    CORSMiddleware,
+    allow_origins=settings.CORS_ALLOWED_ORIGINS if not settings.CORS_ORIGIN_ALLOW_ALL else ['*'],
+    expose_headers=settings.CORS_EXPOSE_HEADERS,
+    allow_origin_regex=settings.CORS_ALLOWED_ORIGIN_REGEXES if not settings.CORS_ORIGIN_ALLOW_ALL else None,
+    allow_methods=getattr(settings, 'CORS_ALLOW_METHODS', ("GET",)) if not settings.CORS_ORIGIN_ALLOW_ALL else ['*'],
+    allow_headers=getattr(settings, 'CORS_ALLOW_HEADERS', ()) if not settings.CORS_ORIGIN_ALLOW_ALL else ['*'],
+    allow_credentials=getattr(settings, 'CORS_ALLOWED_CREDENTIALS', settings.CORS_ORIGIN_ALLOW_ALL),
+)
 
 if settings.HAS_DOCS:
     application.mount(
         settings.DOC_URL,
         GZipMiddleware(StaticFiles(directory=settings.DOCS_ROOT, html=True)),
         name="docs"
     )
@@ -29,14 +42,26 @@
         settings.MEDIA_URL,
         GZipMiddleware(StaticFiles(directory=settings.MEDIA_ROOT)),
         name="media"
     )
 
 
 @static_app.get('/{file_path:path}')
-async def static(file_path: str):
+async def static(file_path: str, request: Request = None):
     absolute_path = finders.find(posixpath.normpath(file_path).lstrip("/"))
     if not absolute_path or os.path.isdir(absolute_path):
         return NOT_FOUND_RESPONSE
-    return FileResponse(absolute_path)
+    response = FileResponse(absolute_path, stat_result=os.stat(absolute_path))
+    if request is not None and StaticFiles.is_not_modified(None, response.headers, request.headers):  # type: ignore
+        return NotModifiedResponse(response.headers)
+    return response
+
+
+@application.get('/.well-known/{file_path:path}')
+async def well_known(file_path: str, request: Request):
+    return await static(f'.well-known/{file_path}', request)
+
+
+before_mount_app.send(sender=application, static=static)
 
-application.mount("/", get_asgi_application())
+if not any(m.path == '/' for m in application.routes):
+    application.mount("/", get_asgi_application())
```

### Comparing `vstutils-5.4.8/vstutils/asgi_worker.py` & `vstutils-5.4.9/vstutils/asgi_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/auth.py` & `vstutils-5.4.9/vstutils/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/auth.pyi` & `vstutils-5.4.9/vstutils/auth.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/celery_beat_scheduler.py` & `vstutils-5.4.9/vstutils/celery_beat_scheduler.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/doc_themes/vst-sphinx-theme/layout.html` & `vstutils-5.4.9/vstutils/doc_themes/vst-sphinx-theme/layout.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/environment.py` & `vstutils-5.4.9/vstutils/environment.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/exceptions.py` & `vstutils-5.4.9/vstutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/gui/context.py` & `vstutils-5.4.9/vstutils/gui/context.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/gui/forms.py` & `vstutils-5.4.9/vstutils/gui/forms.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/gui/pwa_manifest.py` & `vstutils-5.4.9/vstutils/gui/pwa_manifest.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/gui/views.py` & `vstutils-5.4.9/vstutils/gui/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/ldap_utils.py` & `vstutils-5.4.9/vstutils/ldap_utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/management/commands/_base.py` & `vstutils-5.4.9/vstutils/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/management/commands/celery_inspect.py` & `vstutils-5.4.9/vstutils/management/commands/celery_inspect.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/management/commands/dockerrun.py` & `vstutils-5.4.9/vstutils/management/commands/dockerrun.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/management/commands/newproject.py` & `vstutils-5.4.9/vstutils/management/commands/newproject.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/management/commands/run_task.py` & `vstutils-5.4.9/vstutils/management/commands/run_task.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/management/commands/runrpc.py` & `vstutils-5.4.9/vstutils/management/commands/runrpc.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/management/commands/runserver.py` & `vstutils-5.4.9/vstutils/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/management/commands/web.py` & `vstutils-5.4.9/vstutils/management/commands/web.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/middleware.py` & `vstutils-5.4.9/vstutils/middleware.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/models/__init__.py` & `vstutils-5.4.9/vstutils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/models/base.py` & `vstutils-5.4.9/vstutils/models/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/models/cent_notify.py` & `vstutils-5.4.9/vstutils/models/cent_notify.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/models/custom_model.py` & `vstutils-5.4.9/vstutils/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/models/custom_model.pyi` & `vstutils-5.4.9/vstutils/models/custom_model.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/models/decorators.py` & `vstutils-5.4.9/vstutils/models/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/models/fields.py` & `vstutils-5.4.9/vstutils/models/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/models/queryset.py` & `vstutils-5.4.9/vstutils/models/queryset.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/settings.ini` & `vstutils-5.4.9/vstutils/settings.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/settings.py` & `vstutils-5.4.9/vstutils/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,16 @@
         'consent_to_processing_path': ConfigStringType,
     }
 
 
 class WebSection(BaseAppendSection):
     types_map = {
         'allow_cors': ConfigBoolType,
+        'cors_allow_all_origins': ConfigBoolType,
+        'cors_allowed_credentials': ConfigBoolType,
         'cors_allowed_origins': ConfigListType,
         'cors_allowed_origins_regexes': ConfigListType,
         'cors_expose_headers': ConfigListType,
         'cors_allow_methods': ConfigListType,
         'cors_allow_headers': ConfigListType,
         'cors_preflight_max_age': ConfigIntSecondsType,
         'session_timeout': ConfigIntSecondsType,
@@ -427,14 +429,15 @@
             'agreement_terms_path': env.str(f'{ENV_NAME}_TERMS_PATH', default=f'/etc/{VST_PROJECT_LIB}/terms.md'),
             'consent_to_processing_path': env.str(
                 f'{ENV_NAME}_CONSENT_TO_PROCESSING_PATH', default=f'/etc/{VST_PROJECT_LIB}/consent_to_processing.md'
             ),
         },
         'web': {
             'allow_cors': env.bool(f'{ENV_NAME}_WEB_ALLOW_CORS', default=False),
+            'cors_allowed_credentials': env.bool(f'{ENV_NAME}_WEB_CORS_ALLOWED_CREDENTIALS', default=False),
             'cors_allowed_origins': env.list(f'{ENV_NAME}_WEB_CORS_ALLOWED_ORIGINS', default=[]),
             'cors_allowed_origins_regexes': env.list(f'{ENV_NAME}_WEB_CORS_ALLOWED_ORIGINS_REGEXES', default=[]),
             'cors_expose_headers': env.list(f'{ENV_NAME}_WEB_CORS_EXPOSE_HEADERS', default=[]),
             'cors_preflight_max_age': env.str(f'{ENV_NAME}_WEB_CORS_PREFLIGHT_MAX_AGE', default='1d'),
             'session_timeout': env.str(f"{ENV_NAME}_SESSION_TIMEOUT", default='2w'),
             'static_files_url': '/static/',
             'page_limit': env.int(f'{ENV_NAME}_WEB_PAGE_LIMIT', default=20),
@@ -645,15 +648,14 @@
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'vstutils',
     'django.contrib.staticfiles',
-    'corsheaders',
 ]
 
 if has_django_celery_beat:
     INSTALLED_APPS.append('django_celery_beat')
 
 INSTALLED_APPS += [
     'crispy_forms',
@@ -675,15 +677,14 @@
 MIDDLEWARE: _t.List[_t.Text] = [
     'vstutils.middleware.ExecuteTimeHeadersMiddleware',
     'vstutils.middleware.FrontendChangesNotifications',
     'htmlmin.middleware.HtmlMinifyMiddleware',
     'htmlmin.middleware.MarkRequestMiddleware',
     'django.middleware.security.SecurityMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
-    'corsheaders.middleware.CorsMiddleware',
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
     'vstutils.middleware.LangMiddleware',
     'vstutils.middleware.TwoFaMiddleware',
@@ -694,15 +695,14 @@
 MIDDLEWARE_ENDPOINT_CONTROL = {
     'remove': [
         'vstutils.middleware.FrontendChangesNotifications',
         'htmlmin.middleware.HtmlMinifyMiddleware',
         'htmlmin.middleware.MarkRequestMiddleware',
         'django.middleware.security.SecurityMiddleware',
         'django.contrib.sessions.middleware.SessionMiddleware',
-        'corsheaders.middleware.CorsMiddleware',
         'django.middleware.common.CommonMiddleware',
         'django.middleware.csrf.CsrfViewMiddleware',
         'django.contrib.auth.middleware.AuthenticationMiddleware',
         'django.contrib.messages.middleware.MessageMiddleware',
         'django.middleware.clickjacking.XFrameOptionsMiddleware',
         'vstutils.middleware.LangMiddleware',
         'vstutils.middleware.TwoFaMiddleware',
@@ -714,15 +714,16 @@
 }
 
 MAX_TFA_ATTEMPTS: int = web['max_tfa_attempts']
 
 # Allow cross-domain access
 CORS_ORIGIN_ALLOW_ALL: bool = web['allow_cors']
 CORS_ALLOWED_ORIGINS: _t.Sequence[str] = web['cors_allowed_origins']
-CORS_ALLOWED_ORIGIN_REGEXES: _t.Sequence[_t.Union[str, _t.Pattern[str]]] = web['cors_allowed_origins_regexes']
+CORS_ALLOWED_CREDENTIALS: bool = web['cors_allowed_credentials']
+CORS_ALLOWED_ORIGIN_REGEXES: _t.Sequence[_t.Union[str, _t.Pattern[str]]] = web['cors_allowed_origins_regexes'] or None
 CORS_EXPOSE_HEADERS: _t.Sequence = web['cors_expose_headers']
 CORS_PREFLIGHT_MAX_AGE: int = web['cors_preflight_max_age']
 if 'cors_allow_methods' in web:
     CORS_ALLOW_METHODS = web['cors_allow_methods']
 if 'cors_allow_headers' in web:
     CORS_ALLOW_HEADERS = web['cors_allow_headers']
```

### Comparing `vstutils-5.4.8/vstutils/static/bundle/281.chunk.js` & `vstutils-5.4.9/vstutils/static/bundle/281.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/296.chunk.js` & `vstutils-5.4.9/vstutils/static/bundle/296.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/345.chunk.js` & `vstutils-5.4.9/vstutils/static/bundle/345.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/368.chunk.js` & `vstutils-5.4.9/vstutils/static/bundle/368.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/421.js` & `vstutils-5.4.9/vstutils/static/bundle/421.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/421.js.LICENSE.txt` & `vstutils-5.4.9/vstutils/static/bundle/421.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/618.js` & `vstutils-5.4.9/vstutils/static/bundle/618.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/683.chunk.js` & `vstutils-5.4.9/vstutils/static/bundle/683.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/686.js` & `vstutils-5.4.9/vstutils/static/bundle/686.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/742.chunk.js` & `vstutils-5.4.9/vstutils/static/bundle/742.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/742.chunk.js.LICENSE.txt` & `vstutils-5.4.9/vstutils/static/bundle/742.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/755.js` & `vstutils-5.4.9/vstutils/static/bundle/755.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/826.chunk.js` & `vstutils-5.4.9/vstutils/static/bundle/826.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/826.chunk.js.LICENSE.txt` & `vstutils-5.4.9/vstutils/static/bundle/826.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/844.js` & `vstutils-5.4.9/vstutils/static/bundle/844.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/959.js` & `vstutils-5.4.9/vstutils/static/bundle/959.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/959.js.LICENSE.txt` & `vstutils-5.4.9/vstutils/static/bundle/959.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/app_loader.js` & `vstutils-5.4.9/vstutils/static/bundle/app_loader.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/base.js` & `vstutils-5.4.9/vstutils/static/bundle/base.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/bb58e57c48a3e911f15f.woff` & `vstutils-5.4.9/vstutils/static/bundle/bb58e57c48a3e911f15f.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff` & `vstutils-5.4.9/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/output.json` & `vstutils-5.4.9/vstutils/static/bundle/output.json`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/spa.js` & `vstutils-5.4.9/vstutils/static/bundle/spa.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/bundle/vstutils.js` & `vstutils-5.4.9/vstutils/static/bundle/vstutils.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static/img/anonymous.png` & `vstutils-5.4.9/vstutils/static/img/anonymous.png`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/static_files.py` & `vstutils-5.4.9/vstutils/static_files.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/tasks.py` & `vstutils-5.4.9/vstutils/tasks.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/auth/base.html` & `vstutils-5.4.9/vstutils/templates/auth/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/auth/language_selector.html` & `vstutils-5.4.9/vstutils/templates/auth/language_selector.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/auth/tfa.html` & `vstutils-5.4.9/vstutils/templates/auth/tfa.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/base.html` & `vstutils-5.4.9/vstutils/templates/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/gui/base.html` & `vstutils-5.4.9/vstutils/templates/gui/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/gui/offline.html` & `vstutils-5.4.9/vstutils/templates/gui/offline.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/gui/service-worker.js` & `vstutils-5.4.9/vstutils/templates/gui/service-worker.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/newproject/.gitignore.template` & `vstutils-5.4.9/vstutils/templates/newproject/.gitignore.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/newproject/frontend_src/.eslintrc.js.template` & `vstutils-5.4.9/vstutils/templates/newproject/frontend_src/.eslintrc.js.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/newproject/package.json.template` & `vstutils-5.4.9/vstutils/templates/newproject/package.json.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/newproject/project_name/settings.py.template` & `vstutils-5.4.9/vstutils/templates/newproject/project_name/settings.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/newproject/setup.cfg.template` & `vstutils-5.4.9/vstutils/templates/newproject/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/newproject/setup.py.template` & `vstutils-5.4.9/vstutils/templates/newproject/setup.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/newproject/test.py.template` & `vstutils-5.4.9/vstutils/templates/newproject/test.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/newproject/tox.ini.template` & `vstutils-5.4.9/vstutils/templates/newproject/tox.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/newproject/tox_build.ini.template` & `vstutils-5.4.9/vstutils/templates/newproject/tox_build.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/newproject/webpack.config.js.default.template` & `vstutils-5.4.9/vstutils/templates/newproject/webpack.config.js.default.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/registration/confirm_email.html` & `vstutils-5.4.9/vstutils/templates/registration/confirm_email.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/registration/password_reset_confirm.html` & `vstutils-5.4.9/vstutils/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/registration/password_reset_form.html` & `vstutils-5.4.9/vstutils/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/registration/user_registration.html` & `vstutils-5.4.9/vstutils/templates/registration/user_registration.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/rest_framework/admin.html` & `vstutils-5.4.9/vstutils/templates/rest_framework/admin.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/vst_inclusion_tags/bootstrap_form.html` & `vstutils-5.4.9/vstutils/templates/vst_inclusion_tags/bootstrap_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templates/widgets/agreement_widget.html` & `vstutils-5.4.9/vstutils/templates/widgets/agreement_widget.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templatetags/request_static.py` & `vstutils-5.4.9/vstutils/templatetags/request_static.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templatetags/translation.py` & `vstutils-5.4.9/vstutils/templatetags/translation.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templatetags/vst_gravatar.py` & `vstutils-5.4.9/vstutils/templatetags/vst_gravatar.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templatetags/vst_html_tags.py` & `vstutils-5.4.9/vstutils/templatetags/vst_html_tags.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/templatetags/vstconfigs.py` & `vstutils-5.4.9/vstutils/templatetags/vstconfigs.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/tests.py` & `vstutils-5.4.9/vstutils/tests.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/tools.py` & `vstutils-5.4.9/vstutils/tools.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/translations/cn.py` & `vstutils-5.4.9/vstutils/translations/cn.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/translations/ru.py` & `vstutils-5.4.9/vstutils/translations/ru.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/translations/vi.py` & `vstutils-5.4.9/vstutils/translations/vi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/urls.py` & `vstutils-5.4.9/vstutils/urls.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/utils.py` & `vstutils-5.4.9/vstutils/utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/web.ini` & `vstutils-5.4.9/vstutils/web.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils/wsgi.py` & `vstutils-5.4.9/vstutils/wsgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.8/vstutils.egg-info/PKG-INFO` & `vstutils-5.4.9/vstutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.4.8
+Version: 5.4.9
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.4.8/vstutils.egg-info/SOURCES.txt` & `vstutils-5.4.9/vstutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 vstutils/exceptions.py
 vstutils/ldap_utils.py
 vstutils/middleware.py
 vstutils/py.typed
 vstutils/session.py
 vstutils/settings.ini
 vstutils/settings.py
+vstutils/signals.py
 vstutils/static_files.py
 vstutils/tasks.py
 vstutils/tests.py
 vstutils/tools.py
 vstutils/urls.py
 vstutils/utils.py
 vstutils/web.ini
```

### Comparing `vstutils-5.4.8/vstutils.egg-info/requires.txt` & `vstutils-5.4.9/vstutils.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 django~=4.1.7
 configparser~=5.3.0
 configparserc~=1.4.0
-django-cors-headers~=4.0.0
 Markdown==3.4.1
 django-environ~=0.10.0
 djangorestframework~=3.14.0
 drf-yasg==1.21.5
 MarkupSafe==2.0.1
 django-filter==23.2
 django-crispy-forms~=1.14.0
```

