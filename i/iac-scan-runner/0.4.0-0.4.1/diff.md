# Comparing `tmp/iac-scan-runner-0.4.0.tar.gz` & `tmp/iac-scan-runner-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac-scan-runner-0.4.0.tar", last modified: Thu May 11 06:18:40 2023, max compression
+gzip compressed data, was "iac-scan-runner-0.4.1.tar", last modified: Tue Jun  6 11:01:45 2023, max compression
```

## Comparing `iac-scan-runner-0.4.0.tar` & `iac-scan-runner-0.4.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.821981 iac-scan-runner-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.801981 iac-scan-runner-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.801981 iac-scan-runner-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2820 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    11438 2023-05-11 06:18:40.821981 iac-scan-runner-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9458 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.801981 iac-scan-runner-0.4.0/config/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/ansiblelint.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     8327 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/bandit.conf
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/dockerlint.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3678 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/git-leaks.toml
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/git-secrets.txt
--rw-r--r--   0 runner    (1001) docker     (122)      642 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/htmllint.json
--rw-r--r--   0 runner    (1001) docker     (122)     6690 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/javalint.xml
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/jslint.json
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/mdlint.rb
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/mdlint.rc
--rw-r--r--   0 runner    (1001) docker     (122)    16852 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/pylint.rc
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/scsslint.json
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/sonar-project.properties
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/tslint.json
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/config/yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      384 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/docker-compose.yaml
--rwxr-xr-x   0 runner    (1001) docker     (122)     6191 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/install-checks.sh
--rw-r--r--   0 runner    (1001) docker     (122)    26774 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/open-api.json
--rw-r--r--   0 runner    (1001) docker     (122)   271405 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (122)      659 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/package.json
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-05-11 06:18:40.821981 iac-scan-runner-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.801981 iac-scan-runner-0.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.805981 iac-scan-runner-0.4.0/src/iac_scan_runner/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.805981 iac-scan-runner-0.4.0/src/iac_scan_runner/asset/
--rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/asset/response.html
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/asset/table_basic.html
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/asset/table_info.html
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/asset/table_problem.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.813981 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/ansible_lint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/bandit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1711 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/checkstyle.py
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/cloc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/es_lint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/git_leaks.py
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/git_secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/gixy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/hadolint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1206 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/htmlhint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/markdown_lint.py
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/opera_tosca_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/pylint.py
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/pyup_safety.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/shellcheck.py
--rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/snyk.py
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/sonar_scanner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/steampunk_scanner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/stylelint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/terrascan.py
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/tflint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1203 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/tfsec.py
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/ts_lint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/checks/yamllint.py
--rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.817981 iac-scan-runner-0.4.0/src/iac_scan_runner/enums/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/enums/check_target_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/enums/scan_response_type.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.817981 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      733 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/check_output.py
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/cleanup_old_scans.py
--rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (122)     4316 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/project_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5031 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/results_persistence.py
--rw-r--r--   0 runner    (1001) docker     (122)    13500 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/results_summary.py
--rw-r--r--   0 runner    (1001) docker     (122)     7265 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/scan_project.py
--rw-r--r--   0 runner    (1001) docker     (122)    20230 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/scan_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.817981 iac-scan-runner-0.4.0/src/iac_scan_runner/interface/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1549 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/interface/check.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.821981 iac-scan-runner-0.4.0/src/iac_scan_runner/model/
--rw-r--r--   0 runner    (1001) docker     (122)      994 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/model/ConfigureCheck.py
--rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/model/Scan.py
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/object_store.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.821981 iac-scan-runner-0.4.0/src/iac_scan_runner/routers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5701 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/routers/checks.py
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/routers/openapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/routers/project.py
--rw-r--r--   0 runner    (1001) docker     (122)     4274 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-05-11 06:14:08.000000 iac-scan-runner-0.4.0/src/iac_scan_runner/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 06:18:40.805981 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11438 2023-05-11 06:18:40.000000 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-05-11 06:18:40.000000 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 06:18:40.000000 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-11 06:18:40.000000 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-11 06:18:40.000000 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-11 06:18:40.000000 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 06:18:40.000000 iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 11:01:45.713399 iac-scan-runner-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 11:01:45.701399 iac-scan-runner-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 11:01:45.705399 iac-scan-runner-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2820 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    11438 2023-06-06 11:01:45.713399 iac-scan-runner-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9458 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 11:01:45.705399 iac-scan-runner-0.4.1/config/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/ansiblelint.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     8327 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/bandit.conf
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/dockerlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3678 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/git-leaks.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/git-secrets.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      642 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/htmllint.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6690 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/javalint.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/jslint.json
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/mdlint.rb
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/mdlint.rc
+-rw-r--r--   0 runner    (1001) docker     (122)    16852 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/pylint.rc
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/scsslint.json
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/sonar-project.properties
+-rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/tslint.json
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/config/yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      384 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/docker-compose.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6191 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/install-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (122)    26774 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/open-api.json
+-rw-r--r--   0 runner    (1001) docker     (122)   271405 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (122)      659 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-06-06 11:01:45.713399 iac-scan-runner-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 11:01:45.705399 iac-scan-runner-0.4.1/src/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 11:01:45.705399 iac-scan-runner-0.4.1/src/iac_scan_runner/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 11:01:45.705399 iac-scan-runner-0.4.1/src/iac_scan_runner/asset/
+-rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/asset/response.html
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/asset/table_basic.html
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/asset/table_info.html
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/asset/table_problem.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 11:01:45.709399 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/ansible_lint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1711 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/checkstyle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/cloc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/es_lint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/git_leaks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/git_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/gixy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/hadolint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1206 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/htmlhint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/markdown_lint.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/opera_tosca_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/pyup_safety.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/shellcheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/snyk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/sonar_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/steampunk_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/stylelint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/terrascan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/tflint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1203 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/tfsec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/ts_lint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/checks/yamllint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 11:01:45.709399 iac-scan-runner-0.4.1/src/iac_scan_runner/enums/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/enums/check_target_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/enums/scan_response_type.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 11:01:45.713399 iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      733 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/check_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/cleanup_old_scans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4316 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5031 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/results_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13500 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/results_summary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7265 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/scan_project.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20230 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/scan_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 11:01:45.713399 iac-scan-runner-0.4.1/src/iac_scan_runner/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1549 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/interface/check.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 11:01:45.713399 iac-scan-runner-0.4.1/src/iac_scan_runner/model/
+-rw-r--r--   0 runner    (1001) docker     (122)      994 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/model/ConfigureCheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/model/Scan.py
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/object_store.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 11:01:45.713399 iac-scan-runner-0.4.1/src/iac_scan_runner/routers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5732 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/routers/checks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/routers/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/routers/project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4274 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-06-06 10:58:15.000000 iac-scan-runner-0.4.1/src/iac_scan_runner/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 11:01:45.705399 iac-scan-runner-0.4.1/src/iac_scan_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11438 2023-06-06 11:01:45.000000 iac-scan-runner-0.4.1/src/iac_scan_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-06-06 11:01:45.000000 iac-scan-runner-0.4.1/src/iac_scan_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 11:01:45.000000 iac-scan-runner-0.4.1/src/iac_scan_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-06 11:01:45.000000 iac-scan-runner-0.4.1/src/iac_scan_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-06 11:01:45.000000 iac-scan-runner-0.4.1/src/iac_scan_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-06 11:01:45.000000 iac-scan-runner-0.4.1/src/iac_scan_runner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 11:01:45.000000 iac-scan-runner-0.4.1/src/iac_scan_runner.egg-info/zip-safe
```

### Comparing `iac-scan-runner-0.4.0/.dockerignore` & `iac-scan-runner-0.4.1/.dockerignore`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/.github/workflows/ci_cd.yml` & `iac-scan-runner-0.4.1/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/.gitignore` & `iac-scan-runner-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/Dockerfile` & `iac-scan-runner-0.4.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/LICENSE` & `iac-scan-runner-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/PKG-INFO` & `iac-scan-runner-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-scan-runner
-Version: 0.4.0
+Version: 0.4.1
 Summary: IaC Scan Runner CLI
 Home-page: https://github.com/xlab-si/iac-scan-runner
 Author: XLAB d.o.o.
 Author-email: pypi@xlab.si
 Maintainer: xOpera team
 Maintainer-email: xopera@xlab.si
 Project-URL: Source Code, https://github.com/xlab-si/iac-scan-runner
```

