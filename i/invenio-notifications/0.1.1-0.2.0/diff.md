# Comparing `tmp/invenio-notifications-0.1.1.tar.gz` & `tmp/invenio-notifications-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-notifications-0.1.1.tar", last modified: Fri May  5 11:31:57 2023, max compression
+gzip compressed data, was "dist/invenio-notifications-0.2.0.tar", last modified: Tue Jun  6 09:31:43 2023, max compression
```

## Comparing `invenio-notifications-0.1.1.tar` & `invenio-notifications-0.2.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/backends/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/backends/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/backends/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/backends/utils/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/services/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/services/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/services/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/services/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/services/uow.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.accepted.html
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.accepted.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.created.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.created.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.declined.html
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.declined.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.created.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.created.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.deleted.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.deleted.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.submitted.html
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.submitted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/translations/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/translations/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-05 11:31:56.000000 invenio-notifications-0.1.1/invenio_notifications/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/tests/test_invenio_notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/backends/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications/backends/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/backends/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/backends/utils/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/services/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/services/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/services/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/services/uow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/invenio_notifications/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.accepted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.accepted.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.created.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.created.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.declined.html
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.declined.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.created.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.created.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.deleted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.deleted.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.submitted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.submitted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/translations/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/invenio_notifications/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/invenio_notifications.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:31:43.000000 invenio-notifications-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-06 09:31:32.000000 invenio-notifications-0.2.0/tests/test_invenio_notifications.py
```

### Comparing `invenio-notifications-0.1.1/.editorconfig` & `invenio-notifications-0.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/.github/workflows/pypi-publish.yml` & `invenio-notifications-0.2.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/.github/workflows/tests.yml` & `invenio-notifications-0.2.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/.tx/config` & `invenio-notifications-0.2.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/CONTRIBUTING.rst` & `invenio-notifications-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/MANIFEST.in` & `invenio-notifications-0.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/PKG-INFO` & `invenio-notifications-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-notifications
-Version: 0.1.1
+Version: 0.2.0
 Summary: "Invenio module for notifications support."
 Home-page: https://github.com/inveniosoftware/invenio-notifications
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2023 CERN.
@@ -40,14 +40,19 @@
             Invenio-Notifications is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 0.2.0 (released 2023-06-06)
+        
+        - views: register notification settings menu
+        - backends: render template fully once to establish context
+        
         Version 0.1.1 (released 2023-05-05)
         
         - remove type hints
         
         Version 0.1.0 (released 2023-05-04)
         
         - Initial public release.
```

### Comparing `invenio-notifications-0.1.1/README.rst` & `invenio-notifications-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/babel.ini` & `invenio-notifications-0.2.0/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/docs/Makefile` & `invenio-notifications-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/docs/conf.py` & `invenio-notifications-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/docs/index.rst` & `invenio-notifications-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/docs/make.bat` & `invenio-notifications-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/invenio_notifications/__init__.py` & `invenio-notifications-0.2.0/invenio_notifications/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # details.
 
 """Invenio module for notifications support."""
 
 from .ext import InvenioNotifications
 from .proxies import current_notifications, current_notifications_manager
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 __all__ = (
     "__version__",
     "current_notifications",
     "current_notifications_manager",
     "InvenioNotifications",
 )
```

### Comparing `invenio-notifications-0.1.1/invenio_notifications/backends/base.py` & `invenio-notifications-0.2.0/invenio_notifications/backends/base.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/invenio_notifications/backends/email.py` & `invenio-notifications-0.2.0/invenio_notifications/backends/email.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/invenio_notifications/backends/utils/loaders.py` & `invenio-notifications-0.2.0/invenio_notifications/backends/utils/loaders.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
+# Copyright (C) 2023 CERN.
 # Copyright (C) 2023 Graz University of Technology.
 #
 # Invenio-Notifications is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Template loaders for notification backend."""
 
@@ -35,15 +36,21 @@
                 f"{self.template_folder}/{notification.type}.jinja",
             ]
         )
         ctx = template.new_context(
             {
                 "notification": notification,
                 "recipient": recipient,
-            }
+            },
         )
