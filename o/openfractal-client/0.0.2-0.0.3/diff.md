# Comparing `tmp/openfractal_client-0.0.2.tar.gz` & `tmp/openfractal_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfractal_client-0.0.2.tar", last modified: Mon Jun  5 21:53:30 2023, max compression
+gzip compressed data, was "openfractal_client-0.0.3.tar", last modified: Mon Jun  5 21:56:46 2023, max compression
```

## Comparing `openfractal_client-0.0.2.tar` & `openfractal_client-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:53:30.362626 openfractal_client-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:53:30.362626 openfractal_client-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:53:30.362626 openfractal_client-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/CHANGELOGS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-05 21:53:30.362626 openfractal_client-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:53:30.362626 openfractal_client-0.0.2/docker/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1191 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/docker/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:53:30.362626 openfractal_client-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:53:30.362626 openfractal_client-0.0.2/openfractal_client/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/openfractal_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/openfractal_client/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:53:30.362626 openfractal_client-0.0.2/openfractal_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-05 21:53:30.000000 openfractal_client-0.0.2/openfractal_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-05 21:53:30.000000 openfractal_client-0.0.2/openfractal_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:53:30.000000 openfractal_client-0.0.2/openfractal_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 21:53:30.000000 openfractal_client-0.0.2/openfractal_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:53:30.362626 openfractal_client-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:53:30.362626 openfractal_client-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 21:52:54.000000 openfractal_client-0.0.2/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.132992 openfractal_client-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.128992 openfractal_client-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.128992 openfractal_client-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/CHANGELOGS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-05 21:56:46.132992 openfractal_client-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.128992 openfractal_client-0.0.3/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1191 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/docker/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.128992 openfractal_client-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.128992 openfractal_client-0.0.3/openfractal_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/openfractal_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/openfractal_client/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.132992 openfractal_client-0.0.3/openfractal_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-05 21:56:46.000000 openfractal_client-0.0.3/openfractal_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-05 21:56:46.000000 openfractal_client-0.0.3/openfractal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:56:46.000000 openfractal_client-0.0.3/openfractal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 21:56:46.000000 openfractal_client-0.0.3/openfractal_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:56:46.132992 openfractal_client-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:56:46.132992 openfractal_client-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 21:56:10.000000 openfractal_client-0.0.3/tests/test_import.py
```

### Comparing `openfractal_client-0.0.2/.github/CODE_OF_CONDUCT.md` & `openfractal_client-0.0.3/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.2/.github/workflows/code-check.yml` & `openfractal_client-0.0.3/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.2/.github/workflows/doc.yml` & `openfractal_client-0.0.3/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.2/.github/workflows/docker.yml` & `openfractal_client-0.0.3/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.2/.github/workflows/release.yml` & `openfractal_client-0.0.3/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     inputs:
       release-version:
         description: "A valid Semver version string"
         required: true
 
 permissions:
   contents: write
+  pull-requests: write
 
 jobs:
   release:
     # Do not release if not triggered from the default branch
     if: github.ref == format('refs/heads/{0}', github.event.repository.default_branch)
 
     runs-on: ubuntu-latest
@@ -64,26 +65,36 @@
 
           if [ "$IS_HIGHER_VERSION" != "1" ]; then
             echo "The version '$RELEASE_VERSION' is not higher than the latest version '$LATEST_VERSION'."
             echo "The release process is aborted."
             exit 1
           fi
 
+      - name: Build Changelog
+        id: github_release
+        uses: mikepenz/release-changelog-builder-action@v4
+        env:
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+          outputFile: CHANGELOGS.md
+
       - name: Configure git
         run: |
           git config --global user.name "${GITHUB_ACTOR}"
           git config --global user.email "${GITHUB_ACTOR}@users.noreply.github.com"
 
       - name: Create and push git tag
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: |
           # Tag the release
           git tag -a "${{ inputs.release-version }}" -m "Release version ${{ inputs.release-version }}"
 
+          # Push the modified changelogs
+          git push origin main
+
           # Push the tags
           git push origin "${{ inputs.release-version }}"
 
       - name: Install library
         run: python -m pip install --no-deps .
 
       - name: Build the wheel and sdist
@@ -91,19 +102,12 @@
 
       - name: Publish package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
           packages-dir: dist/
 
-      - name: Build Changelog
-        id: github_release
-        uses: mikepenz/release-changelog-builder-action@v4
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-          outputFile: CHANGELOGS.md
-
       - name: Create GitHub Release
         uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
         with:
           tag_name: ${{ inputs.release-version }}
           body: ${{steps.github_release.outputs.changelog}}
```

### Comparing `openfractal_client-0.0.2/.github/workflows/test.yml` & `openfractal_client-0.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.2/Dockerfile` & `openfractal_client-0.0.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.2/LICENSE` & `openfractal_client-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.2/PKG-INFO` & `openfractal_client-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfractal_client
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python client based on QCPortal for Open Drug Discovery (ODD) QM large scale data generation.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Source Code, https://github.com/OpenDrugDiscovery/openfractal-client
 Project-URL: Bug Tracker, https://github.com/OpenDrugDiscovery/openfractal-client/issues
 Project-URL: Documentation, https://github.com/OpenDrugDiscovery/openfractal-client
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openfractal_client-0.0.2/README.md` & `openfractal_client-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.2/docker/entrypoint.sh` & `openfractal_client-0.0.3/docker/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.2/docker-compose.yml` & `openfractal_client-0.0.3/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.2/env.yml` & `openfractal_client-0.0.3/env.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.2/mkdocs.yml` & `openfractal_client-0.0.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.2/openfractal_client.egg-info/PKG-INFO` & `openfractal_client-0.0.3/openfractal_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfractal-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python client based on QCPortal for Open Drug Discovery (ODD) QM large scale data generation.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Source Code, https://github.com/OpenDrugDiscovery/openfractal-client
 Project-URL: Bug Tracker, https://github.com/OpenDrugDiscovery/openfractal-client/issues
 Project-URL: Documentation, https://github.com/OpenDrugDiscovery/openfractal-client
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openfractal_client-0.0.2/openfractal_client.egg-info/SOURCES.txt` & `openfractal_client-0.0.3/openfractal_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.2/pyproject.toml` & `openfractal_client-0.0.3/pyproject.toml`

 * *Files identical despite different names*

