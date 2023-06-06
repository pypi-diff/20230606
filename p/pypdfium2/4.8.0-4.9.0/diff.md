# Comparing `tmp/pypdfium2-4.8.0.tar.gz` & `tmp/pypdfium2-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdfium2-4.8.0.tar", last modified: Tue Apr 25 04:02:15 2023, max compression
+gzip compressed data, was "pypdfium2-4.9.0.tar", last modified: Tue May  2 04:01:19 2023, max compression
```

## Comparing `pypdfium2-4.8.0.tar` & `pypdfium2-4.9.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.775060 pypdfium2-4.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.763060 pypdfium2-4.8.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/.reuse/dep5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.763060 pypdfium2-4.8.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    43950 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/LICENSES/LicenseRef-PdfiumThirdParty.txt
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    40298 2023-04-25 04:02:15.775060 pypdfium2-4.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 04:02:15.775060 pypdfium2-4.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.759060 pypdfium2-4.8.0/setupsrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.763060 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/autorelease.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10887 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/build_pdfium.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/craft_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/packaging_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/setup_base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6272 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/setupsrc/pypdfium2_setup/update_pdfium.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.759060 pypdfium2-4.8.0/sourcebuild/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.763060 pypdfium2-4.8.0/sourcebuild/patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/sourcebuild/patches/public_headers.patch
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/sourcebuild/patches/shared_library.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.763060 pypdfium2-4.8.0/sourcebuild/patches/win/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/sourcebuild/patches/win/build.patch
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/sourcebuild/patches/win/pdfium.patch
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/sourcebuild/patches/win/resources.rc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.759060 pypdfium2-4.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.767060 pypdfium2-4.8.0/src/pypdfium2/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.771060 pypdfium2-4.8.0/src/pypdfium2/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/arrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/extract_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/extract_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/imgtopdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/pageobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/pdfinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_cli/toc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.771060 pypdfium2-4.8.0/src/pypdfium2/_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.775060 pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/bitmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    26905 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/pageobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/textpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/_helpers/unsupported.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-25 04:00:57.000000 pypdfium2-4.8.0/src/pypdfium2/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-25 04:01:33.000000 pypdfium2-4.8.0/src/pypdfium2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:02:15.767060 pypdfium2-4.8.0/src/pypdfium2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40298 2023-04-25 04:02:15.000000 pypdfium2-4.8.0/src/pypdfium2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-25 04:02:15.000000 pypdfium2-4.8.0/src/pypdfium2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:02:15.000000 pypdfium2-4.8.0/src/pypdfium2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-25 04:02:15.000000 pypdfium2-4.8.0/src/pypdfium2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 04:02:15.000000 pypdfium2-4.8.0/src/pypdfium2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:01:19.566763 pypdfium2-4.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:01:19.558762 pypdfium2-4.9.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/.reuse/dep5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:01:19.558762 pypdfium2-4.9.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    43950 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/LICENSES/LicenseRef-PdfiumThirdParty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    40298 2023-05-02 04:01:19.566763 pypdfium2-4.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 04:01:19.566763 pypdfium2-4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:01:19.554762 pypdfium2-4.9.0/setupsrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:01:19.558762 pypdfium2-4.9.0/setupsrc/pypdfium2_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/setupsrc/pypdfium2_setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/setupsrc/pypdfium2_setup/autorelease.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10887 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/setupsrc/pypdfium2_setup/build_pdfium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/setupsrc/pypdfium2_setup/craft_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/setupsrc/pypdfium2_setup/packaging_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/setupsrc/pypdfium2_setup/setup_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6272 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/setupsrc/pypdfium2_setup/update_pdfium.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:01:19.554762 pypdfium2-4.9.0/sourcebuild/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:01:19.558762 pypdfium2-4.9.0/sourcebuild/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/sourcebuild/patches/public_headers.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/sourcebuild/patches/shared_library.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:01:19.558762 pypdfium2-4.9.0/sourcebuild/patches/win/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/sourcebuild/patches/win/build.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/sourcebuild/patches/win/pdfium.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/sourcebuild/patches/win/resources.rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:01:19.558762 pypdfium2-4.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:01:19.558762 pypdfium2-4.9.0/src/pypdfium2/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:01:19.562763 pypdfium2-4.9.0/src/pypdfium2/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_cli/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_cli/arrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_cli/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_cli/extract_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_cli/extract_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_cli/imgtopdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_cli/pageobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_cli/pdfinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_cli/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_cli/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_cli/toc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:01:19.562763 pypdfium2-4.9.0/src/pypdfium2/_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:01:19.566763 pypdfium2-4.9.0/src/pypdfium2/_helpers/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_helpers/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_helpers/_internal/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_helpers/_internal/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_helpers/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_helpers/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_helpers/bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_helpers/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_helpers/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_helpers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19640 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_helpers/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16792 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_helpers/pageobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_helpers/textpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/_helpers/unsupported.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-02 04:00:33.000000 pypdfium2-4.9.0/src/pypdfium2/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-02 04:01:00.000000 pypdfium2-4.9.0/src/pypdfium2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:01:19.562763 pypdfium2-4.9.0/src/pypdfium2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40298 2023-05-02 04:01:19.000000 pypdfium2-4.9.0/src/pypdfium2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-02 04:01:19.000000 pypdfium2-4.9.0/src/pypdfium2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:01:19.000000 pypdfium2-4.9.0/src/pypdfium2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 04:01:19.000000 pypdfium2-4.9.0/src/pypdfium2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 04:01:19.000000 pypdfium2-4.9.0/src/pypdfium2.egg-info/top_level.txt
```

### Comparing `pypdfium2-4.8.0/.reuse/dep5` & `pypdfium2-4.9.0/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/LICENSES/Apache-2.0.txt` & `pypdfium2-4.9.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/LICENSES/BSD-3-Clause.txt` & `pypdfium2-4.9.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/LICENSES/CC-BY-4.0.txt` & `pypdfium2-4.9.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/LICENSES/LicenseRef-PdfiumThirdParty.txt` & `pypdfium2-4.9.0/LICENSES/LicenseRef-PdfiumThirdParty.txt`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/MANIFEST.in` & `pypdfium2-4.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/PKG-INFO` & `pypdfium2-4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdfium2
-Version: 4.8.0
+Version: 4.9.0
 Summary: Python bindings to PDFium
 Author: pypdfium2-team
 Author-email: geisserml <geisserml@gmail.com>
 License: Apache-2.0 or BSD-3-Clause
 Project-URL: homepage, https://github.com/pypdfium2-team/pypdfium2
 Project-URL: documentation, https://pypdfium2.readthedocs.io/
 Project-URL: changelog, https://pypdfium2.readthedocs.io/en/stable/changelog.html
```

