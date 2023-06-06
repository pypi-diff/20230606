# Comparing `tmp/money-to-prisoners-common-9.8.1.tar.gz` & `tmp/money-to-prisoners-common-9.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/money-to-prisoners-common-9.8.1.tar", last modified: Fri Aug  9 15:04:50 2019, max compression
+gzip compressed data, was "dist/money-to-prisoners-common-9.9.0.tar", last modified: Fri Sep  6 09:52:35 2019, max compression
```

## Comparing `money-to-prisoners-common-9.8.1.tar` & `money-to-prisoners-common-9.9.0.tar`

### file list

```diff
@@ -1,305 +1,300 @@
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/
--rw-r--r--   0 igorushkarev   (502) staff       (20)     6808 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/PKG-INFO
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/money_to_prisoners_common.egg-info/
--rw-r--r--   0 igorushkarev   (502) staff       (20)     6808 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/money_to_prisoners_common.egg-info/PKG-INFO
--rw-r--r--   0 igorushkarev   (502) staff       (20)    13148 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/money_to_prisoners_common.egg-info/SOURCES.txt
--rw-r--r--   0 igorushkarev   (502) staff       (20)      544 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/money_to_prisoners_common.egg-info/requires.txt
--rw-r--r--   0 igorushkarev   (502) staff       (20)       11 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/money_to_prisoners_common.egg-info/top_level.txt
--rw-r--r--   0 igorushkarev   (502) staff       (20)        1 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/money_to_prisoners_common.egg-info/dependency_links.txt
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1119 2019-06-24 16:35:23.000000 money-to-prisoners-common-9.8.1/LICENSE
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/user_admin/
--rw-r--r--   0 igorushkarev   (502) staff       (20)        0 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/user_admin/__init__.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     7283 2018-08-17 10:32:34.000000 money-to-prisoners-common-9.8.1/mtp_common/user_admin/forms.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)      747 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/user_admin/urls.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)    16174 2019-03-07 17:14:40.000000 money-to-prisoners-common-9.8.1/mtp_common/user_admin/views.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     4071 2018-03-13 11:35:18.000000 money-to-prisoners-common-9.8.1/mtp_common/bank_accounts.py
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/templatetags/
--rw-r--r--   0 igorushkarev   (502) staff       (20)        0 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/templatetags/__init__.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)    13863 2019-08-05 12:13:51.000000 money-to-prisoners-common-9.8.1/mtp_common/templatetags/mtp_common.py
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/metrics/
--rw-r--r--   0 igorushkarev   (502) staff       (20)      792 2019-03-12 11:53:53.000000 money-to-prisoners-common-9.8.1/mtp_common/metrics/metrics.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)       56 2019-03-12 11:53:53.000000 money-to-prisoners-common-9.8.1/mtp_common/metrics/__init__.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)      829 2019-03-12 11:53:53.000000 money-to-prisoners-common-9.8.1/mtp_common/metrics/app.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)      442 2019-03-12 11:53:53.000000 money-to-prisoners-common-9.8.1/mtp_common/metrics/views.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1346 2017-07-05 15:37:16.000000 money-to-prisoners-common-9.8.1/mtp_common/logging.py
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/locale/
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/locale/en_GB/
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/locale/en_GB/LC_MESSAGES/
--rw-r--r--   0 igorushkarev   (502) staff       (20)      511 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/locale/en_GB/LC_MESSAGES/django.mo
--rw-r--r--   0 igorushkarev   (502) staff       (20)      665 2017-08-10 12:59:27.000000 money-to-prisoners-common-9.8.1/mtp_common/locale/en_GB/LC_MESSAGES/djangojs.po
--rw-r--r--   0 igorushkarev   (502) staff       (20)    15950 2018-05-30 14:05:29.000000 money-to-prisoners-common-9.8.1/mtp_common/locale/en_GB/LC_MESSAGES/django.po
--rw-r--r--   0 igorushkarev   (502) staff       (20)      511 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/locale/en_GB/LC_MESSAGES/djangojs.mo
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/locale/cy/
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/locale/cy/LC_MESSAGES/
--rw-r--r--   0 igorushkarev   (502) staff       (20)    12271 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/locale/cy/LC_MESSAGES/django.mo
--rw-r--r--   0 igorushkarev   (502) staff       (20)      804 2017-10-16 14:23:21.000000 money-to-prisoners-common-9.8.1/mtp_common/locale/cy/LC_MESSAGES/djangojs.po
--rw-r--r--   0 igorushkarev   (502) staff       (20)    21217 2018-05-30 14:05:29.000000 money-to-prisoners-common-9.8.1/mtp_common/locale/cy/LC_MESSAGES/django.po
--rw-r--r--   0 igorushkarev   (502) staff       (20)      612 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/locale/cy/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 igorushkarev   (502) staff       (20)     3763 2019-04-10 13:06:35.000000 money-to-prisoners-common-9.8.1/mtp_common/tasks.py
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/forms/
--rw-r--r--   0 igorushkarev   (502) staff       (20)     3512 2019-07-16 11:59:12.000000 money-to-prisoners-common-9.8.1/mtp_common/forms/fields.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1574 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/forms/__init__.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)        0 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/models.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1488 2018-04-17 15:39:17.000000 money-to-prisoners-common-9.8.1/mtp_common/screenshots.py
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/auth/
--rw-r--r--   0 igorushkarev   (502) staff       (20)      417 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/auth/test_utils.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     2820 2017-11-15 17:03:44.000000 money-to-prisoners-common-9.8.1/mtp_common/auth/csrf.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     2462 2018-02-28 14:13:19.000000 money-to-prisoners-common-9.8.1/mtp_common/auth/models.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     4591 2019-06-17 12:11:27.000000 money-to-prisoners-common-9.8.1/mtp_common/auth/__init__.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)    12020 2019-06-27 14:15:23.000000 money-to-prisoners-common-9.8.1/mtp_common/auth/forms.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1124 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/auth/backends.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)      462 2017-09-26 15:45:29.000000 money-to-prisoners-common-9.8.1/mtp_common/auth/exceptions.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     6879 2019-07-16 11:59:11.000000 money-to-prisoners-common-9.8.1/mtp_common/auth/api_client.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1099 2018-01-03 16:43:16.000000 money-to-prisoners-common-9.8.1/mtp_common/auth/middleware.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     9135 2019-07-16 11:59:11.000000 money-to-prisoners-common-9.8.1/mtp_common/auth/views.py
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/test_utils/
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1248 2018-02-26 17:05:08.000000 money-to-prisoners-common-9.8.1/mtp_common/test_utils/code_style.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1006 2017-11-15 17:03:44.000000 money-to-prisoners-common-9.8.1/mtp_common/test_utils/runner.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)    14538 2019-03-08 16:38:05.000000 money-to-prisoners-common-9.8.1/mtp_common/test_utils/functional_tests.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)      261 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/test_utils/__init__.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     4851 2018-04-17 15:39:17.000000 money-to-prisoners-common-9.8.1/mtp_common/test_utils/webdrivers.py
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/management/
--rw-r--r--   0 igorushkarev   (502) staff       (20)        0 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/management/__init__.py
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/management/commands/
--rw-r--r--   0 igorushkarev   (502) staff       (20)      649 2017-08-09 15:53:47.000000 money-to-prisoners-common-9.8.1/mtp_common/management/commands/makemessages.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)        0 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/management/commands/__init__.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)      835 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/management/commands/functionaltest.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)      372 2016-12-14 14:30:09.000000 money-to-prisoners-common-9.8.1/mtp_common/management/commands/takescreenshots.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)      642 2017-07-31 14:11:48.000000 money-to-prisoners-common-9.8.1/mtp_common/management/commands/compilemessages.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)      111 2019-08-09 15:03:30.000000 money-to-prisoners-common-9.8.1/mtp_common/__init__.py
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/feedback/
--rw-r--r--   0 igorushkarev   (502) staff       (20)        0 2017-05-23 13:37:33.000000 money-to-prisoners-common-9.8.1/mtp_common/feedback/__init__.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     2448 2017-05-23 13:37:33.000000 money-to-prisoners-common-9.8.1/mtp_common/feedback/views.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     3502 2019-07-16 11:59:11.000000 money-to-prisoners-common-9.8.1/mtp_common/api.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1539 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/context_processors.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     7127 2018-06-14 16:15:00.000000 money-to-prisoners-common-9.8.1/mtp_common/nomis.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)      280 2019-04-24 13:24:11.000000 money-to-prisoners-common-9.8.1/mtp_common/utils.py
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/
--rw-r--r--   0 igorushkarev   (502) staff       (20)      808 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/year-field-completion.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1207 2017-11-07 17:44:21.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/disclosure.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)      887 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/placeholder-polyfill.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1657 2018-07-20 12:47:11.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/select-all.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)      375 2018-03-08 10:49:43.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/hide-long-text.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)      369 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/element-focus.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1056 2017-07-31 12:19:06.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/unload.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)     6486 2018-11-13 15:21:36.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/date-picker.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)     4231 2019-08-05 12:13:51.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/tabbed-panel.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1894 2018-03-13 14:18:27.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/polyfills.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)     3758 2017-07-31 12:03:49.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/dialogue-box.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1275 2017-07-31 14:11:48.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/upload.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1763 2018-03-13 11:35:18.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/mailcheck-warning.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)     2329 2017-05-23 13:37:33.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/footer-feedback.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1284 2018-03-08 10:49:43.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/character-count-warning.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1348 2019-03-22 17:22:54.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/analytics.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)      312 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/track-printing.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)      476 2018-05-22 13:21:06.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/async-load.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)      925 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/notifications.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)     3931 2019-03-15 16:09:07.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/autocomplete-select.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)      144 2017-11-30 15:32:42.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/messages.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)     2439 2017-07-18 13:17:01.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/print.js
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/
--rw-r--r--   0 igorushkarev   (502) staff       (20)      146 2019-03-07 17:14:40.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/_mtp-internal.scss
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/internal/
--rw-r--r--   0 igorushkarev   (502) staff       (20)     2986 2019-01-11 14:12:44.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/internal/_notifications.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1168 2017-11-10 15:00:28.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/internal/_proposition-extra.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      599 2019-03-07 17:14:40.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/internal/_settings.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      765 2017-11-10 15:00:28.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/internal/_overrides.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      174 2017-11-10 15:00:28.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/_print-basic.scss
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1580 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_checkbox.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      559 2018-07-20 12:47:11.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_sub-nav.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)     3214 2019-08-05 12:13:51.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_tabbed-panel.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      586 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_important.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1048 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_large-link.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)     2213 2018-11-12 10:13:22.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_date-picker.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1907 2018-09-25 17:05:45.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_table.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      584 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_forms.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      301 2017-05-23 13:37:33.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_buttons.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      531 2017-05-23 13:37:33.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_footer-feedback.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      670 2017-06-13 14:20:19.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_disclosure.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)     2996 2019-07-25 11:22:03.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_pagination.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      985 2017-07-18 13:17:01.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_dialogue-box.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      101 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_placeholder-polyfill.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      199 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_print-box.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)       70 2018-03-08 10:49:43.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_character-count-warning.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      308 2019-03-15 16:09:07.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_autocomplete.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      369 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_spinner.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      199 2018-03-13 11:35:18.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_mailcheck-warning.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      309 2019-08-09 15:02:31.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_ie-support-banner.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      631 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_delete-icons.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1504 2018-09-25 17:05:45.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_account-management.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      443 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_upload.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1315 2017-08-09 15:53:47.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_messages.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      678 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/_mtp.scss
--rw-r--r--   0 igorushkarev   (502) staff       (20)      583 2017-11-22 12:33:20.000000 money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/_base.scss
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/static/
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/
--rw-r--r--   0 igorushkarev   (502) staff       (20)      534 2019-07-08 13:44:52.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/page-list@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      162 2019-07-08 13:44:52.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/ordering-asc@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      829 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/govuk-header-logo.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      996 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/arrow-sprite.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      396 2017-08-09 15:53:47.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/message-info.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      344 2017-06-20 15:24:59.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/pagination-sprite.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1724 2017-12-05 12:19:12.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/notification-control@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      412 2017-08-09 15:53:47.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/message-success.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      248 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/select-dropdown@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      499 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/undelete-icon@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      144 2018-11-08 16:52:34.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/date-picker.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      513 2017-11-10 15:00:28.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/proposition-user-icon.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      201 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/select-dropdown-focused.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      116 2019-07-08 13:44:52.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/ordering-asc.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      459 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/collapse-button@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)       95 2018-07-20 12:47:11.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/checkbox@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      576 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/delete-icon@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      606 2017-08-09 15:53:47.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/message-error@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      533 2017-11-10 15:00:28.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/proposition-user-icon-focused.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      939 2017-08-09 15:53:47.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/message-warning@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      551 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/pagination-sprite@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      654 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/message-success@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      262 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/expand-button.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      237 2016-12-14 14:30:09.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/large-link-arrow.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      240 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/collapse-button.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1937 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/arrow-sprite@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      240 2018-07-20 12:47:11.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/checkbox-checked.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      415 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/important.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1510 2019-07-08 13:44:52.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/crest-moj.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      246 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/select-dropdown-focused@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      201 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/select-dropdown.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      198 2019-07-08 13:44:52.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/checkmark.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)     4643 2019-08-09 15:02:31.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/firefox.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      946 2017-11-10 15:00:28.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/proposition-user-icon@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      966 2017-11-10 15:00:28.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/proposition-user-icon-focused@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      279 2016-12-14 14:30:09.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/help-arrows.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)     2903 2019-04-05 15:18:10.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/govuk-header-logo-email.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      200 2018-07-20 12:47:11.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/ordering-none@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      101 2019-07-08 13:44:52.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/header-back-arrow.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      451 2016-12-14 14:30:09.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/help-arrows@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1198 2017-12-05 12:19:12.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/notification-control.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      330 2018-07-20 12:47:11.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/checkbox-checked@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      104 2019-07-08 13:44:52.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/header-back-arrow@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      181 2019-07-08 13:44:52.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/ordering-desc@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      362 2017-08-09 15:53:47.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/message-error.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      533 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/message-warning.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      311 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/large-link-arrow@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      289 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/undelete-icon.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      251 2019-07-08 13:44:52.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/checkmark@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1873 2017-11-10 15:00:28.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/crest-moj@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      664 2017-08-09 15:53:47.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/message-info@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      103 2018-07-20 12:47:11.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/checkbox.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      285 2019-07-08 13:44:52.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/page-list.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      149 2018-11-08 16:52:34.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/date-picker@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      145 2018-07-20 12:47:11.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/ordering-none.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      294 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/delete-icon.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      479 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/expand-button@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      918 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/important@2x.png
--rw-r--r--   0 igorushkarev   (502) staff       (20)      124 2018-07-20 12:47:11.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/ordering-desc.png
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/javascripts/
--rw-r--r--   0 igorushkarev   (502) staff       (20)    34117 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/javascripts/webfont-debug.js
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/a11y/
--rw-r--r--   0 igorushkarev   (502) staff       (20)   110469 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/a11y/axs_testing.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)   121427 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/a11y/HTMLCS.js
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/static/stylesheets/
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1173 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/static/stylesheets/fonts-ie8.css
--rw-r--r--   0 igorushkarev   (502) staff       (20)     3500 2019-03-12 11:53:53.000000 money-to-prisoners-common-9.8.1/mtp_common/stack.py
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/build_tasks/
--rw-r--r--   0 igorushkarev   (502) staff       (20)    13991 2019-08-09 15:03:11.000000 money-to-prisoners-common-9.8.1/mtp_common/build_tasks/tasks.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1831 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/build_tasks/paths.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)        0 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/build_tasks/__init__.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     4295 2017-11-07 17:31:49.000000 money-to-prisoners-common-9.8.1/mtp_common/build_tasks/app.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)    19195 2019-07-16 11:59:12.000000 money-to-prisoners-common-9.8.1/mtp_common/build_tasks/executor.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)      331 2017-08-10 12:59:27.000000 money-to-prisoners-common-9.8.1/mtp_common/app.py
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/
--rw-r--r--   0 igorushkarev   (502) staff       (20)     6148 2019-04-05 14:22:44.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/.DS_Store
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1943 2018-08-21 15:55:16.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/update.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     6148 2018-08-09 11:51:03.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/.DS_Store
--rw-r--r--   0 igorushkarev   (502) staff       (20)      276 2017-08-09 15:53:47.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/base.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      819 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/undelete.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     4698 2018-09-25 17:05:45.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/list.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      249 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/sign-up-has-role.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      381 2017-07-05 15:37:16.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/deleted.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1190 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/sign-up.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      813 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/user-description.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      557 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/saved.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      537 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/sign-up-success.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1570 2018-09-25 17:05:45.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/accept-request.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      506 2018-12-06 17:34:24.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/incompatible-admin.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      817 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/delete.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      919 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/sign-up-confirm-changes.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      763 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/sign-up-has-other-roles.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      549 2017-07-05 15:37:16.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/incompatible-user.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      381 2017-07-05 15:37:16.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/undeleted.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     6148 2019-04-05 14:22:53.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/.DS_Store
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/
--rw-r--r--   0 igorushkarev   (502) staff       (20)     6148 2018-11-06 12:39:49.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/.DS_Store
--rw-r--r--   0 igorushkarev   (502) staff       (20)      327 2017-05-23 13:37:33.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/field-label.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      942 2018-11-08 16:52:34.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/checkbox-field.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1085 2018-03-08 10:49:43.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/textarea.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1060 2018-11-08 16:52:34.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/radio-field.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      127 2017-05-23 13:37:33.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/field-help-text.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1167 2017-07-05 15:37:16.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/error-summary.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1312 2018-11-12 10:13:22.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/date-picker-field.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1259 2018-08-16 14:00:13.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/generic.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1035 2018-03-08 10:49:43.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/field.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      259 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/field-errors.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1484 2018-11-06 12:35:16.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/select-field.html
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/auth/
--rw-r--r--   0 igorushkarev   (502) staff       (20)      311 2017-08-09 16:43:20.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/auth/password_change_with_code.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      739 2019-06-17 12:11:27.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/auth/email-change-email.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      313 2017-07-05 15:37:16.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/auth/reset-password.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1701 2017-11-10 15:00:28.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/auth/login.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      309 2019-06-17 12:11:27.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/auth/email-change.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      427 2019-06-17 12:11:27.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/auth/email-change-email.txt
--rw-r--r--   0 igorushkarev   (502) staff       (20)      627 2017-08-09 16:43:20.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/auth/reset-password-done.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      528 2017-07-05 15:37:16.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/auth/password_change_done.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      315 2017-07-05 15:37:16.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/auth/password_change.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      276 2018-04-18 10:34:08.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/sentry-js.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      931 2017-11-10 15:00:28.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/sub-nav.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     4911 2019-08-09 13:43:55.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/mtp_base.html
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/
--rw-r--r--   0 igorushkarev   (502) staff       (20)      685 2019-08-05 12:13:51.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/tabbed-panel.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      245 2017-08-09 15:53:47.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/message_box.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      283 2018-07-20 12:47:11.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/sortable-cell.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      625 2018-09-25 17:05:45.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/notifications.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     2617 2019-07-08 13:44:52.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/page-list.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      132 2018-01-08 15:30:12.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/panel-tab.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1229 2017-05-23 13:37:33.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/footer-feedback.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      521 2019-03-07 17:14:40.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/proposition-user-menu.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      650 2017-11-10 15:00:28.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/language-switch.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      748 2017-07-18 13:17:01.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/dialogue-box.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)   300312 2017-08-10 12:59:27.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/maintenance-citizen.html
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/feedback/
--rw-r--r--   0 igorushkarev   (502) staff       (20)     2121 2018-12-06 17:34:24.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/feedback/submit_feedback.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      723 2018-12-06 17:34:24.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/feedback/success.html
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/build_tasks/
--rw-r--r--   0 igorushkarev   (502) staff       (20)      304 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/build_tasks/sass-lint.yml
--rw-r--r--   0 igorushkarev   (502) staff       (20)     6148 2016-12-01 16:38:41.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/build_tasks/.DS_Store
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1831 2017-07-18 13:17:01.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/build_tasks/eslintrc.json
--rw-r--r--   0 igorushkarev   (502) staff       (20)      645 2017-11-10 15:00:28.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/build_tasks/webpack.config.js
--rw-r--r--   0 igorushkarev   (502) staff       (20)      818 2018-12-12 10:42:11.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/build_tasks/package.json
--rw-r--r--   0 igorushkarev   (502) staff       (20)      336 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/build_tasks/docker-compose.yml
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/errors/
--rw-r--r--   0 igorushkarev   (502) staff       (20)      567 2017-07-05 15:37:16.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/errors/500.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      535 2017-07-05 15:37:16.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/errors/404.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      582 2017-07-05 15:37:16.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/errors/400.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1431 2019-06-17 12:11:27.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/settings.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1500 2016-11-14 16:55:38.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/a11y.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)   300122 2017-08-10 12:59:27.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/maintenance.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)      348 2019-08-09 15:02:31.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/ie-support-banner.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)     3575 2019-06-17 12:11:27.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/email_base.html
-drwxr-xr-x   0 igorushkarev   (502) staff       (20)        0 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/govuk_template/
--rw-r--r--   0 igorushkarev   (502) staff       (20)     5055 2017-09-27 11:52:39.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/govuk_template/base.html
--rw-r--r--   0 igorushkarev   (502) staff       (20)       16 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/mtp_common/templates/.gitignore
--rw-r--r--   0 igorushkarev   (502) staff       (20)      725 2017-12-19 14:39:26.000000 money-to-prisoners-common-9.8.1/mtp_common/dates.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)      781 2019-03-22 17:22:54.000000 money-to-prisoners-common-9.8.1/mtp_common/analytics.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     1672 2018-01-04 10:16:13.000000 money-to-prisoners-common-9.8.1/mtp_common/views.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)     6131 2018-02-28 14:13:19.000000 money-to-prisoners-common-9.8.1/mtp_common/spooling.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)      621 2017-03-13 16:42:49.000000 money-to-prisoners-common-9.8.1/MANIFEST.in
--rw-r--r--   0 igorushkarev   (502) staff       (20)     2136 2019-07-16 11:59:12.000000 money-to-prisoners-common-9.8.1/setup.py
--rw-r--r--   0 igorushkarev   (502) staff       (20)      162 2019-08-09 15:04:50.000000 money-to-prisoners-common-9.8.1/setup.cfg
--rw-r--r--   0 igorushkarev   (502) staff       (20)     5025 2019-03-14 15:42:55.000000 money-to-prisoners-common-9.8.1/README.rst
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1119 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/LICENSE
+-rw-r--r--   0 marcofucci   (501) staff       (20)      621 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/MANIFEST.in
+-rw-r--r--   0 marcofucci   (501) staff       (20)     6808 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/PKG-INFO
+-rw-r--r--   0 marcofucci   (501) staff       (20)     5025 2019-09-06 09:44:25.000000 money-to-prisoners-common-9.9.0/README.rst
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/money_to_prisoners_common.egg-info/
+-rw-r--r--   0 marcofucci   (501) staff       (20)     6808 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/money_to_prisoners_common.egg-info/PKG-INFO
+-rw-r--r--   0 marcofucci   (501) staff       (20)    12920 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/money_to_prisoners_common.egg-info/SOURCES.txt
+-rw-r--r--   0 marcofucci   (501) staff       (20)        1 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/money_to_prisoners_common.egg-info/dependency_links.txt
+-rw-r--r--   0 marcofucci   (501) staff       (20)      544 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/money_to_prisoners_common.egg-info/requires.txt
+-rw-r--r--   0 marcofucci   (501) staff       (20)       11 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/money_to_prisoners_common.egg-info/top_level.txt
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/
+-rw-r--r--   0 marcofucci   (501) staff       (20)      111 2019-09-06 09:51:01.000000 money-to-prisoners-common-9.9.0/mtp_common/__init__.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1192 2019-09-06 08:59:20.000000 money-to-prisoners-common-9.9.0/mtp_common/analytics.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     3502 2019-07-25 10:58:05.000000 money-to-prisoners-common-9.9.0/mtp_common/api.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)      331 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/app.py
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1809 2019-09-06 09:16:17.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/analytics.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)      476 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/async-load.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)     3931 2019-08-15 15:54:44.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/autocomplete-select.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1284 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/character-count-warning.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)     6486 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/date-picker.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)     3758 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/dialogue-box.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1207 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/disclosure.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)      369 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/element-focus.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)     2329 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/footer-feedback.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)      375 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/hide-long-text.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1763 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/mailcheck-warning.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)      144 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/messages.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)      925 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/notifications.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)      887 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/placeholder-polyfill.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1894 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/polyfills.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)     2439 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/print.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1657 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/select-all.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)     4231 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/tabbed-panel.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)      312 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/track-printing.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1056 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/unload.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1275 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/upload.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)      808 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/year-field-completion.js
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/
+-rw-r--r--   0 marcofucci   (501) staff       (20)      583 2019-08-09 14:16:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/_base.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      146 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/_mtp-internal.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      678 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/_mtp.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      174 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/_print-basic.scss
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1504 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_account-management.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      308 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_autocomplete.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      301 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_buttons.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)       70 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_character-count-warning.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1580 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_checkbox.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)     2213 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_date-picker.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      631 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_delete-icons.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      985 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_dialogue-box.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      670 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_disclosure.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      531 2019-08-09 14:14:26.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_footer-feedback.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      584 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_forms.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      309 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_ie-support-banner.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      586 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_important.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1048 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_large-link.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      199 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_mailcheck-warning.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1315 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_messages.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)     2996 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_pagination.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      101 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_placeholder-polyfill.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      199 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_print-box.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      369 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_spinner.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      559 2019-07-05 13:22:19.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_sub-nav.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)     3214 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_tabbed-panel.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1907 2019-07-23 15:16:20.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_table.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      443 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_upload.scss
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/internal/
+-rw-r--r--   0 marcofucci   (501) staff       (20)     2986 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/internal/_notifications.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      765 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/internal/_overrides.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1168 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/internal/_proposition-extra.scss
+-rw-r--r--   0 marcofucci   (501) staff       (20)      599 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/internal/_settings.scss
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/auth/
+-rw-r--r--   0 marcofucci   (501) staff       (20)     4591 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/auth/__init__.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     6879 2019-07-25 10:58:05.000000 money-to-prisoners-common-9.9.0/mtp_common/auth/api_client.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1124 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/auth/backends.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     2820 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/auth/csrf.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)      462 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/auth/exceptions.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)    12020 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/auth/forms.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1099 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/auth/middleware.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     2462 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/auth/models.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)      417 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/auth/test_utils.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     9135 2019-07-25 10:58:05.000000 money-to-prisoners-common-9.9.0/mtp_common/auth/views.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     4071 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/bank_accounts.py
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/build_tasks/
+-rw-r--r--   0 marcofucci   (501) staff       (20)        0 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/build_tasks/__init__.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     4295 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/build_tasks/app.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)    19195 2019-07-25 10:58:05.000000 money-to-prisoners-common-9.9.0/mtp_common/build_tasks/executor.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1831 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/build_tasks/paths.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)    13991 2019-09-02 14:47:24.000000 money-to-prisoners-common-9.9.0/mtp_common/build_tasks/tasks.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1539 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/context_processors.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)      725 2019-07-04 09:09:58.000000 money-to-prisoners-common-9.9.0/mtp_common/dates.py
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/feedback/
+-rw-r--r--   0 marcofucci   (501) staff       (20)        0 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/feedback/__init__.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     2448 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/feedback/views.py
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/forms/
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1574 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/forms/__init__.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     3512 2019-07-25 10:58:05.000000 money-to-prisoners-common-9.9.0/mtp_common/forms/fields.py
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/locale/
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/locale/cy/
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/locale/cy/LC_MESSAGES/
+-rw-r--r--   0 marcofucci   (501) staff       (20)    12230 2019-09-06 09:52:34.000000 money-to-prisoners-common-9.9.0/mtp_common/locale/cy/LC_MESSAGES/django.mo
+-rw-r--r--   0 marcofucci   (501) staff       (20)    21217 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/locale/cy/LC_MESSAGES/django.po
+-rw-r--r--   0 marcofucci   (501) staff       (20)      571 2019-09-06 09:52:34.000000 money-to-prisoners-common-9.9.0/mtp_common/locale/cy/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 marcofucci   (501) staff       (20)      804 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/locale/cy/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/locale/en_GB/
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/locale/en_GB/LC_MESSAGES/
+-rw-r--r--   0 marcofucci   (501) staff       (20)      470 2019-09-06 09:52:34.000000 money-to-prisoners-common-9.9.0/mtp_common/locale/en_GB/LC_MESSAGES/django.mo
+-rw-r--r--   0 marcofucci   (501) staff       (20)    15950 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/locale/en_GB/LC_MESSAGES/django.po
+-rw-r--r--   0 marcofucci   (501) staff       (20)      470 2019-09-06 09:52:34.000000 money-to-prisoners-common-9.9.0/mtp_common/locale/en_GB/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 marcofucci   (501) staff       (20)      665 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/locale/en_GB/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1346 2019-07-04 09:12:22.000000 money-to-prisoners-common-9.9.0/mtp_common/logging.py
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/management/
+-rw-r--r--   0 marcofucci   (501) staff       (20)        0 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/management/__init__.py
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/management/commands/
+-rw-r--r--   0 marcofucci   (501) staff       (20)        0 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/management/commands/__init__.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)      642 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/management/commands/compilemessages.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)      835 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/management/commands/functionaltest.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)      649 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/management/commands/makemessages.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)      372 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/management/commands/takescreenshots.py
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/metrics/
+-rw-r--r--   0 marcofucci   (501) staff       (20)       56 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/metrics/__init__.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)      829 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/metrics/app.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)      792 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/metrics/metrics.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)      442 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/metrics/views.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)        0 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/models.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     7127 2019-07-03 16:20:13.000000 money-to-prisoners-common-9.9.0/mtp_common/nomis.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1488 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/screenshots.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     6131 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/spooling.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     3500 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/stack.py
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/static/
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/a11y/
+-rw-r--r--   0 marcofucci   (501) staff       (20)   121427 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/a11y/HTMLCS.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)   110469 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/a11y/axs_testing.js
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/
+-rw-r--r--   0 marcofucci   (501) staff       (20)      996 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/arrow-sprite.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1937 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/arrow-sprite@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      240 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/checkbox-checked.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      330 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/checkbox-checked@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      103 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/checkbox.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)       95 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/checkbox@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      198 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/checkmark.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      251 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/checkmark@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      240 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/collapse-button.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      459 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/collapse-button@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1510 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/crest-moj.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1873 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/crest-moj@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      144 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/date-picker.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      149 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/date-picker@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      294 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/delete-icon.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      576 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/delete-icon@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      262 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/expand-button.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      479 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/expand-button@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)     4643 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/firefox.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)     2903 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/govuk-header-logo-email.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      829 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/govuk-header-logo.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      101 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/header-back-arrow.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      104 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/header-back-arrow@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      279 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/help-arrows.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      451 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/help-arrows@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      415 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/important.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      918 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/important@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      237 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/large-link-arrow.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      311 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/large-link-arrow@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      362 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/message-error.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      606 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/message-error@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      396 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/message-info.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      664 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/message-info@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      412 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/message-success.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      654 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/message-success@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      533 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/message-warning.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      939 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/message-warning@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1198 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/notification-control.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1724 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/notification-control@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      116 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/ordering-asc.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      162 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/ordering-asc@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      124 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/ordering-desc.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      181 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/ordering-desc@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      145 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/ordering-none.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      200 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/ordering-none@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      285 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/page-list.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      534 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/page-list@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      344 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/pagination-sprite.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      551 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/pagination-sprite@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      533 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/proposition-user-icon-focused.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      966 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/proposition-user-icon-focused@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      513 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/proposition-user-icon.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      946 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/proposition-user-icon@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      201 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/select-dropdown-focused.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      246 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/select-dropdown-focused@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      201 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/select-dropdown.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      248 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/select-dropdown@2x.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      289 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/undelete-icon.png
+-rw-r--r--   0 marcofucci   (501) staff       (20)      499 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/undelete-icon@2x.png
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/javascripts/
+-rw-r--r--   0 marcofucci   (501) staff       (20)    34117 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/javascripts/webfont-debug.js
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/static/stylesheets/
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1173 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/static/stylesheets/fonts-ie8.css
+-rw-r--r--   0 marcofucci   (501) staff       (20)     3763 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/tasks.py
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/
+-rw-r--r--   0 marcofucci   (501) staff       (20)       16 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/.gitignore
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/govuk_template/
+-rw-r--r--   0 marcofucci   (501) staff       (20)     5055 2017-09-27 11:52:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/govuk_template/base.html
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1500 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/a11y.html
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/auth/
+-rw-r--r--   0 marcofucci   (501) staff       (20)      739 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/auth/email-change-email.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      427 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/auth/email-change-email.txt
+-rw-r--r--   0 marcofucci   (501) staff       (20)      309 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/auth/email-change.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1701 2019-07-11 10:54:38.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/auth/login.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      315 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/auth/password_change.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      528 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/auth/password_change_done.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      311 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/auth/password_change_with_code.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      627 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/auth/reset-password-done.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      313 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/auth/reset-password.html
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/build_tasks/
+-rw-r--r--   0 marcofucci   (501) staff       (20)      336 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/build_tasks/docker-compose.yml
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1831 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/build_tasks/eslintrc.json
+-rw-r--r--   0 marcofucci   (501) staff       (20)      818 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/build_tasks/package.json
+-rw-r--r--   0 marcofucci   (501) staff       (20)      304 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/build_tasks/sass-lint.yml
+-rw-r--r--   0 marcofucci   (501) staff       (20)      645 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/build_tasks/webpack.config.js
+-rw-r--r--   0 marcofucci   (501) staff       (20)     3575 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/email_base.html
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/errors/
+-rw-r--r--   0 marcofucci   (501) staff       (20)      582 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/errors/400.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      535 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/errors/404.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      567 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/errors/500.html
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/feedback/
+-rw-r--r--   0 marcofucci   (501) staff       (20)     2121 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/feedback/submit_feedback.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      723 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/feedback/success.html
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/
+-rw-r--r--   0 marcofucci   (501) staff       (20)      942 2019-08-12 11:17:00.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/checkbox-field.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1312 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/date-picker-field.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1167 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/error-summary.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      259 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/field-errors.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      127 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/field-help-text.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      327 2019-08-12 11:16:18.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/field-label.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1035 2019-08-12 11:05:33.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/field.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1259 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/generic.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1060 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/radio-field.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1484 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/select-field.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1085 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/textarea.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      348 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/ie-support-banner.html
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/
+-rw-r--r--   0 marcofucci   (501) staff       (20)      748 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/dialogue-box.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1229 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/footer-feedback.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      650 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/language-switch.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      245 2019-07-11 10:19:40.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/message_box.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      625 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/notifications.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     2617 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/page-list.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      132 2019-07-29 15:16:50.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/panel-tab.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      521 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/proposition-user-menu.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      283 2019-09-05 14:26:47.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/sortable-cell.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      685 2019-09-02 14:49:26.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/tabbed-panel.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)   300312 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/maintenance-citizen.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)   300122 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/maintenance.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     4664 2019-09-06 08:59:20.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/mtp_base.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      276 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/sentry-js.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1431 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/settings.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      931 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/sub-nav.html
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1570 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/accept-request.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      276 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/base.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      817 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/delete.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      381 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/deleted.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      506 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/incompatible-admin.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      549 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/incompatible-user.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     4698 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/list.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      557 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/saved.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      919 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/sign-up-confirm-changes.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      763 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/sign-up-has-other-roles.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      249 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/sign-up-has-role.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      537 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/sign-up-success.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1190 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/sign-up.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      819 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/undelete.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      381 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/undeleted.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1943 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/update.html
+-rw-r--r--   0 marcofucci   (501) staff       (20)      813 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/user-description.html
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/templatetags/
+-rw-r--r--   0 marcofucci   (501) staff       (20)        0 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/templatetags/__init__.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)    13863 2019-09-05 14:24:21.000000 money-to-prisoners-common-9.9.0/mtp_common/templatetags/mtp_common.py
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/test_utils/
+-rw-r--r--   0 marcofucci   (501) staff       (20)      261 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/test_utils/__init__.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1248 2019-07-04 14:00:04.000000 money-to-prisoners-common-9.9.0/mtp_common/test_utils/code_style.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)    14538 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/test_utils/functional_tests.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1006 2019-07-09 10:43:05.000000 money-to-prisoners-common-9.9.0/mtp_common/test_utils/runner.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     4851 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/test_utils/webdrivers.py
+drwxr-xr-x   0 marcofucci   (501) staff       (20)        0 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/mtp_common/user_admin/
+-rw-r--r--   0 marcofucci   (501) staff       (20)        0 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/user_admin/__init__.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     7283 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/user_admin/forms.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)      747 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/user_admin/urls.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)    16174 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/user_admin/views.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)      280 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/utils.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)     1672 2019-07-03 09:38:39.000000 money-to-prisoners-common-9.9.0/mtp_common/views.py
+-rw-r--r--   0 marcofucci   (501) staff       (20)      162 2019-09-06 09:52:35.000000 money-to-prisoners-common-9.9.0/setup.cfg
+-rw-r--r--   0 marcofucci   (501) staff       (20)     2136 2019-08-30 10:18:58.000000 money-to-prisoners-common-9.9.0/setup.py
```

### Comparing `money-to-prisoners-common-9.8.1/PKG-INFO` & `money-to-prisoners-common-9.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: money-to-prisoners-common
-Version: 9.8.1
+Version: 9.9.0
 Summary: Django app with common code and assets for Money to Prisoners serivces
 Home-page: https://github.com/ministryofjustice/money-to-prisoners-common
 Author: Ministry of Justice Digital Services
 License: MIT
 Description: Money to Prisoners
         ==================
         
