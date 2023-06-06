# Comparing `tmp/drops-0.3.8.tar.gz` & `tmp/drops-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drops-0.3.8.tar", last modified: Thu Feb 16 14:25:35 2023, max compression
+gzip compressed data, was "drops-0.3.9.tar", last modified: Mon Mar  6 14:12:05 2023, max compression
```

## Comparing `drops-0.3.8.tar` & `drops-0.3.9.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.430108 drops-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-16 14:25:20.000000 drops-0.3.8/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-02-16 14:25:20.000000 drops-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    49809 2023-02-16 14:25:35.430108 drops-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-02-16 14:25:20.000000 drops-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-02-16 14:25:20.000000 drops-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 14:25:35.430108 drops-0.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.410108 drops-0.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.414108 drops-0.3.8/src/drops/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.418108 drops-0.3.8/src/drops/console/
--rwxr-xr-x   0 runner    (1001) docker     (123)      707 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.426108 drops-0.3.8/src/drops/console/internal/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1872 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2342 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/backup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1499 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/clean_up.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5209 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1058 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/deploy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1498 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/deploy_https_key.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/echo_paths.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2851 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/er.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/exec.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      716 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/globals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3123 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/host.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1452 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/init.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/init_remove_env_debian.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14904 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/internal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/kill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1264 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/logs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1614 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/new.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1134 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/nginx_force_reload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1060 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/nginx_reload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1344 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/project.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      981 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/ps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/pull.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1138 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/redeploy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1096 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/restart.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1353 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/rm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/ssh.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1086 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/start.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1081 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/stop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1422 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1552 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/undeploy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1084 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/internal/up.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1827 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/console/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.426108 drops-0.3.8/src/drops/docker_ops/
--rwxr-xr-x   0 runner    (1001) docker     (123)       35 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     2957 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/docker-compose.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)        7 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/drops.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.426108 drops-0.3.8/src/drops/docker_ops/release/
--rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/release/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.426108 drops-0.3.8/src/drops/docker_ops/release/html/
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/release/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.426108 drops-0.3.8/src/drops/docker_ops/secrets/
--rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/secrets/README.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.426108 drops-0.3.8/src/drops/docker_ops/secrets/home_ssh/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/secrets/home_ssh/id_ed25519
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/secrets/home_ssh/known_hosts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.426108 drops-0.3.8/src/drops/docker_ops/servers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      205 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.426108 drops-0.3.8/src/drops/docker_ops/servers/acme.sh/
--rwxr-xr-x   0 runner    (1001) docker     (123)      485 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/acme.sh/redeploy-ssl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.426108 drops-0.3.8/src/drops/docker_ops/servers/drops/
--rwxr-xr-x   0 runner    (1001) docker     (123)      262 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/drops/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.426108 drops-0.3.8/src/drops/docker_ops/servers/drops/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/drops/bin/.keep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.414108 drops-0.3.8/src/drops/docker_ops/servers/drops/cron/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.426108 drops-0.3.8/src/drops/docker_ops/servers/drops/cron/daily/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/drops/cron/daily/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.426108 drops-0.3.8/src/drops/docker_ops/servers/drops/cron/hourly/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/drops/cron/hourly/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.430108 drops-0.3.8/src/drops/docker_ops/servers/drops/cron/monthly/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/drops/cron/monthly/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.430108 drops-0.3.8/src/drops/docker_ops/servers/drops/cron/weekly/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/drops/cron/weekly/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.430108 drops-0.3.8/src/drops/docker_ops/servers/drops/cron_example/
--rwxr-xr-x   0 runner    (1001) docker     (123)      265 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/drops/cron_example/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/drops/cron_example/backup.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      463 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/drops/cron_example/drops-backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.430108 drops-0.3.8/src/drops/docker_ops/servers/drops/drops/
--rwxr-xr-x   0 runner    (1001) docker     (123)      139 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/drops/drops/README.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.430108 drops-0.3.8/src/drops/docker_ops/servers/nginx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.430108 drops-0.3.8/src/drops/docker_ops/servers/nginx/conf.d/
--rwxr-xr-x   0 runner    (1001) docker     (123)      347 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/nginx/conf.d/drops.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.430108 drops-0.3.8/src/drops/docker_ops/servers/nginx/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)      280 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/nginx/lib/go_to_https.conf
--rwxr-xr-x   0 runner    (1001) docker     (123)      228 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/nginx/lib/gzip.conf
--rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/nginx/lib/referer.conf
--rwxr-xr-x   0 runner    (1001) docker     (123)      428 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/nginx/lib/ssl.conf
--rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/servers/nginx/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.430108 drops-0.3.8/src/drops/docker_ops/volumes/
--rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/docker_ops/volumes/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-02-16 14:25:20.000000 drops-0.3.8/src/drops/drops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:25:35.418108 drops-0.3.8/src/drops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    49809 2023-02-16 14:25:35.000000 drops-0.3.8/src/drops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-02-16 14:25:35.000000 drops-0.3.8/src/drops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 14:25:35.000000 drops-0.3.8/src/drops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-16 14:25:35.000000 drops-0.3.8/src/drops.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-16 14:25:35.000000 drops-0.3.8/src/drops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-16 14:25:35.000000 drops-0.3.8/src/drops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.542087 drops-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-06 14:11:54.000000 drops-0.3.9/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-03-06 14:11:54.000000 drops-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    49809 2023-03-06 14:12:05.542087 drops-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-03-06 14:11:54.000000 drops-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-06 14:11:54.000000 drops-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 14:12:05.542087 drops-0.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.526086 drops-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.530087 drops-0.3.9/src/drops/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.530087 drops-0.3.9/src/drops/console/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      707 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.538087 drops-0.3.9/src/drops/console/internal/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1872 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2342 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/backup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1499 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/clean_up.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5209 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1058 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/deploy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1498 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/deploy_https_key.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/echo_paths.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2851 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/er.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/exec.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      716 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/globals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3123 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/host.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1452 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/init.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/init_remove_env_debian.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14904 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/internal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/kill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1264 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/logs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1614 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/new.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1134 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/nginx_force_reload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1060 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/nginx_reload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1344 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/project.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      981 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/ps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/pull.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1138 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/redeploy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1096 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/restart.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1353 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/rm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/ssh.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1086 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/start.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1081 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/stop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1422 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1552 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/undeploy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1100 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/internal/up.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1827 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/console/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.538087 drops-0.3.9/src/drops/docker_ops/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       35 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2957 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/docker-compose.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)        7 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/drops.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.538087 drops-0.3.9/src/drops/docker_ops/release/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/release/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.538087 drops-0.3.9/src/drops/docker_ops/release/html/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/release/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.538087 drops-0.3.9/src/drops/docker_ops/secrets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/secrets/README.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.538087 drops-0.3.9/src/drops/docker_ops/secrets/home_ssh/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/secrets/home_ssh/id_ed25519
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/secrets/home_ssh/known_hosts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.538087 drops-0.3.9/src/drops/docker_ops/servers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      205 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.538087 drops-0.3.9/src/drops/docker_ops/servers/acme.sh/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      485 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/acme.sh/redeploy-ssl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.538087 drops-0.3.9/src/drops/docker_ops/servers/drops/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      262 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/drops/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.538087 drops-0.3.9/src/drops/docker_ops/servers/drops/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/drops/bin/.keep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.526086 drops-0.3.9/src/drops/docker_ops/servers/drops/cron/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.538087 drops-0.3.9/src/drops/docker_ops/servers/drops/cron/daily/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/drops/cron/daily/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.538087 drops-0.3.9/src/drops/docker_ops/servers/drops/cron/hourly/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/drops/cron/hourly/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.538087 drops-0.3.9/src/drops/docker_ops/servers/drops/cron/monthly/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/drops/cron/monthly/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.538087 drops-0.3.9/src/drops/docker_ops/servers/drops/cron/weekly/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/drops/cron/weekly/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.542087 drops-0.3.9/src/drops/docker_ops/servers/drops/cron_example/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      265 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/drops/cron_example/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/drops/cron_example/backup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      463 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/drops/cron_example/drops-backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.542087 drops-0.3.9/src/drops/docker_ops/servers/drops/drops/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      139 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/drops/drops/README.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.542087 drops-0.3.9/src/drops/docker_ops/servers/nginx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.542087 drops-0.3.9/src/drops/docker_ops/servers/nginx/conf.d/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      347 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/nginx/conf.d/drops.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.542087 drops-0.3.9/src/drops/docker_ops/servers/nginx/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      280 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/nginx/lib/go_to_https.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)      228 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/nginx/lib/gzip.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/nginx/lib/referer.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)      428 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/nginx/lib/ssl.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/servers/nginx/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.542087 drops-0.3.9/src/drops/docker_ops/volumes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/docker_ops/volumes/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-03-06 14:11:54.000000 drops-0.3.9/src/drops/drops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:12:05.530087 drops-0.3.9/src/drops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49809 2023-03-06 14:12:05.000000 drops-0.3.9/src/drops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-03-06 14:12:05.000000 drops-0.3.9/src/drops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:12:05.000000 drops-0.3.9/src/drops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-06 14:12:05.000000 drops-0.3.9/src/drops.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-06 14:12:05.000000 drops-0.3.9/src/drops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-06 14:12:05.000000 drops-0.3.9/src/drops.egg-info/top_level.txt
```

### Comparing `drops-0.3.8/LICENSE` & `drops-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/PKG-INFO` & `drops-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drops
-Version: 0.3.8
+Version: 0.3.9
 Summary: drops 是基于 ssh 和 docker-compose 的运维模板，附带的 drops 命令可以方便的管理项目，部署服务。
 Author-email: szerr <i@szerr.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `drops-0.3.8/README.md` & `drops-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/pyproject.toml` & `drops-0.3.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "drops"
-version = "v0.3.8"
+version = "v0.3.9"
 authors = [
   { name="szerr", email="i@szerr.org" },
 ]
 description = "drops 是基于 ssh 和 docker-compose 的运维模板，附带的 drops 命令可以方便的管理项目，部署服务。"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
```