+
+        # "Force" rendering the whole template (including global variables).
+        # Since we render block by block afterwards, the context and variables
+        # would be lost between blocks.
+        list(template.root_render_func(ctx))
+
         return {
             block: "".join(
                 block_func(ctx)
             )  # have to evaluate, as block_func is a generator
             for block, block_func in template.blocks.items()
         }
```

### Comparing `invenio-notifications-0.1.1/invenio_notifications/config.py` & `invenio-notifications-0.2.0/invenio_notifications/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,7 +46,14 @@
         UserResultItemResolver(),
         RDMRecordResultItemResolver(),
         CommunityResultItemResolver(),
         RequestResultItemResolver(),
         RequestEventResultItemResolver(),
     ]
 """
+
+NOTIFICATIONS_SETTINGS_VIEW_FUNCTION = None
+"""View function for notification settings.
+
+This should be set higher up in the module hierarchy (e.g. invenio-app-rdm), as
+this module does not have knowledge of the settings view.
+"""
```

### Comparing `invenio-notifications-0.1.1/invenio_notifications/errors.py` & `invenio-notifications-0.2.0/invenio_notifications/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/invenio_notifications/ext.py` & `invenio-notifications-0.2.0/invenio_notifications/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/invenio_notifications/manager.py` & `invenio-notifications-0.2.0/invenio_notifications/manager.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/invenio_notifications/models.py` & `invenio-notifications-0.2.0/invenio_notifications/models.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/invenio_notifications/proxies.py` & `invenio-notifications-0.2.0/invenio_notifications/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/invenio_notifications/registry.py` & `invenio-notifications-0.2.0/invenio_notifications/registry.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/invenio_notifications/services/builders.py` & `invenio-notifications-0.2.0/invenio_notifications/services/builders.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/invenio_notifications/services/filters.py` & `invenio-notifications-0.2.0/invenio_notifications/services/filters.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/invenio_notifications/services/generators.py` & `invenio-notifications-0.2.0/invenio_notifications/services/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/invenio_notifications/services/uow.py` & `invenio-notifications-0.2.0/invenio_notifications/services/uow.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/invenio_notifications/tasks.py` & `invenio-notifications-0.2.0/invenio_notifications/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/invenio_notifications.egg-info/PKG-INFO` & `invenio-notifications-0.2.0/invenio_notifications.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-notifications
-Version: 0.1.1
+Version: 0.2.0
 Summary: "Invenio module for notifications support."
 Home-page: https://github.com/inveniosoftware/invenio-notifications
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2023 CERN.
@@ -40,14 +40,19 @@
             Invenio-Notifications is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 0.2.0 (released 2023-06-06)
+        
+        - views: register notification settings menu
+        - backends: render template fully once to establish context
+        
         Version 0.1.1 (released 2023-05-05)
         
         - remove type hints
         
         Version 0.1.0 (released 2023-05-04)
         
         - Initial public release.
```

### Comparing `invenio-notifications-0.1.1/invenio_notifications.egg-info/SOURCES.txt` & `invenio-notifications-0.2.0/invenio_notifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/run-tests.sh` & `invenio-notifications-0.2.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/setup.cfg` & `invenio-notifications-0.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 	invenio-search[opensearch2]>=2.1.0,<3.0.0
 
 [options.entry_points]
 invenio_base.apps = 
 	invenio_notifications = invenio_notifications:InvenioNotifications
 invenio_base.api_apps = 
 	invenio_notifications = invenio_notifications:InvenioNotifications
+invenio_base.blueprints = 
+	invenio_notifications_settings = invenio_notifications.views:create_blueprint_settings
 invenio_base.api_blueprints = 
 	invenio_notifications = invenio_notifications.views:create_blueprint
 invenio_celery.tasks = 
 	invenio_notifications = invenio_notifications.tasks
 invenio_i18n.translations = 
 	messages = invenio_notifications
```

### Comparing `invenio-notifications-0.1.1/tests/conftest.py` & `invenio-notifications-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.1/tests/test_invenio_notifications.py` & `invenio-notifications-0.2.0/tests/test_invenio_notifications.py`

 * *Files identical despite different names*