@@ -148,9 +148,9 @@
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
-Provides-Extra: monitoring
 Provides-Extra: testing
+Provides-Extra: monitoring
```

### Comparing `money-to-prisoners-common-9.8.1/money_to_prisoners_common.egg-info/PKG-INFO` & `money-to-prisoners-common-9.9.0/money_to_prisoners_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: money-to-prisoners-common
-Version: 9.8.1
+Version: 9.9.0
 Summary: Django app with common code and assets for Money to Prisoners serivces
 Home-page: https://github.com/ministryofjustice/money-to-prisoners-common
 Author: Ministry of Justice Digital Services
 License: MIT
 Description: Money to Prisoners
         ==================
         
@@ -148,9 +148,9 @@
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
-Provides-Extra: monitoring
 Provides-Extra: testing
+Provides-Extra: monitoring
```

### Comparing `money-to-prisoners-common-9.8.1/money_to_prisoners_common.egg-info/SOURCES.txt` & `money-to-prisoners-common-9.9.0/money_to_prisoners_common.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -174,18 +174,16 @@
 mtp_common/static/mtp_common/images/select-dropdown-focused@2x.png
 mtp_common/static/mtp_common/images/select-dropdown.png
 mtp_common/static/mtp_common/images/select-dropdown@2x.png
 mtp_common/static/mtp_common/images/undelete-icon.png
 mtp_common/static/mtp_common/images/undelete-icon@2x.png
 mtp_common/static/mtp_common/javascripts/webfont-debug.js
 mtp_common/static/stylesheets/fonts-ie8.css