### Comparing `drops-0.3.8/src/drops/__init__.py` & `drops-0.3.9/src/drops/__init__.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/__init__.py` & `drops-0.3.9/src/drops/console/__init__.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/__init__.py` & `drops-0.3.9/src/drops/console/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/backup.py` & `drops-0.3.9/src/drops/console/internal/backup.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/clean_up.py` & `drops-0.3.9/src/drops/console/internal/clean_up.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/config.py` & `drops-0.3.9/src/drops/console/internal/config.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/deploy.py` & `drops-0.3.9/src/drops/console/internal/deploy.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/deploy_https_key.py` & `drops-0.3.9/src/drops/console/internal/deploy_https_key.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/echo_paths.py` & `drops-0.3.9/src/drops/console/internal/echo_paths.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/er.py` & `drops-0.3.9/src/drops/console/internal/er.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/exec.py` & `drops-0.3.9/src/drops/console/internal/exec.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/globals.py` & `drops-0.3.9/src/drops/console/internal/globals.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/host.py` & `drops-0.3.9/src/drops/console/internal/host.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/init.py` & `drops-0.3.9/src/drops/console/internal/init.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/init_remove_env_debian.py` & `drops-0.3.9/src/drops/console/internal/init_remove_env_debian.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/internal.py` & `drops-0.3.9/src/drops/console/internal/internal.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/kill.py` & `drops-0.3.9/src/drops/console/internal/kill.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/logs.py` & `drops-0.3.9/src/drops/console/internal/logs.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/new.py` & `drops-0.3.9/src/drops/console/internal/new.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/nginx_force_reload.py` & `drops-0.3.9/src/drops/console/internal/nginx_force_reload.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/nginx_reload.py` & `drops-0.3.9/src/drops/console/internal/nginx_reload.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/project.py` & `drops-0.3.9/src/drops/console/internal/project.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/ps.py` & `drops-0.3.9/src/drops/console/internal/ps.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/pull.py` & `drops-0.3.9/src/drops/console/internal/pull.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/redeploy.py` & `drops-0.3.9/src/drops/console/internal/redeploy.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/restart.py` & `drops-0.3.9/src/drops/console/internal/restart.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/rm.py` & `drops-0.3.9/src/drops/console/internal/rm.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/ssh.py` & `drops-0.3.9/src/drops/console/internal/ssh.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/start.py` & `drops-0.3.9/src/drops/console/internal/start.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/stop.py` & `drops-0.3.9/src/drops/console/internal/stop.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/sync.py` & `drops-0.3.9/src/drops/console/internal/sync.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/undeploy.py` & `drops-0.3.9/src/drops/console/internal/undeploy.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/console/internal/up.py` & `drops-0.3.9/src/drops/console/internal/up.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,11 +24,11 @@
     internal.add_arg_host(p)
     internal.add_arg_container(p)
     p.set_defaults(func=up_cmd)
 
 
 def up_cmd(p):
     host = internal.get_arg_host_from_conf(p)