### Comparing `pypdfium2-4.8.0/README.md` & `pypdfium2-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/pyproject.toml` & `pypdfium2-4.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/setup.py` & `pypdfium2-4.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/setupsrc/pypdfium2_setup/autorelease.py` & `pypdfium2-4.9.0/setupsrc/pypdfium2_setup/autorelease.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/setupsrc/pypdfium2_setup/build_pdfium.py` & `pypdfium2-4.9.0/setupsrc/pypdfium2_setup/build_pdfium.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/setupsrc/pypdfium2_setup/craft_packages.py` & `pypdfium2-4.9.0/setupsrc/pypdfium2_setup/craft_packages.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/setupsrc/pypdfium2_setup/packaging_base.py` & `pypdfium2-4.9.0/setupsrc/pypdfium2_setup/packaging_base.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/setupsrc/pypdfium2_setup/setup_base.py` & `pypdfium2-4.9.0/setupsrc/pypdfium2_setup/setup_base.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/setupsrc/pypdfium2_setup/update_pdfium.py` & `pypdfium2-4.9.0/setupsrc/pypdfium2_setup/update_pdfium.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/sourcebuild/patches/public_headers.patch` & `pypdfium2-4.9.0/sourcebuild/patches/public_headers.patch`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/sourcebuild/patches/win/build.patch` & `pypdfium2-4.9.0/sourcebuild/patches/win/build.patch`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/sourcebuild/patches/win/resources.rc` & `pypdfium2-4.9.0/sourcebuild/patches/win/resources.rc`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/__main__.py` & `pypdfium2-4.9.0/src/pypdfium2/__main__.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_cli/_parsers.py` & `pypdfium2-4.9.0/src/pypdfium2/_cli/_parsers.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_cli/arrange.py` & `pypdfium2-4.9.0/src/pypdfium2/_cli/arrange.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_cli/attachments.py` & `pypdfium2-4.9.0/src/pypdfium2/_cli/attachments.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_cli/extract_images.py` & `pypdfium2-4.9.0/src/pypdfium2/_cli/extract_images.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,30 +44,33 @@
     
     if not args.output_dir.is_dir():
         raise NotADirectoryError(args.output_dir)
     if args.use_bitmap and not args.format:
         args.format = "png"
     
     pdf = get_input(args)