-mtp_common/templates/.DS_Store
 mtp_common/templates/.gitignore
 mtp_common/templates/govuk_template/base.html
-mtp_common/templates/mtp_common/.DS_Store
 mtp_common/templates/mtp_common/a11y.html
 mtp_common/templates/mtp_common/email_base.html
 mtp_common/templates/mtp_common/ie-support-banner.html
 mtp_common/templates/mtp_common/maintenance-citizen.html
 mtp_common/templates/mtp_common/maintenance.html
 mtp_common/templates/mtp_common/mtp_base.html
 mtp_common/templates/mtp_common/sentry-js.html
@@ -196,26 +194,24 @@
 mtp_common/templates/mtp_common/auth/email-change.html
 mtp_common/templates/mtp_common/auth/login.html
 mtp_common/templates/mtp_common/auth/password_change.html
 mtp_common/templates/mtp_common/auth/password_change_done.html
 mtp_common/templates/mtp_common/auth/password_change_with_code.html
 mtp_common/templates/mtp_common/auth/reset-password-done.html
 mtp_common/templates/mtp_common/auth/reset-password.html
-mtp_common/templates/mtp_common/build_tasks/.DS_Store
 mtp_common/templates/mtp_common/build_tasks/docker-compose.yml
 mtp_common/templates/mtp_common/build_tasks/eslintrc.json
 mtp_common/templates/mtp_common/build_tasks/package.json
 mtp_common/templates/mtp_common/build_tasks/sass-lint.yml
 mtp_common/templates/mtp_common/build_tasks/webpack.config.js
 mtp_common/templates/mtp_common/errors/400.html
 mtp_common/templates/mtp_common/errors/404.html
 mtp_common/templates/mtp_common/errors/500.html
 mtp_common/templates/mtp_common/feedback/submit_feedback.html
 mtp_common/templates/mtp_common/feedback/success.html
