# Comparing `tmp/openfractal_client-0.0.3.tar.gz` & `tmp/openfractal_client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfractal_client-0.0.3.tar", last modified: Mon Jun  5 21:56:46 2023, max compression
+gzip compressed data, was "openfractal_client-0.0.4.tar", last modified: Mon Jun  5 22:01:50 2023, max compression
```

## Comparing `openfractal_client-0.0.3.tar` & `openfractal_client-0.0.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.132992 openfractal_client-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.128992 openfractal_client-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.128992 openfractal_client-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/CHANGELOGS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-05 21:56:46.132992 openfractal_client-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.128992 openfractal_client-0.0.3/docker/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1191 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/docker/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.128992 openfractal_client-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.128992 openfractal_client-0.0.3/openfractal_client/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/openfractal_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/openfractal_client/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.132992 openfractal_client-0.0.3/openfractal_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-05 21:56:46.000000 openfractal_client-0.0.3/openfractal_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-05 21:56:46.000000 openfractal_client-0.0.3/openfractal_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:56:46.000000 openfractal_client-0.0.3/openfractal_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 21:56:46.000000 openfractal_client-0.0.3/openfractal_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:56:46.132992 openfractal_client-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.132992 openfractal_client-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:01:50.847861 openfractal_client-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:01:50.843861 openfractal_client-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:01:50.847861 openfractal_client-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/CHANGELOGS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-05 22:01:50.847861 openfractal_client-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:01:50.847861 openfractal_client-0.0.4/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1191 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/docker/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:01:50.847861 openfractal_client-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:01:50.847861 openfractal_client-0.0.4/openfractal_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/openfractal_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/openfractal_client/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:01:50.847861 openfractal_client-0.0.4/openfractal_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-05 22:01:50.000000 openfractal_client-0.0.4/openfractal_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-05 22:01:50.000000 openfractal_client-0.0.4/openfractal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 22:01:50.000000 openfractal_client-0.0.4/openfractal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 22:01:50.000000 openfractal_client-0.0.4/openfractal_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 22:01:50.847861 openfractal_client-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:01:50.847861 openfractal_client-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 22:01:00.000000 openfractal_client-0.0.4/tests/test_import.py
```

### Comparing `openfractal_client-0.0.3/.github/CODE_OF_CONDUCT.md` & `openfractal_client-0.0.4/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.3/.github/workflows/code-check.yml` & `openfractal_client-0.0.4/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.3/.github/workflows/doc.yml` & `openfractal_client-0.0.4/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.3/.github/workflows/docker.yml` & `openfractal_client-0.0.4/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.3/.github/workflows/release.yml` & `openfractal_client-0.0.4/.github/workflows/release.yml`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,14 @@
           fi
 
       - name: Build Changelog
         id: github_release
         uses: mikepenz/release-changelog-builder-action@v4
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-          outputFile: CHANGELOGS.md
 
       - name: Configure git
         run: |
           git config --global user.name "${GITHUB_ACTOR}"
           git config --global user.email "${GITHUB_ACTOR}@users.noreply.github.com"
 
       - name: Create and push git tag
```

### Comparing `openfractal_client-0.0.3/.github/workflows/test.yml` & `openfractal_client-0.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.3/Dockerfile` & `openfractal_client-0.0.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.3/LICENSE` & `openfractal_client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.3/PKG-INFO` & `openfractal_client-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfractal_client
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python client based on QCPortal for Open Drug Discovery (ODD) QM large scale data generation.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Source Code, https://github.com/OpenDrugDiscovery/openfractal-client
 Project-URL: Bug Tracker, https://github.com/OpenDrugDiscovery/openfractal-client/issues
 Project-URL: Documentation, https://github.com/OpenDrugDiscovery/openfractal-client
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openfractal_client-0.0.3/README.md` & `openfractal_client-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.3/docker/entrypoint.sh` & `openfractal_client-0.0.4/docker/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.3/docker-compose.yml` & `openfractal_client-0.0.4/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.3/env.yml` & `openfractal_client-0.0.4/env.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.3/mkdocs.yml` & `openfractal_client-0.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.3/openfractal_client.egg-info/PKG-INFO` & `openfractal_client-0.0.4/openfractal_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfractal-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python client based on QCPortal for Open Drug Discovery (ODD) QM large scale data generation.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Source Code, https://github.com/OpenDrugDiscovery/openfractal-client
 Project-URL: Bug Tracker, https://github.com/OpenDrugDiscovery/openfractal-client/issues
 Project-URL: Documentation, https://github.com/OpenDrugDiscovery/openfractal-client
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openfractal_client-0.0.3/openfractal_client.egg-info/SOURCES.txt` & `openfractal_client-0.0.4/openfractal_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.3/pyproject.toml` & `openfractal_client-0.0.4/pyproject.toml`

 * *Files identical despite different names*

