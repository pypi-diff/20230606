# Comparing `tmp/aimmo-v0.1.1-alpha.post.dev8.tar.gz` & `tmp/aimmo-v0.1.1-alpha.post.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aimmo-v0.1.1-alpha.post.dev8.tar", last modified: Wed Jan 31 13:38:42 2018, max compression
+gzip compressed data, was "dist/aimmo-v0.1.1-alpha.post.dev9.tar", last modified: Wed Jan 31 13:40:22 2018, max compression
```

## Comparing `aimmo-v0.1.1-alpha.post.dev8.tar` & `aimmo-v0.1.1-alpha.post.dev9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7722 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      783 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/players/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/autoconfig.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13141 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/tests.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/players/static/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/players/static/css/
--rw-rw-r--   0 travis    (2000) travis    (2000)       36 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/static/css/program.css
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/static/css/watch.css
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/players/static/js/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3022 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/static/js/program.js
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/players/management/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/management/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/players/management/commands/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3400 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/management/commands/generate_players.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/management/commands/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      442 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/management/commands/delete_generated_players.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1864 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3307 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      488 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/players/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      121 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/admin.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/players/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/players/templates/players/
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/templates/players/statistics.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      428 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/templates/players/home.html
--rwxrwxr-x   0 travis    (2000) travis    (2000)      715 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/templates/players/viewer.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/templates/players/program.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      500 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/templates/players/dropdown.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      323 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/templates/players/add_game.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3499 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/templates/players/base.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1988 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/templates/players/watch.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/players/templates/registration/
--rw-rw-r--   0 travis    (2000) travis    (2000)      652 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/templates/registration/login.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      372 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/app_settings.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/players/templatetags/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/templatetags/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      448 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/templatetags/players_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/forms.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5593 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/views.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/players/avatar_examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1689 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/avatar_examples/health_seeker_avatar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1392 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/avatar_examples/attacking_avatar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       20 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/avatar_examples/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      254 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/avatar_examples/dumb_avatar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/avatar_examples/winner_avatar.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/players/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3175 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/migrations/0003_auto_20160802_1418.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      942 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1933 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/migrations/0005_auto_20160808_1545.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      411 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/migrations/0002_auto_20160601_1914.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      411 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/migrations/0006_game_static_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1557 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/players/migrations/0004_auto_20160808_1511.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/aimmo_runner/
--rw-rw-r--   0 travis    (2000) travis    (2000)      580 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/aimmo_runner/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/aimmo_runner/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2778 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/aimmo_runner/runner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/aimmo_runner/shell_api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4294 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/aimmo_runner/minikube.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      461 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2018-01-31 13:30:32.000000 aimmo-v0.1.1-alpha.post.dev8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      230 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:38:42.000000 aimmo-v0.1.1-alpha.post.dev8/aimmo.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2018-01-31 13:38:41.000000 aimmo-v0.1.1-alpha.post.dev8/aimmo.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-01-31 13:38:41.000000 aimmo-v0.1.1-alpha.post.dev8/aimmo.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      193 2018-01-31 13:38:41.000000 aimmo-v0.1.1-alpha.post.dev8/aimmo.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      226 2018-01-31 13:38:41.000000 aimmo-v0.1.1-alpha.post.dev8/aimmo.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-01-31 13:38:41.000000 aimmo-v0.1.1-alpha.post.dev8/aimmo.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1708 2018-01-31 13:38:41.000000 aimmo-v0.1.1-alpha.post.dev8/aimmo.egg-info/SOURCES.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7722 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      783 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/players/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/autoconfig.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13141 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/tests.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/players/static/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/players/static/css/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       36 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/static/css/program.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/static/css/watch.css
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/players/static/js/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3022 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/static/js/program.js
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/players/management/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/management/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/players/management/commands/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3400 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/management/commands/generate_players.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/management/commands/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      442 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/management/commands/delete_generated_players.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1864 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/urls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3307 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      488 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/players/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      121 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/admin.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/players/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/players/templates/players/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/templates/players/statistics.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      428 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/templates/players/home.html
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      715 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/templates/players/viewer.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1024 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/templates/players/program.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      500 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/templates/players/dropdown.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      323 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/templates/players/add_game.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3499 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/templates/players/base.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1988 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/templates/players/watch.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/players/templates/registration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      652 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/templates/registration/login.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      372 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/app_settings.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/players/templatetags/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/templatetags/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      448 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/templatetags/players_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      228 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/forms.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5593 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/views.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/players/avatar_examples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1689 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/avatar_examples/health_seeker_avatar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1392 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/avatar_examples/attacking_avatar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       20 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/avatar_examples/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      254 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/avatar_examples/dumb_avatar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/avatar_examples/winner_avatar.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/players/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3175 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/migrations/0003_auto_20160802_1418.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      942 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1933 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/migrations/0005_auto_20160808_1545.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      411 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/migrations/0002_auto_20160601_1914.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      411 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/migrations/0006_game_static_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1557 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/players/migrations/0004_auto_20160808_1511.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/aimmo_runner/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      580 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/aimmo_runner/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/aimmo_runner/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2778 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/aimmo_runner/runner.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/aimmo_runner/shell_api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4294 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/aimmo_runner/minikube.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      461 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2018-01-31 13:31:38.000000 aimmo-v0.1.1-alpha.post.dev9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      230 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-01-31 13:40:22.000000 aimmo-v0.1.1-alpha.post.dev9/aimmo.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2018-01-31 13:40:21.000000 aimmo-v0.1.1-alpha.post.dev9/aimmo.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-01-31 13:40:21.000000 aimmo-v0.1.1-alpha.post.dev9/aimmo.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      193 2018-01-31 13:40:21.000000 aimmo-v0.1.1-alpha.post.dev9/aimmo.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      226 2018-01-31 13:40:21.000000 aimmo-v0.1.1-alpha.post.dev9/aimmo.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-01-31 13:40:21.000000 aimmo-v0.1.1-alpha.post.dev9/aimmo.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1708 2018-01-31 13:40:21.000000 aimmo-v0.1.1-alpha.post.dev9/aimmo.egg-info/SOURCES.txt
```

### Comparing `aimmo-v0.1.1-alpha.post.dev8/README.md` & `aimmo-v0.1.1-alpha.post.dev9/README.md`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/setup.py` & `aimmo-v0.1.1-alpha.post.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/autoconfig.py` & `aimmo-v0.1.1-alpha.post.dev9/players/autoconfig.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/tests.py` & `aimmo-v0.1.1-alpha.post.dev9/players/tests.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/static/js/program.js` & `aimmo-v0.1.1-alpha.post.dev9/players/static/js/program.js`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/management/commands/generate_players.py` & `aimmo-v0.1.1-alpha.post.dev9/players/management/commands/generate_players.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/urls.py` & `aimmo-v0.1.1-alpha.post.dev9/players/urls.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/models.py` & `aimmo-v0.1.1-alpha.post.dev9/players/models.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/templates/players/viewer.html` & `aimmo-v0.1.1-alpha.post.dev9/players/templates/players/viewer.html`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/templates/players/program.html` & `aimmo-v0.1.1-alpha.post.dev9/players/templates/players/program.html`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/templates/players/base.html` & `aimmo-v0.1.1-alpha.post.dev9/players/templates/players/base.html`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/templates/players/watch.html` & `aimmo-v0.1.1-alpha.post.dev9/players/templates/players/watch.html`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/templates/registration/login.html` & `aimmo-v0.1.1-alpha.post.dev9/players/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/views.py` & `aimmo-v0.1.1-alpha.post.dev9/players/views.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/avatar_examples/health_seeker_avatar.py` & `aimmo-v0.1.1-alpha.post.dev9/players/avatar_examples/health_seeker_avatar.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/avatar_examples/attacking_avatar.py` & `aimmo-v0.1.1-alpha.post.dev9/players/avatar_examples/attacking_avatar.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/avatar_examples/winner_avatar.py` & `aimmo-v0.1.1-alpha.post.dev9/players/avatar_examples/winner_avatar.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/migrations/0003_auto_20160802_1418.py` & `aimmo-v0.1.1-alpha.post.dev9/players/migrations/0003_auto_20160802_1418.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/migrations/0001_initial.py` & `aimmo-v0.1.1-alpha.post.dev9/players/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/migrations/0005_auto_20160808_1545.py` & `aimmo-v0.1.1-alpha.post.dev9/players/migrations/0005_auto_20160808_1545.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/players/migrations/0004_auto_20160808_1511.py` & `aimmo-v0.1.1-alpha.post.dev9/players/migrations/0004_auto_20160808_1511.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/aimmo_runner/setup.py` & `aimmo-v0.1.1-alpha.post.dev9/aimmo_runner/setup.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/aimmo_runner/runner.py` & `aimmo-v0.1.1-alpha.post.dev9/aimmo_runner/runner.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/aimmo_runner/shell_api.py` & `aimmo-v0.1.1-alpha.post.dev9/aimmo_runner/shell_api.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/aimmo_runner/minikube.py` & `aimmo-v0.1.1-alpha.post.dev9/aimmo_runner/minikube.py`

 * *Files identical despite different names*

### Comparing `aimmo-v0.1.1-alpha.post.dev8/aimmo.egg-info/SOURCES.txt` & `aimmo-v0.1.1-alpha.post.dev9/aimmo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