-mtp_common/templates/mtp_common/forms/.DS_Store
 mtp_common/templates/mtp_common/forms/checkbox-field.html
 mtp_common/templates/mtp_common/forms/date-picker-field.html
 mtp_common/templates/mtp_common/forms/error-summary.html
 mtp_common/templates/mtp_common/forms/field-errors.html
 mtp_common/templates/mtp_common/forms/field-help-text.html
 mtp_common/templates/mtp_common/forms/field-label.html
 mtp_common/templates/mtp_common/forms/field.html
@@ -229,15 +225,14 @@
 mtp_common/templates/mtp_common/includes/message_box.html
 mtp_common/templates/mtp_common/includes/notifications.html
 mtp_common/templates/mtp_common/includes/page-list.html
 mtp_common/templates/mtp_common/includes/panel-tab.html
 mtp_common/templates/mtp_common/includes/proposition-user-menu.html
 mtp_common/templates/mtp_common/includes/sortable-cell.html
 mtp_common/templates/mtp_common/includes/tabbed-panel.html
-mtp_common/templates/mtp_common/user_admin/.DS_Store
 mtp_common/templates/mtp_common/user_admin/accept-request.html
 mtp_common/templates/mtp_common/user_admin/base.html
 mtp_common/templates/mtp_common/user_admin/delete.html
 mtp_common/templates/mtp_common/user_admin/deleted.html
 mtp_common/templates/mtp_common/user_admin/incompatible-admin.html
 mtp_common/templates/mtp_common/user_admin/incompatible-user.html
 mtp_common/templates/mtp_common/user_admin/list.html
