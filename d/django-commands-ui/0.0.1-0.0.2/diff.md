# Comparing `tmp/django-commands-ui-0.0.1.tar.gz` & `tmp/django-commands-ui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-commands-ui-0.0.1.tar", last modified: Thu Mar 30 09:28:25 2023, max compression
+gzip compressed data, was "django-commands-ui-0.0.2.tar", last modified: Tue Jun  6 13:28:46 2023, max compression
```

## Comparing `django-commands-ui-0.0.1.tar` & `django-commands-ui-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:28:25.892139 django-commands-ui-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-03-30 09:28:25.892139 django-commands-ui-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:28:25.892139 django-commands-ui-0.0.1/commands_ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15629 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/management_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:28:25.892139 django-commands-ui-0.0.1/commands_ui/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:28:25.892139 django-commands-ui-0.0.1/commands_ui/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:28:25.892139 django-commands-ui-0.0.1/commands_ui/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/templates/jobs/job-detail-history.html
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/templates/jobs/job-detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/templates/jobs/job-list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/templates/jobs/job-status.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:28:25.892139 django-commands-ui-0.0.1/commands_ui/templates/jobs/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/templates/jobs/partials/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/templates/jobs/partials/job-output.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:28:25.892139 django-commands-ui-0.0.1/commands_ui/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/templatetags/tags_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/use_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/commands_ui/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:28:25.892139 django-commands-ui-0.0.1/django_commands_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-03-30 09:28:25.000000 django-commands-ui-0.0.1/django_commands_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-30 09:28:25.000000 django-commands-ui-0.0.1/django_commands_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 09:28:25.000000 django-commands-ui-0.0.1/django_commands_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-30 09:28:25.000000 django-commands-ui-0.0.1/django_commands_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-30 09:28:25.000000 django-commands-ui-0.0.1/django_commands_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-30 09:28:13.000000 django-commands-ui-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 09:28:25.892139 django-commands-ui-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:28:46.464435 django-commands-ui-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-06 13:28:46.464435 django-commands-ui-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:28:46.460435 django-commands-ui-0.0.2/commands_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/management_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:28:46.460435 django-commands-ui-0.0.2/commands_ui/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:28:46.460435 django-commands-ui-0.0.2/commands_ui/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:28:46.464435 django-commands-ui-0.0.2/commands_ui/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/templates/jobs/job-detail-history.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/templates/jobs/job-detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/templates/jobs/job-list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/templates/jobs/job-status.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:28:46.464435 django-commands-ui-0.0.2/commands_ui/templates/jobs/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/templates/jobs/partials/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/templates/jobs/partials/job-output.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:28:46.464435 django-commands-ui-0.0.2/commands_ui/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/templatetags/tags_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/use_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/commands_ui/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:28:46.464435 django-commands-ui-0.0.2/django_commands_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-06 13:28:46.000000 django-commands-ui-0.0.2/django_commands_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-06 13:28:46.000000 django-commands-ui-0.0.2/django_commands_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:28:46.000000 django-commands-ui-0.0.2/django_commands_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-06 13:28:46.000000 django-commands-ui-0.0.2/django_commands_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 13:28:46.000000 django-commands-ui-0.0.2/django_commands_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-06 13:28:37.000000 django-commands-ui-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:28:46.464435 django-commands-ui-0.0.2/setup.cfg
```

### Comparing `django-commands-ui-0.0.1/LICENSE` & `django-commands-ui-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/PKG-INFO` & `django-commands-ui-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,52 @@
-Metadata-Version: 2.1
-Name: django-commands-ui
-Version: 0.0.1
-Summary: Plugin interface to list and execute existing management commands.
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-        # Django Commands UI
+# Django Commands UI
 
 This project offers a solution to list and execute all existing management commands in your Django project.
 
+## Requirements
+
+This project requires Python 3.10 or greater.
+
 ## Configuration
 
 To install and configure it these steps should be followed:
 1. Install the dependency from PyPi.
    ```
    pip install django-commands-ui
    ```
 2. Add `commands_ui` as an installed app in your Django project.
-3. Add these needed settings:
+3. If you haven't already done so, you will need to add celery to your django project. You can follow the steps in the [First steps with Django](https://docs.celeryq.dev/en/stable/django/first-steps-with-django.html) guide if you haven't used celery before.
+4. Add the root location of your management commands to your installed apps. For example, if your management commands are in the `commands` folder in your project root, you would add `your-project-name.commands` to your installed apps.
+5. Add these required settings:
    ```
-    # Celery app name
+    # Celery app name.
     COMMANDS_UI_CELERY_APP = ""
 
     # Working celery queue name for delayed jobs.
     COMMANDS_UI_DELAYED_JOBS_QUEUE = ""
 
     # Working celery queue name for standard jobs.
     COMMANDS_UI_JOBS_QUEUE = ""
 
-    # List of apps from we want to extract the runnable commands.
-    COMMANDS_UI_JOB_APPS = ""
+    # Tuple of compiled regexes to extract the runnable commands from.
+    # By default, all commands from all installed apps are extracted.
+    COMMANDS_UI_JOB_APPS = (re.compile(r".*"),)
 
     # Primary database identifyer, not the replica one.
     DATABASE_PRIMARY = getattr(settings, "DATABASE_PRIMARY", "default")
 
     # Define if the current environment is a cron environment.
     CRON_ENVIRONMENT = getattr(settings, "CRON_ENVIRONMENT", False)
    ```