### Comparing `iac-scan-runner-0.4.0/README.md` & `iac-scan-runner-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/config/bandit.conf` & `iac-scan-runner-0.4.1/config/bandit.conf`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/config/git-leaks.toml` & `iac-scan-runner-0.4.1/config/git-leaks.toml`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/config/htmllint.json` & `iac-scan-runner-0.4.1/config/htmllint.json`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/config/javalint.xml` & `iac-scan-runner-0.4.1/config/javalint.xml`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/config/jslint.json` & `iac-scan-runner-0.4.1/config/jslint.json`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/config/pylint.rc` & `iac-scan-runner-0.4.1/config/pylint.rc`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/config/scsslint.json` & `iac-scan-runner-0.4.1/config/scsslint.json`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/config/tslint.json` & `iac-scan-runner-0.4.1/config/tslint.json`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/install-checks.sh` & `iac-scan-runner-0.4.1/install-checks.sh`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/open-api.json` & `iac-scan-runner-0.4.1/open-api.json`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/package-lock.json` & `iac-scan-runner-0.4.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/package.json` & `iac-scan-runner-0.4.1/package.json`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/setup.cfg` & `iac-scan-runner-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/api.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/api.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/asset/response.html` & `iac-scan-runner-0.4.1/src/iac_scan_runner/asset/response.html`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/ansible_lint.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/ansible_lint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/bandit.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/bandit.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/checkstyle.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/checkstyle.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/cloc.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/cloc.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/es_lint.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/es_lint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/git_leaks.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/git_leaks.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/git_secrets.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/git_secrets.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/gixy.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/gixy.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/hadolint.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/hadolint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/htmlhint.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/htmlhint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/markdown_lint.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/markdown_lint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/opera_tosca_parser.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/opera_tosca_parser.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/pylint.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/pylint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/pyup_safety.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/pyup_safety.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/shellcheck.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/shellcheck.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/snyk.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/snyk.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/sonar_scanner.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/sonar_scanner.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/steampunk_scanner.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/steampunk_scanner.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/stylelint.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/stylelint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/terrascan.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/terrascan.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/tflint.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/tflint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/tfsec.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/tfsec.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/ts_lint.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/ts_lint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/checks/yamllint.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/checks/yamllint.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/cli.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/cli.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/check_output.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/check_output.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/compatibility.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/compatibility.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/project_config.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/project_config.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/results_persistence.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/results_persistence.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/results_summary.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/results_summary.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/scan_project.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/scan_project.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/functionality/scan_runner.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/functionality/scan_runner.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/interface/check.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/interface/check.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/model/ConfigureCheck.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/model/ConfigureCheck.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/model/Scan.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/model/Scan.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/object_store.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/object_store.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/routers/checks.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/routers/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from fastapi import APIRouter
 from fastapi import status, Depends
 from fastapi.responses import JSONResponse, HTMLResponse
 
 from iac_scan_runner.enums.check_target_entity_type import CheckTargetEntityType
 from iac_scan_runner.enums.scan_response_type import ScanResponseType
 from iac_scan_runner.model.ConfigureCheck import CheckConfigurationModel