```

### Comparing `money-to-prisoners-common-9.8.1/money_to_prisoners_common.egg-info/requires.txt` & `money-to-prisoners-common-9.9.0/money_to_prisoners_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/LICENSE` & `money-to-prisoners-common-9.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/user_admin/forms.py` & `money-to-prisoners-common-9.9.0/mtp_common/user_admin/forms.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/user_admin/urls.py` & `money-to-prisoners-common-9.9.0/mtp_common/user_admin/urls.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/user_admin/views.py` & `money-to-prisoners-common-9.9.0/mtp_common/user_admin/views.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/bank_accounts.py` & `money-to-prisoners-common-9.9.0/mtp_common/bank_accounts.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templatetags/mtp_common.py` & `money-to-prisoners-common-9.9.0/mtp_common/templatetags/mtp_common.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/metrics/metrics.py` & `money-to-prisoners-common-9.9.0/mtp_common/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/metrics/app.py` & `money-to-prisoners-common-9.9.0/mtp_common/metrics/app.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/logging.py` & `money-to-prisoners-common-9.9.0/mtp_common/logging.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/locale/en_GB/LC_MESSAGES/djangojs.po` & `money-to-prisoners-common-9.9.0/mtp_common/locale/en_GB/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/locale/en_GB/LC_MESSAGES/django.po` & `money-to-prisoners-common-9.9.0/mtp_common/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/locale/cy/LC_MESSAGES/django.mo` & `money-to-prisoners-common-9.9.0/mtp_common/locale/cy/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-10-16 15:21+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Igor U <igor.ushkarev@digital.justice.gov.uk>, 2017\n"
 "Language-Team: Welsh (https://www.transifex.com/ministry-of-justice/"
 "teams/34553/cy/)\n"
 "Language: cy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