-4. Include package URLs to your base urls file like this:
+6. Include package URLs to your base urls file like this:
    ```
    path("jobs/", include("commands_ui.urls")),
    ```
 
-5. Create tables:
+7. Create tables:
    ```
    python manage.py migrate commands_ui
    ```
 
 It is recommended to override `base.html` so the appearance is customizable, as all `django-commands-ui` templates extend from it.
 
 ## Documentation
@@ -57,20 +55,38 @@
 
 The only needed thing for implementing a working management command job in
 `django-commands-ui` is extending the existing JobBasedCommand.
 This class adds some default arguments (such as `--job-id`).
 
 Example on how to use this class:
 ```
+from typing import Any
 from commands_ui import management_commands
 from django.core.management.base import CommandParser
 
 # Extend the JobBasedCommand class
 class Command(management_commands.JobBasedCommand):
    def handle(self, *args: Any, **options: Any) -> None:
       # Any time `self.print` is used, the message will be added to both standard output and
       # Job output.
       self.print("Starting")
       for i in range(0, 20):
          self.print(i)
       self.print("Finishing")
 ```
+
+### Command Grouping
+
+You can group types of commands by adding a `interface_name` class attribute to your management command class. This will group all commands with the same `interface_name` together in the UI.
+For example you can group cronjobs together by adding `interface_name = "cron"` to all your cronjobs.
+
+```
+from typing import Any
+from commands_ui import management_commands
+from django.core.management.base import CommandParser
+
+# Extend the JobBasedCommand class
+class Command(management_commands.JobBasedCommand):
+    interface_name = "cron"
+   def handle(self, *args: Any, **options: Any) -> None:
+      ...
+```
```

### Comparing `django-commands-ui-0.0.1/commands_ui/app_settings.py` & `django-commands-ui-0.0.2/commands_ui/app_settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,29 @@
+import re
+
 from django.conf import settings
 from django.utils.module_loading import import_string
 
 USER_MODEL = getattr(settings, "COMMANDS_UI_USER_MODEL", settings.AUTH_USER_MODEL)
 
 CELERY_APP = getattr(settings, "COMMANDS_UI_CELERY_APP")
 
 # Database identifiers
 DATABASE_PRIMARY = getattr(settings, "DATABASE_PRIMARY", "default")
 
 # Define if this is a cron environment
 CRON_ENVIRONMENT = getattr(settings, "CRON_ENVIRONMENT", False)
 
-# List of apps from we want to extract the runnable commands
+# Tuple of compiled regexes to extract the runnable commands from.
+# If empty, all commands from installed packages are found.
 COMMANDS_UI_JOB_APPS = getattr(settings, "COMMANDS_UI_JOB_APPS", "")
 
+if not COMMANDS_UI_JOB_APPS:
+    COMMANDS_UI_JOB_APPS = (re.compile(r".*"),)
+
 # Working celery queue name for standard jobs
 COMMANDS_UI_JOBS_QUEUE = getattr(settings, "COMMANDS_UI_JOBS_QUEUE", "")
 
 # Media path
 MEDIA_URL = getattr(settings, "MEDIA_URL", "")
 MEDIA_ROOT = getattr(settings, "MEDIA_ROOT", "")