+    n_pdigits = len(str( max(args.pages)+1 ))
     
-    images = []
     for i in args.pages:
+        
         page = pdf[i]
-        obj_searcher = page.get_objects(
+        images = page.get_objects(
             filter = (pdfium_c.FPDF_PAGEOBJ_IMAGE, ),
             max_depth = args.max_depth,
         )
-        images += list(obj_searcher)
-    
-    n_digits = len(str(len(images)))
-    
-    for i, image in enumerate(images):
-        prefix = args.output_dir / ("%s_%0*d" % (args.input.stem, n_digits, i+1))
         
-        try:
-            if args.use_bitmap:
-                pil_image = image.get_bitmap(render=args.render).to_pil()
-                pil_image.save(f"{prefix}.{args.format}")
-            else:
-                image.extract(prefix, fb_format=args.format, fb_render=args.render)
-        except pdfium.PdfiumError:
-            traceback.print_exc()
+        # not perfectly memory efficient, but we need image count for digit formatting
+        images = list(images)
+        n_idigits = len(str( len(images) ))
+        
+        for j, image in enumerate(images):
+            stem = "%s_%0*d_%0*d" % (args.input.stem, n_pdigits, i+1, n_idigits, j+1)
+            prefix = args.output_dir / stem
+            try:
+                if args.use_bitmap:
+                    pil_image = image.get_bitmap(render=args.render).to_pil()
+                    pil_image.save( prefix.with_suffix("."+args.format) )
+                else:
+                    image.extract(prefix, fb_format=args.format, fb_render=args.render)
+            except pdfium.PdfiumError:
+                traceback.print_exc()
+            image.close()
```

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_cli/extract_text.py` & `pypdfium2-4.9.0/src/pypdfium2/_cli/extract_text.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_cli/imgtopdf.py` & `pypdfium2-4.9.0/src/pypdfium2/_cli/imgtopdf.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_cli/pageobjects.py` & `pypdfium2-4.9.0/src/pypdfium2/_cli/pageobjects.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_cli/pdfinfo.py` & `pypdfium2-4.9.0/src/pypdfium2/_cli/pdfinfo.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_cli/render.py` & `pypdfium2-4.9.0/src/pypdfium2/_cli/render.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_cli/tile.py` & `pypdfium2-4.9.0/src/pypdfium2/_cli/tile.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class Units (Enum):
     PT = 0
     MM = 1
     CM = 2
     IN = 3
 
 
-def units_to_pt(value, unit: Units):
+def units_to_pt(value, unit):
     if unit is Units.PT:
         return value
     elif unit is Units.IN:
         return value*72
     elif unit is Units.CM:
         return (value*72) / 2.54
     elif unit is Units.MM:
@@ -70,18 +70,14 @@
 
 
 def main(args):
     
     # Rudimentary page tiling, powered by pdfium
     # A more sophisticated implementation could place XObjects rather than using PDFium's helper function, support merging and arranging on the fly, etc.
     
-    width = units_to_pt(args.width, args.unit)
-    height = units_to_pt(args.height, args.unit)
+    w = units_to_pt(args.width, args.unit)
+    h = units_to_pt(args.height, args.unit)
     
     src_pdf = get_input(args)
-    raw_dest = pdfium_c.FPDF_ImportNPagesToOne(
-        src_pdf,
-        width, height,
-        args.cols, args.rows,
-    )
+    raw_dest = pdfium_c.FPDF_ImportNPagesToOne(src_pdf, w, h, args.cols, args.rows)
     dest_pdf = pdfium.PdfDocument(raw_dest)
     dest_pdf.save(args.output)
```

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_cli/toc.py` & `pypdfium2-4.9.0/src/pypdfium2/_cli/toc.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_helpers/__init__.py` & `pypdfium2-4.9.0/src/pypdfium2/_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/bases.py` & `pypdfium2-4.9.0/src/pypdfium2/_helpers/_internal/bases.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/consts.py` & `pypdfium2-4.9.0/src/pypdfium2/_helpers/_internal/consts.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_helpers/_internal/utils.py` & `pypdfium2-4.9.0/src/pypdfium2/_helpers/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_helpers/attachment.py` & `pypdfium2-4.9.0/src/pypdfium2/_helpers/attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,15 @@
     
     # Problems with PDFium's attachment API:
     # - https://crbug.com/pdfium/1939
     # - https://crbug.com/pdfium/893
     
     
     def __init__(self, raw, pdf):
-        self.raw = raw
-        self.pdf = pdf
+        self.raw, self.pdf = raw, pdf
     
     
     def get_name(self):
         """
         Returns:
             str: Name of the attachment.
         """
```

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_helpers/bitmap.py` & `pypdfium2-4.9.0/src/pypdfium2/_helpers/bitmap.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,38 +41,20 @@
     Attributes:
         raw (FPDF_BITMAP):
             The underlying PDFium bitmap handle.
         buffer (~ctypes.c_ubyte):
             A ctypes array representation of the pixel data (each item is an unsigned byte, i. e. a number ranging from 0 to 255).
     """
     
-    def __init__(
-            self,
-            raw,
-            buffer,
-            width,
-            height,
-            stride,
-            format,
-            rev_byteorder,
-            needs_free,
-        ):
-        self.raw = raw
-        self.buffer = buffer
-        self.width = width
-        self.height = height
-        self.stride = stride
-        self.format = format
-        self.rev_byteorder = rev_byteorder
+    def __init__(self, raw, buffer, width, height, stride, format, rev_byteorder, needs_free):
+        self.raw, self.buffer = raw, buffer
+        self.width, self.height, self.stride = width, height, stride
+        self.format, self.rev_byteorder = format, rev_byteorder
         self.n_channels = consts.BitmapTypeToNChannels[self.format]
-        if self.rev_byteorder:
-            self.mode = consts.BitmapTypeToStrReverse[self.format]
-        else:
-            self.mode = consts.BitmapTypeToStr[self.format]
-        
+        self.mode = (consts.BitmapTypeToStrReverse if self.rev_byteorder else consts.BitmapTypeToStr)[self.format]
         AutoCloseable.__init__(self, pdfium_c.FPDFBitmap_Destroy, needs_free=needs_free, obj=self.buffer)
     
     
     @property
     def parent(self):  # AutoCloseable hook
         return None
```

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_helpers/document.py` & `pypdfium2-4.9.0/src/pypdfium2/_helpers/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -601,14 +601,16 @@
             kwargs (dict):
                 Keyword arguments to the renderer.
         
         Yields:
             :data:`typing.Any`: Parameter-dependent result.
         """
         
+        # TODO(v5) remove mk_formconfig parameter (bloat)
+        
         if not isinstance(self._input, (Path, str)):
             raise ValueError("Can only render in parallel with file path input.")
         
         n_pages = len(self)
         if not page_indices:
             page_indices = [i for i in range(n_pages)]
         else:
@@ -697,18 +699,18 @@
 
 def _open_pdf(input_data, password, autoclose):
     
     to_hold = ()
     to_close = ()
     
     if password is not None:
-        password = (password + "\x00").encode("utf-8")
+        password = (password+"\x00").encode("utf-8")
     
     if isinstance(input_data, Path):
-        pdf = pdfium_c.FPDF_LoadDocument((str(input_data) + "\x00").encode("utf-8"), password)
+        pdf = pdfium_c.FPDF_LoadDocument((str(input_data)+"\x00").encode("utf-8"), password)
     elif isinstance(input_data, (bytes, ctypes.Array)):
         pdf = pdfium_c.FPDF_LoadMemDocument64(input_data, len(input_data), password)
         to_hold = (input_data, )
     elif utils.is_buffer(input_data, "r"):
         bufaccess, to_hold = utils.get_bufreader(input_data)
         if autoclose:
             to_close = (input_data, )
```

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_helpers/matrix.py` & `pypdfium2-4.9.0/src/pypdfium2/_helpers/matrix.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_helpers/page.py` & `pypdfium2-4.9.0/src/pypdfium2/_helpers/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,14 +255,16 @@
             max_depth (int):
                 Maximum recursion depth to consider when descending into Form XObjects.
         
         Yields:
             :class:`.PdfObject`: A page object.
         """
         
+        # TODO? close skipped objects explicitly ?
+        
         if form:
             count_objects = pdfium_c.FPDFFormObj_CountObjects
             get_object = pdfium_c.FPDFFormObj_GetObject
             parent = form
         else:
             count_objects = pdfium_c.FPDFPage_CountObjects
             get_object = pdfium_c.FPDFPage_GetObject
```

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_helpers/pageobjects.py` & `pypdfium2-4.9.0/src/pypdfium2/_helpers/pageobjects.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,18 +69,16 @@
                 raise ValueError("*page* must belong to *pdf* when constructing a pageobject.")
         
         AutoCloseable.__init__(self, pdfium_c.FPDFPageObj_Destroy, needs_free=(page is None))
     
     
     @property
     def parent(self):  # AutoCloseable hook
-        if self.page is None:
-            return self.pdf  # may be none
-        else:
-            return self.page
+        # May be None (loose pageobject)
+        return self.pdf if self.page is None else self.page
     
     
     def get_pos(self):
         """
         Get the position of the object on the page.
         
         Returns:
@@ -130,14 +128,15 @@
 # In principle, we would like to move PdfImage to a separate file, but it's not that easy because of the two-fold connection with PdfObject, which would run us into a circular import. (However, what we could do is externalize the class under a different name and turn PdfImage into a wrapper which merely inherits from that class.)
 
 class PdfImage (PdfObject):
     """
     Image object helper class (specific kind of page object).
     """
     
+    # cf. https://crbug.com/pdfium/1203
     #: Filters applied by :func:`FPDFImageObj_GetImageDataDecoded`. Hereafter referred to as "simple filters", while non-simple filters will be called "complex filters".
     SIMPLE_FILTERS = ("ASCIIHexDecode", "ASCII85Decode", "RunLengthDecode", "FlateDecode", "LZWDecode")
     
     
     @classmethod
     def new(cls, pdf):
         """
@@ -282,25 +281,18 @@
         Parameters:
             decode_simple (bool):
                 If True, apply simple filters, resulting in semi-decoded data (see :attr:`.SIMPLE_FILTERS`).
                 Otherwise, the raw data will be returned.
         Returns:
             ctypes.Array: The data of the image stream (as :class:`~ctypes.c_ubyte` array).
         """
-        
-        if decode_simple:
-            # apply simple filters (see https://crbug.com/pdfium/1203 for description)
-            func = pdfium_c.FPDFImageObj_GetImageDataDecoded
-        else:
-            func = pdfium_c.FPDFImageObj_GetImageDataRaw
-        
+        func = pdfium_c.FPDFImageObj_GetImageDataDecoded if decode_simple else pdfium_c.FPDFImageObj_GetImageDataRaw
         n_bytes = func(self, None, 0)
         buffer = (ctypes.c_ubyte * n_bytes)()
         func(self, buffer, n_bytes)
-        
         return buffer
     
     
     def get_filters(self, skip_simple=False):
         """
         Parameters:
             skip_simple (bool):
@@ -345,16 +337,18 @@
         """
         
         # https://crbug.com/pdfium/1930
         
         extraction_gen = _extract_smart(self, *args, **kwargs)
         format = next(extraction_gen)
         
-        if isinstance(dest, (str, Path)):
-            with open(f"{dest}.{format}", "wb") as buf:
+        if isinstance(dest, str):
+            dest = Path(dest)
+        if isinstance(dest, Path):
+            with open(dest.with_suffix("."+format), "wb") as buf:
                 extraction_gen.send(buf)
         elif utils.is_buffer(dest, "w"):
             extraction_gen.send(dest)
         else:
             raise ValueError(f"Cannot extract to '{dest}'")
 
 
@@ -378,85 +372,63 @@
         return "CMYK"
     else:
         return None
 
 
 def _extract_smart(image_obj, fb_format=None, fb_render=False):
     
-    pil_image = None
-    data = None
-    info = None
+    # FIXME somewhat hard to read...
     
     try:
         data, info = _extract_direct(image_obj)
     except ImageNotExtractableError:
+        # TODO? log reason why the image cannot be extracted directly
         pil_image = image_obj.get_bitmap(render=fb_render).to_pil()
     else:
+        pil_image = None
         format = info.format
         if format == "raw":
             metadata = info.metadata
             pil_image = PIL.Image.frombuffer(
                 info.mode,
                 (metadata.width, metadata.height),
                 image_obj.get_data(decode_simple=True),
                 "raw", info.mode, 0, 1,
             )
     
     if pil_image:
-        if fb_format:
-            format = fb_format
-        elif pil_image.mode == "CMYK":
-            format = "tiff"
-        else:
-            format = "png"
+        format = fb_format if fb_format else "tiff" if pil_image.mode == "CMYK" else "png"
     
-    # provide format, receive buffer
     buffer = yield format
+    pil_image.save(buffer, format=format) if pil_image else buffer.write(data)
     
-    if pil_image:
-        pil_image.save(buffer, format=format)
-    else:
-        buffer.write(data)
-    
-    # breakpoint preventing StopIteration on send()
-    yield None
+    yield  # breakpoint preventing StopIteration on .send()
 
 
 def _extract_direct(image_obj):
     
     all_filters = image_obj.get_filters()
     complex_filters = [f for f in all_filters if f not in PdfImage.SIMPLE_FILTERS]
     metadata = image_obj.get_metadata()
     mode = _get_pil_mode(metadata.colorspace, metadata.bits_per_pixel)
     
-    out_data = None
-    out_format = None
-    
-    # Not sure if FlateDecode or LZWDecode data could be wrapped directly in an image file structure like PNG or TIFF
-    
     if len(complex_filters) == 0:
         if mode:
             out_data = image_obj.get_data(decode_simple=True)
             out_format = "raw"
         else:
-            raise ImageNotExtractableError(f"Unhandled color space {consts.ColorspaceToStr.get(metadata.colorspace)} - don't know how to treat data")
-    
+            raise ImageNotExtractableError(f"Unhandled color space {consts.ColorspaceToStr.get(metadata.colorspace)} - don't know how to treat data.")
     elif len(complex_filters) == 1:
         f = complex_filters[0]
         if f == "DCTDecode":
             out_data = image_obj.get_data(decode_simple=True)
             out_format = "jpg"
         elif f == "JPXDecode":
             out_data = image_obj.get_data(decode_simple=True)
             out_format = "jp2"
         else:
-            raise ImageNotExtractableError(f"Unhandled complex filter {f}")
-        
-        # Other complex filters:
-        # CCITTFaxDecode: In theory, could be extracted directly (with a TIFF header builder like pikepdf/models/_transcoding.py:generate_ccitt_header), but PDFium doesn't tell us which CCITT group encoding it is.
-        # JBIG2Decode: In PDF, JBIG2 header info is stripped, and global segments may be stored in a separate stream. In that form, the data would probably not be of much use, except perhaps for direct re-insertion into another PDF. We're not sure if it would be possible to re-combine this into a single JBIG2 file, or if any application could use this at all. PDFium doesn't provide us with the global segments, anyway.
-    
+            raise ImageNotExtractableError(f"Unhandled complex filter {f}.")
     else:
-        raise ImageNotExtractableError(f"Cannot handle multiple complex filters {complex_filters}")
+        raise ImageNotExtractableError(f"Cannot handle multiple complex filters {complex_filters}.")
     
     info = ImageInfo(out_format, mode, metadata, all_filters, complex_filters)
     return out_data, info
```

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_helpers/textpage.py` & `pypdfium2-4.9.0/src/pypdfium2/_helpers/textpage.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/_helpers/unsupported.py` & `pypdfium2-4.9.0/src/pypdfium2/_helpers/unsupported.py`

 * *Files identical despite different names*

### Comparing `pypdfium2-4.8.0/src/pypdfium2/version.py` & `pypdfium2-4.9.0/src/pypdfium2/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-FileCopyrightText: 2023 geisserml <geisserml@gmail.com>
 # SPDX-License-Identifier: Apache-2.0 OR BSD-3-Clause
 
 __all__ = ["V_PYPDFIUM2", "V_LIBPDFIUM", "V_BUILDNAME", "V_PDFIUM_IS_V8"]
 
 V_MAJOR = 4
-V_MINOR = 8
+V_MINOR = 9
 V_PATCH = 0
 V_BETA = None
 
 #: pypdfium2 version string
 V_PYPDFIUM2 = f"{V_MAJOR}.{V_MINOR}.{V_PATCH}"
 if V_BETA is not None:
     V_PYPDFIUM2 += f"b{V_BETA}"
 
 #: PDFium library version string (git tag or commit hash)
-V_LIBPDFIUM = "5731"
+V_LIBPDFIUM = "5744"
 
 #: String describing the included PDFium binary's origin (pdfium-binaries, source)
 V_BUILDNAME = "pdfium-binaries"
 
 #: Whether the included PDFium binary was built with V8 support or not
 V_PDFIUM_IS_V8 = False
```

### Comparing `pypdfium2-4.8.0/src/pypdfium2.egg-info/PKG-INFO` & `pypdfium2-4.9.0/src/pypdfium2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdfium2
-Version: 4.8.0
+Version: 4.9.0
 Summary: Python bindings to PDFium
 Author: pypdfium2-team
 Author-email: geisserml <geisserml@gmail.com>
 License: Apache-2.0 or BSD-3-Clause
 Project-URL: homepage, https://github.com/pypdfium2-team/pypdfium2
 Project-URL: documentation, https://pypdfium2.readthedocs.io/
 Project-URL: changelog, https://pypdfium2.readthedocs.io/en/stable/changelog.html
```

### Comparing `pypdfium2-4.8.0/src/pypdfium2.egg-info/SOURCES.txt` & `pypdfium2-4.9.0/src/pypdfium2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