```

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/locale/cy/LC_MESSAGES/djangojs.po` & `money-to-prisoners-common-9.9.0/mtp_common/locale/cy/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/locale/cy/LC_MESSAGES/django.po` & `money-to-prisoners-common-9.9.0/mtp_common/locale/cy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/locale/cy/LC_MESSAGES/djangojs.mo` & `money-to-prisoners-common-9.9.0/mtp_common/locale/cy/LC_MESSAGES/djangojs.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-08-10 12:27+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Welsh Language Unit <welsh.language.unit.manager@hmcts.gsi."
 "gov.uk>, 2017\n"
 "Language-Team: Welsh (https://www.transifex.com/ministry-of-justice/"
 "teams/34553/cy/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
```

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/tasks.py` & `money-to-prisoners-common-9.9.0/mtp_common/tasks.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/forms/fields.py` & `money-to-prisoners-common-9.9.0/mtp_common/forms/fields.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/forms/__init__.py` & `money-to-prisoners-common-9.9.0/mtp_common/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/screenshots.py` & `money-to-prisoners-common-9.9.0/mtp_common/screenshots.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/auth/csrf.py` & `money-to-prisoners-common-9.9.0/mtp_common/auth/csrf.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/auth/models.py` & `money-to-prisoners-common-9.9.0/mtp_common/auth/models.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/auth/__init__.py` & `money-to-prisoners-common-9.9.0/mtp_common/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/auth/forms.py` & `money-to-prisoners-common-9.9.0/mtp_common/auth/forms.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/auth/backends.py` & `money-to-prisoners-common-9.9.0/mtp_common/auth/backends.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/auth/api_client.py` & `money-to-prisoners-common-9.9.0/mtp_common/auth/api_client.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/auth/middleware.py` & `money-to-prisoners-common-9.9.0/mtp_common/auth/middleware.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/auth/views.py` & `money-to-prisoners-common-9.9.0/mtp_common/auth/views.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/test_utils/code_style.py` & `money-to-prisoners-common-9.9.0/mtp_common/test_utils/code_style.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/test_utils/runner.py` & `money-to-prisoners-common-9.9.0/mtp_common/test_utils/runner.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/test_utils/functional_tests.py` & `money-to-prisoners-common-9.9.0/mtp_common/test_utils/functional_tests.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/test_utils/webdrivers.py` & `money-to-prisoners-common-9.9.0/mtp_common/test_utils/webdrivers.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/management/commands/makemessages.py` & `money-to-prisoners-common-9.9.0/mtp_common/management/commands/makemessages.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/management/commands/functionaltest.py` & `money-to-prisoners-common-9.9.0/mtp_common/management/commands/functionaltest.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/management/commands/compilemessages.py` & `money-to-prisoners-common-9.9.0/mtp_common/management/commands/compilemessages.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/feedback/views.py` & `money-to-prisoners-common-9.9.0/mtp_common/feedback/views.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/api.py` & `money-to-prisoners-common-9.9.0/mtp_common/api.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/context_processors.py` & `money-to-prisoners-common-9.9.0/mtp_common/context_processors.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/nomis.py` & `money-to-prisoners-common-9.9.0/mtp_common/nomis.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/year-field-completion.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/year-field-completion.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/disclosure.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/disclosure.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/placeholder-polyfill.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/placeholder-polyfill.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/select-all.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/select-all.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/unload.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/unload.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/date-picker.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/date-picker.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/tabbed-panel.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/tabbed-panel.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/polyfills.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/polyfills.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/dialogue-box.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/dialogue-box.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/upload.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/upload.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/mailcheck-warning.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/mailcheck-warning.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/footer-feedback.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/footer-feedback.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/character-count-warning.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/character-count-warning.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/analytics.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/analytics.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -13,14 +13,19 @@
     init: function() {
         if (this._gaExists()) {
             $('*[data-' + this.attrName + ']').on('click', $.proxy(this._sendFromEvent, this));
         }
     },
 
     send: function() {
+        /*
+          Sends to GA passing through all specified arguments.
+          It appends an object with page, location and title to the call, if you don't want
+          this use rawSend instead.
+        */
         if (this._gaExists()) {
             var ga_data = $('span.mtp-ga-data');
             if (ga_data) {
                 var ga_override = {
                     page: ga_data.data('page'),
                     location: ga_data.data('location'),
                     title: ga_data.data('title') || document.title,
@@ -28,14 +33,25 @@
                 [].push.call(arguments, ga_override);
             }
             [].unshift.call(arguments, 'send');
             ga.apply(window, arguments);
         }
     },
 
+    rawSend: function() {
+        /*
+          Sends to GA passing through all specified arguments.
+          Unlike send, it does NOT modify any arguments.
+        */
+        if (this._gaExists()) {
+            [].unshift.call(arguments, 'send');
+            ga.apply(window, arguments);
+        }
+    },
+
     _sendFromEvent: function(event) {
         var analyticsParams = $(event.currentTarget).data(this.attrName).split(',');
         this.send.apply(this, analyticsParams);
         return true;
     },
 
     _gaExists: function() {
```

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/notifications.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/notifications.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/autocomplete-select.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/autocomplete-select.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/javascripts/modules/print.js` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/javascripts/modules/print.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/internal/_notifications.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/internal/_notifications.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/internal/_proposition-extra.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/internal/_proposition-extra.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/internal/_settings.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/internal/_settings.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/internal/_overrides.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/internal/_overrides.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_checkbox.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_checkbox.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_sub-nav.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_sub-nav.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_tabbed-panel.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_tabbed-panel.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_important.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_important.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_large-link.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_large-link.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_date-picker.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_date-picker.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_table.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_table.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_forms.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_forms.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_footer-feedback.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_footer-feedback.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_disclosure.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_disclosure.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_pagination.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_pagination.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_dialogue-box.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_dialogue-box.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_delete-icons.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_delete-icons.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_account-management.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_account-management.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/elements/_messages.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/elements/_messages.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/_mtp.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/_mtp.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/assets-src/stylesheets/_base.scss` & `money-to-prisoners-common-9.9.0/mtp_common/assets-src/stylesheets/_base.scss`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/page-list@2x.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/page-list@2x.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/govuk-header-logo.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/govuk-header-logo.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/arrow-sprite.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/arrow-sprite.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/notification-control@2x.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/notification-control@2x.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/proposition-user-icon.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/proposition-user-icon.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/delete-icon@2x.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/delete-icon@2x.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/message-error@2x.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/message-error@2x.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/proposition-user-icon-focused.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/proposition-user-icon-focused.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/message-warning@2x.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/message-warning@2x.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/pagination-sprite@2x.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/pagination-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/message-success@2x.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/message-success@2x.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/arrow-sprite@2x.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/arrow-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/crest-moj.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/crest-moj.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/firefox.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/firefox.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/proposition-user-icon@2x.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/proposition-user-icon@2x.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/proposition-user-icon-focused@2x.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/proposition-user-icon-focused@2x.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/govuk-header-logo-email.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/govuk-header-logo-email.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/notification-control.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/notification-control.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/message-warning.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/message-warning.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/crest-moj@2x.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/crest-moj@2x.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/message-info@2x.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/message-info@2x.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/images/important@2x.png` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/images/important@2x.png`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/javascripts/webfont-debug.js` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/javascripts/webfont-debug.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/a11y/axs_testing.js` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/a11y/axs_testing.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/mtp_common/a11y/HTMLCS.js` & `money-to-prisoners-common-9.9.0/mtp_common/static/mtp_common/a11y/HTMLCS.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/static/stylesheets/fonts-ie8.css` & `money-to-prisoners-common-9.9.0/mtp_common/static/stylesheets/fonts-ie8.css`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/stack.py` & `money-to-prisoners-common-9.9.0/mtp_common/stack.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/build_tasks/tasks.py` & `money-to-prisoners-common-9.9.0/mtp_common/build_tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/build_tasks/paths.py` & `money-to-prisoners-common-9.9.0/mtp_common/build_tasks/paths.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/build_tasks/app.py` & `money-to-prisoners-common-9.9.0/mtp_common/build_tasks/app.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/build_tasks/executor.py` & `money-to-prisoners-common-9.9.0/mtp_common/build_tasks/executor.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/update.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/update.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/undelete.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/undelete.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/list.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/list.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/sign-up.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/sign-up.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/user-description.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/user-description.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/saved.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/saved.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/sign-up-success.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/sign-up-success.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/accept-request.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/accept-request.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/delete.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/delete.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/sign-up-confirm-changes.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/sign-up-confirm-changes.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/sign-up-has-other-roles.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/sign-up-has-other-roles.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/user_admin/incompatible-user.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/user_admin/incompatible-user.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/checkbox-field.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/checkbox-field.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/textarea.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/textarea.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/radio-field.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/radio-field.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/error-summary.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/error-summary.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/date-picker-field.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/date-picker-field.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/generic.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/generic.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/field.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/field.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/forms/select-field.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/forms/select-field.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/auth/email-change-email.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/auth/email-change-email.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/auth/login.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/auth/login.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/auth/reset-password-done.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/auth/reset-password-done.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/auth/password_change_done.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/auth/password_change_done.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/sub-nav.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/sub-nav.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/mtp_base.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/mtp_base.html`

 * *Files 10% similar despite different names*

```diff
@@ -20,28 +20,26 @@
   {% if GOOGLE_ANALYTICS_ID %}
     <script>
       (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
       (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
       m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
       })(window,document,'script','https://www.google-analytics.com/analytics.js','ga');
       ga('create', '{{ GOOGLE_ANALYTICS_ID }}', 'auto');
-      {% if google_analytics_pageview %}
-        ga('send', 'pageview', '{{ google_analytics_pageview.page }}', {
-          'page': '{{ google_analytics_pageview.page }}',
-          'location': '{{ google_analytics_pageview.location }}',
-          'title': '{{ google_analytics_pageview.title }}'
-        });
-      {% elif default_google_analytics_pageview %}
-        ga('send', 'pageview', '{{ default_google_analytics_pageview.page }}', {
-          'page': '{{ default_google_analytics_pageview.page }}',
-          'location': '{{ default_google_analytics_pageview.location }}'
-        });
-      {% else %}
-        ga('send', 'pageview');
-      {% endif %}
+
+      {% with default_ga_data=default_google_analytics_pageview %}
+      {% with ga_data=google_analytics_pageview|default:default_ga_data %}
+        {% spaceless %}
+          {% for key, value in ga_data.items %}
+            {% if value %}ga('set', '{{ key }}', '{{ value }}');{% endif %}
+          {% endfor %}
+        {% endspaceless %}
+
+      ga('send', 'pageview');
+      {% endwith %}
+      {% endwith %}
     </script>
   {% endif %}
 {% endblock %}
 
 {% block body_classes %}{{ block.super }} {% if moj_internal_site %}mtp-internal-site{% endif %} {% if footer_feedback_context %}without-footer-padding{% endif %}{% endblock %}
 
 {% block cookie_message %}
```

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/tabbed-panel.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/tabbed-panel.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/notifications.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/notifications.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/page-list.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/page-list.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/footer-feedback.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/footer-feedback.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/proposition-user-menu.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/proposition-user-menu.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/language-switch.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/language-switch.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/includes/dialogue-box.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/includes/dialogue-box.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/maintenance-citizen.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/maintenance-citizen.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/feedback/submit_feedback.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/feedback/submit_feedback.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/feedback/success.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/feedback/success.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/build_tasks/eslintrc.json` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/build_tasks/eslintrc.json`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/build_tasks/webpack.config.js` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/build_tasks/webpack.config.js`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/build_tasks/package.json` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/build_tasks/package.json`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/errors/500.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/errors/500.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/errors/404.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/errors/404.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/errors/400.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/errors/400.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/settings.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/settings.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/a11y.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/a11y.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/maintenance.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/maintenance.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/mtp_common/email_base.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/mtp_common/email_base.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/templates/govuk_template/base.html` & `money-to-prisoners-common-9.9.0/mtp_common/templates/govuk_template/base.html`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/dates.py` & `money-to-prisoners-common-9.9.0/mtp_common/dates.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/views.py` & `money-to-prisoners-common-9.9.0/mtp_common/views.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/mtp_common/spooling.py` & `money-to-prisoners-common-9.9.0/mtp_common/spooling.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/MANIFEST.in` & `money-to-prisoners-common-9.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/setup.py` & `money-to-prisoners-common-9.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `money-to-prisoners-common-9.8.1/README.rst` & `money-to-prisoners-common-9.9.0/README.rst`

 * *Files identical despite different names*