-from iac_scan_runner.model.Scan import ScanModel
+from iac_scan_runner.model.Scan import ScanModel, ScanModelDeprecated
 from iac_scan_runner.object_store import scan_runner
 
 router = APIRouter(tags=["Checks"])
 
 
 @router.get("/default/checks", summary="Retrieve and filter checks", responses={200: {}, 400: {"model": str}})
 async def get_checks(keyword: Optional[str] = None, enabled: Optional[bool] = None, configured: Optional[bool] = None,
@@ -92,15 +92,15 @@
         return JSONResponse(status_code=status.HTTP_200_OK,
                             content=scan_runner.configure_check(check_name, form_data.config_file, form_data.secret))
     except Exception as e:
         return JSONResponse(status_code=status.HTTP_400_BAD_REQUEST, content=str(e))
 
 
 @router.post("/default/scan", summary="Initiate IaC scan", responses={200: {}, 400: {"model": str}})
-async def post_scan(form_data: ScanModel = Depends(ScanModel.as_form),
+async def post_scan(form_data: ScanModel = Depends(ScanModelDeprecated.as_form),
                     scan_response_type: ScanResponseType = ScanResponseType.json) -> Union[JSONResponse, HTMLResponse]:
     """
     Run IaC scan
     \f
     :param form_data: Form data model
     :param scan_response_type: Scan response type (JSON or HTML)
     :return: JSONResponse or HTMLResponse object (with status code 200 or 400)
```

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/routers/openapi.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/routers/openapi.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/routers/project.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/routers/project.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/utils.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/utils.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner/vars.py` & `iac-scan-runner-0.4.1/src/iac_scan_runner/vars.py`

 * *Files identical despite different names*

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/PKG-INFO` & `iac-scan-runner-0.4.1/src/iac_scan_runner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-scan-runner
-Version: 0.4.0
+Version: 0.4.1
 Summary: IaC Scan Runner CLI
 Home-page: https://github.com/xlab-si/iac-scan-runner
 Author: XLAB d.o.o.
 Author-email: pypi@xlab.si
 Maintainer: xOpera team
 Maintainer-email: xopera@xlab.si
 Project-URL: Source Code, https://github.com/xlab-si/iac-scan-runner
```

### Comparing `iac-scan-runner-0.4.0/src/iac_scan_runner.egg-info/SOURCES.txt` & `iac-scan-runner-0.4.1/src/iac_scan_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