-    b = 'up -d '
+    b = 'up -d --remove-orphans'
     if p.container:
         b += ' ' + ' '.join(p.container)
     return internal.docker_compose_cmd(b, host)
```

### Comparing `drops-0.3.8/src/drops/console/main.py` & `drops-0.3.9/src/drops/console/main.py`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/docker_ops/docker-compose.yaml` & `drops-0.3.9/src/drops/docker_ops/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/docker_ops/servers/drops/cron_example/backup.sh` & `drops-0.3.9/src/drops/docker_ops/servers/drops/cron_example/backup.sh`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/docker_ops/servers/nginx/lib/referer.conf` & `drops-0.3.9/src/drops/docker_ops/servers/nginx/lib/referer.conf`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops/docker_ops/servers/nginx/nginx.conf` & `drops-0.3.9/src/drops/docker_ops/servers/nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `drops-0.3.8/src/drops.egg-info/PKG-INFO` & `drops-0.3.9/src/drops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drops
-Version: 0.3.8
+Version: 0.3.9
 Summary: drops 是基于 ssh 和 docker-compose 的运维模板，附带的 drops 命令可以方便的管理项目，部署服务。
 Author-email: szerr <i@szerr.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `drops-0.3.8/src/drops.egg-info/SOURCES.txt` & `drops-0.3.9/src/drops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