```

### Comparing `django-commands-ui-0.0.1/commands_ui/domain.py` & `django-commands-ui-0.0.2/commands_ui/domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                     continue
                 if _user_can_view_job(job, user):
                     display_name = getattr(job, "verbose_name", _clean_name(name))
                     command_list.append(
                         {
                             "display_name": display_name,
                             "name": name,
-                            "interface": getattr(job, "interface_name", "unknown"),
+                            "interface": getattr(job, "interface_name", ""),
                         }
                     )
             app_configs.append(
                 {
                     "path": app_config.name,
                     "name": app_config.verbose_name,
                     "command_list": command_list,
```

### Comparing `django-commands-ui-0.0.1/commands_ui/forms.py` & `django-commands-ui-0.0.2/commands_ui/forms.py`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/commands_ui/management_commands.py` & `django-commands-ui-0.0.2/commands_ui/management_commands.py`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/commands_ui/migrations/0001_initial.py` & `django-commands-ui-0.0.2/commands_ui/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/commands_ui/models.py` & `django-commands-ui-0.0.2/commands_ui/models.py`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/commands_ui/patch.py` & `django-commands-ui-0.0.2/commands_ui/patch.py`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/commands_ui/tasks.py` & `django-commands-ui-0.0.2/commands_ui/tasks.py`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/commands_ui/templates/jobs/job-detail-history.html` & `django-commands-ui-0.0.2/commands_ui/templates/jobs/job-detail-history.html`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/commands_ui/templates/jobs/job-detail.html` & `django-commands-ui-0.0.2/commands_ui/templates/jobs/job-detail.html`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/commands_ui/templates/jobs/job-list.html` & `django-commands-ui-0.0.2/commands_ui/templates/jobs/job-list.html`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/commands_ui/templates/jobs/job-status.html` & `django-commands-ui-0.0.2/commands_ui/templates/jobs/job-status.html`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/commands_ui/templates/jobs/partials/form.html` & `django-commands-ui-0.0.2/commands_ui/templates/jobs/partials/form.html`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/commands_ui/templates/jobs/partials/job-output.html` & `django-commands-ui-0.0.2/commands_ui/templates/jobs/partials/job-output.html`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/commands_ui/use_cases.py` & `django-commands-ui-0.0.2/commands_ui/use_cases.py`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/commands_ui/views.py` & `django-commands-ui-0.0.2/commands_ui/views.py`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/django_commands_ui.egg-info/PKG-INFO` & `django-commands-ui-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 Metadata-Version: 2.1
 Name: django-commands-ui
-Version: 0.0.1
+Version: 0.0.2
 Summary: Plugin interface to list and execute existing management commands.
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-        # Django Commands UI
+# Django Commands UI
 
 This project offers a solution to list and execute all existing management commands in your Django project.
 
+## Requirements
+
+This project requires Python 3.10 or greater.
+
 ## Configuration
 
 To install and configure it these steps should be followed:
 1. Install the dependency from PyPi.
    ```
    pip install django-commands-ui
    ```
 2. Add `commands_ui` as an installed app in your Django project.
-3. Add these needed settings:
+3. If you haven't already done so, you will need to add celery to your django project. You can follow the steps in the [First steps with Django](https://docs.celeryq.dev/en/stable/django/first-steps-with-django.html) guide if you haven't used celery before.
+4. Add the root location of your management commands to your installed apps. For example, if your management commands are in the `commands` folder in your project root, you would add `your-project-name.commands` to your installed apps.
+5. Add these required settings:
    ```
-    # Celery app name
+    # Celery app name.
     COMMANDS_UI_CELERY_APP = ""
 
     # Working celery queue name for delayed jobs.
     COMMANDS_UI_DELAYED_JOBS_QUEUE = ""
 
     # Working celery queue name for standard jobs.
     COMMANDS_UI_JOBS_QUEUE = ""
 
-    # List of apps from we want to extract the runnable commands.
-    COMMANDS_UI_JOB_APPS = ""
+    # Tuple of compiled regexes to extract the runnable commands from.
+    # By default, all commands from all installed apps are extracted.
+    COMMANDS_UI_JOB_APPS = (re.compile(r".*"),)
 
     # Primary database identifyer, not the replica one.
     DATABASE_PRIMARY = getattr(settings, "DATABASE_PRIMARY", "default")
 
     # Define if the current environment is a cron environment.
     CRON_ENVIRONMENT = getattr(settings, "CRON_ENVIRONMENT", False)
    ```
-4. Include package URLs to your base urls file like this:
+6. Include package URLs to your base urls file like this:
    ```
    path("jobs/", include("commands_ui.urls")),
    ```
 
-5. Create tables:
+7. Create tables:
    ```
    python manage.py migrate commands_ui
    ```
 
 It is recommended to override `base.html` so the appearance is customizable, as all `django-commands-ui` templates extend from it.
 
 ## Documentation
@@ -57,20 +64,38 @@
 
 The only needed thing for implementing a working management command job in
 `django-commands-ui` is extending the existing JobBasedCommand.
 This class adds some default arguments (such as `--job-id`).
 
 Example on how to use this class:
 ```
+from typing import Any
 from commands_ui import management_commands
 from django.core.management.base import CommandParser
 
 # Extend the JobBasedCommand class
 class Command(management_commands.JobBasedCommand):
    def handle(self, *args: Any, **options: Any) -> None:
       # Any time `self.print` is used, the message will be added to both standard output and
       # Job output.
       self.print("Starting")
       for i in range(0, 20):
          self.print(i)
       self.print("Finishing")
 ```
+
+### Command Grouping
+
+You can group types of commands by adding a `interface_name` class attribute to your management command class. This will group all commands with the same `interface_name` together in the UI.
+For example you can group cronjobs together by adding `interface_name = "cron"` to all your cronjobs.
+
+```
+from typing import Any
+from commands_ui import management_commands
+from django.core.management.base import CommandParser
+
+# Extend the JobBasedCommand class
+class Command(management_commands.JobBasedCommand):
+    interface_name = "cron"
+   def handle(self, *args: Any, **options: Any) -> None:
+      ...
+```
```

### Comparing `django-commands-ui-0.0.1/django_commands_ui.egg-info/SOURCES.txt` & `django-commands-ui-0.0.2/django_commands_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-commands-ui-0.0.1/pyproject.toml` & `django-commands-ui-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-commands-ui"
-version = "0.0.1"
+version = "0.0.2"
 description = "Plugin interface to list and execute existing management commands."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 dependencies = [
   "boto3>=1.26.82",
   "celery>=5.2.7",
   "django_extensions>=3.2.1",
   "django-multidb-router>=0.10",
   "djangorestframework>=3.14.0",
   "xocto>=3.0.0",
```

