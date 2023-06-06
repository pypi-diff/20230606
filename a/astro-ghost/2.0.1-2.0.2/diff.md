# Comparing `tmp/astro_ghost-2.0.1.tar.gz` & `tmp/astro_ghost-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-2.0.1.tar", last modified: Sun Jun  4 03:58:04 2023, max compression
+gzip compressed data, was "astro_ghost-2.0.2.tar", last modified: Tue Jun  6 15:53:20 2023, max compression
```

## Comparing `astro_ghost-2.0.1.tar` & `astro_ghost-2.0.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.988061 astro_ghost-2.0.1/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.920248 astro_ghost-2.0.1/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.926281 astro_ghost-2.0.1/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      587 2023-05-24 04:50:38.000000 astro_ghost-2.0.1/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-04 03:58:04.988323 astro_ghost-2.0.1/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2023-05-24 04:49:23.000000 astro_ghost-2.0.1/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.965719 astro_ghost-2.0.1/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    21836 2023-06-04 03:47:53.000000 astro_ghost-2.0.1/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-22 16:28:50.000000 astro_ghost-2.0.1/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    38679 2023-05-22 16:28:56.000000 astro_ghost-2.0.1/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.1/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.1/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.1/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.1/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-06-04 03:56:11.000000 astro_ghost-2.0.1/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.1/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    39826 2023-05-23 03:25:58.000000 astro_ghost-2.0.1/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2023-06-04 03:48:08.000000 astro_ghost-2.0.1/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.1/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    17727 2023-05-22 03:39:53.000000 astro_ghost-2.0.1/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     9853 2023-05-22 16:28:44.000000 astro_ghost-2.0.1/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     7737 2023-05-24 04:44:13.000000 astro_ghost-2.0.1/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2023-05-24 04:43:14.000000 astro_ghost-2.0.1/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.1/astro_ghost/tonry_ps1_locus.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.969469 astro_ghost-2.0.1/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-04 03:58:04.000000 astro_ghost-2.0.1/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-06-04 03:58:04.000000 astro_ghost-2.0.1/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-04 03:58:04.000000 astro_ghost-2.0.1/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-04 03:58:04.000000 astro_ghost-2.0.1/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-06-04 03:58:04.000000 astro_ghost-2.0.1/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-06-04 03:58:04.000000 astro_ghost-2.0.1/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.972875 astro_ghost-2.0.1/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.1/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.1/docs/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.981314 astro_ghost-2.0.1/docs/source/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.1/docs/source/associationmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.1/docs/source/basicusage.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.1/docs/source/catalogmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.1/docs/source/detailedtutorials.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.1/docs/source/installation.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.1/docs/source/preprocessingmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.1/docs/source/supplementalmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.1/docs/source/wrappermodules.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.984071 astro_ghost-2.0.1/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.1/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-06-04 03:58:04.989543 astro_ghost-2.0.1/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-06-04 03:56:21.000000 astro_ghost-2.0.1/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-04 03:58:04.987136 astro_ghost-2.0.1/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.1/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.1/tests/debug.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.1/tests/pytest.ini
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4213 2023-05-22 05:37:16.000000 astro_ghost-2.0.1/tests/test_tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1391 2023-05-24 04:36:02.000000 astro_ghost-2.0.1/tox.ini
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:20.060965 astro_ghost-2.0.2/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:19.986346 astro_ghost-2.0.2/.github/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:19.993622 astro_ghost-2.0.2/.github/workflows/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      587 2023-05-24 04:50:38.000000 astro_ghost-2.0.2/.github/workflows/tests.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/.gitignore
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/.readthedocs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/MANIFEST.in
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-06 15:53:20.061173 astro_ghost-2.0.2/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2023-05-24 04:49:23.000000 astro_ghost-2.0.2/README.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:20.041456 astro_ghost-2.0.2/astro_ghost/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    21836 2023-06-04 03:47:53.000000 astro_ghost-2.0.2/astro_ghost/DLR.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-22 16:28:50.000000 astro_ghost-2.0.2/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    38694 2023-06-06 15:46:00.000000 astro_ghost-2.0.2/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.2/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.2/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.2/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.2/astro_ghost/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-06-06 15:51:38.000000 astro_ghost-2.0.2/astro_ghost/_version.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.2/astro_ghost/conftest.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    39826 2023-05-23 03:25:58.000000 astro_ghost-2.0.2/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2023-06-04 03:48:08.000000 astro_ghost-2.0.2/astro_ghost/gradientAscent.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.2/astro_ghost/hostMatching.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    17727 2023-05-22 03:39:53.000000 astro_ghost-2.0.2/astro_ghost/photoz_helper.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     9853 2023-05-22 16:28:44.000000 astro_ghost-2.0.2/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     7737 2023-05-24 04:44:13.000000 astro_ghost-2.0.2/astro_ghost/starSeparation.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2023-05-24 04:43:14.000000 astro_ghost-2.0.2/astro_ghost/stellarLocus.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.2/astro_ghost/tonry_ps1_locus.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:20.044081 astro_ghost-2.0.2/astro_ghost.egg-info/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-06 15:53:19.000000 astro_ghost-2.0.2/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-06-06 15:53:19.000000 astro_ghost-2.0.2/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-06 15:53:19.000000 astro_ghost-2.0.2/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-06 15:53:19.000000 astro_ghost-2.0.2/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-06-06 15:53:19.000000 astro_ghost-2.0.2/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-06-06 15:53:19.000000 astro_ghost-2.0.2/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:20.047686 astro_ghost-2.0.2/docs/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/docs/Makefile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.2/docs/conf.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.2/docs/index.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/docs/make.bat
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:20.055021 astro_ghost-2.0.2/docs/source/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.2/docs/source/associationmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.2/docs/source/basicusage.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.2/docs/source/catalogmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.2/docs/source/detailedtutorials.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.2/docs/source/installation.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.2/docs/source/preprocessingmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.2/docs/source/supplementalmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.2/docs/source/wrappermodules.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:20.057484 astro_ghost-2.0.2/licenses/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/licenses/LICENSE.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/licenses/README.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/pyproject.toml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-06-06 15:53:20.062137 astro_ghost-2.0.2/setup.cfg
+-rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-06-06 15:51:48.000000 astro_ghost-2.0.2/setup.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:20.060125 astro_ghost-2.0.2/tests/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.2/tests/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.2/tests/debug.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.2/tests/pytest.ini
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4213 2023-05-22 05:37:16.000000 astro_ghost-2.0.2/tests/test_tutorial.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1391 2023-05-24 04:36:02.000000 astro_ghost-2.0.2/tox.ini
```

### Comparing `astro_ghost-2.0.1/.github/workflows/tests.yml` & `astro_ghost-2.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/.gitignore` & `astro_ghost-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/PKG-INFO` & `astro_ghost-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_ghost
-Version: 2.0.1
+Version: 2.0.2
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-2.0.1/README.rst` & `astro_ghost-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/astro_ghost/DLR.py` & `astro_ghost-2.0.2/astro_ghost/DLR.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-2.0.2/astro_ghost/NEDQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-2.0.2/astro_ghost/PS1QueryFunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,30 +378,30 @@
         objDec = resolvedObject['resolvedCoordinate'][0]['decl']
     except IndexError as e:
         raise ValueError("Unknown object '{}'".format(name))
     return (objRa, objDec)
 
 def checklegal(table,release):
     """Checks if this combination of table and release is acceptable.
-       Raises a VelueError exception if there is problem.
+       Raises a ValueError exception if there is problem.
 
     :param table: Table type. Can be \\'mean\\', \\'stack\\', or \\'detection\\'
     :type table: str
     :param release: The Pan-STARRS data release. Can be \\'dr1\\' or \\'dr2\\'.
     :type release: str
     :raises ValueError: Raises error if table and release combination are invalid.
     """
 
     releaselist = ("dr1", "dr2")
     if release not in ("dr1","dr2"):
         raise ValueError("Bad value for release (must be one of {})".format(', '.join(releaselist)))
     if release=="dr1":
         tablelist = ("mean", "stack")
     else:
-        tablelist = ("mean", "stack", "detection")
+        tablelist = ("mean", "stack", "detection", "forced_mean")
     if table not in tablelist:
         raise ValueError("Bad value for table (for {} must be one of {})".format(release, ", ".join(tablelist)))
 
 def ps1search(table="mean",release="dr1",format="csv",columns=None,baseurl="https://catalogs.mast.stsci.edu/api/v0.1/panstarrs", verbose=False,**kw):
     """Do a general search of the PS1 catalog (possibly without ra/dec/radius).
 
     :param table: Table type. Can be \\'mean\\', \\'stack\\', or \\'detection\\'
```

### Comparing `astro_ghost-2.0.1/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-2.0.2/astro_ghost/SimbadQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-2.0.2/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/astro_ghost/TNSQueryFunctions.py` & `astro_ghost-2.0.2/astro_ghost/TNSQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/astro_ghost/conftest.py` & `astro_ghost-2.0.2/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-2.0.2/astro_ghost/ghostHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/astro_ghost/gradientAscent.py` & `astro_ghost-2.0.2/astro_ghost/gradientAscent.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/astro_ghost/hostMatching.py` & `astro_ghost-2.0.2/astro_ghost/hostMatching.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/astro_ghost/photoz_helper.py` & `astro_ghost-2.0.2/astro_ghost/photoz_helper.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/astro_ghost/sourceCleaning.py` & `astro_ghost-2.0.2/astro_ghost/sourceCleaning.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/astro_ghost/starSeparation.py` & `astro_ghost-2.0.2/astro_ghost/starSeparation.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/astro_ghost/stellarLocus.py` & `astro_ghost-2.0.2/astro_ghost/stellarLocus.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/astro_ghost.egg-info/PKG-INFO` & `astro_ghost-2.0.2/astro_ghost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-ghost
-Version: 2.0.1
+Version: 2.0.2
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-2.0.1/astro_ghost.egg-info/SOURCES.txt` & `astro_ghost-2.0.2/astro_ghost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/docs/Makefile` & `astro_ghost-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/docs/conf.py` & `astro_ghost-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/docs/index.rst` & `astro_ghost-2.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/docs/make.bat` & `astro_ghost-2.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/docs/source/associationmodules.rst` & `astro_ghost-2.0.2/docs/source/associationmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/docs/source/basicusage.rst` & `astro_ghost-2.0.2/docs/source/basicusage.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/docs/source/catalogmodules.rst` & `astro_ghost-2.0.2/docs/source/catalogmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/docs/source/installation.rst` & `astro_ghost-2.0.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/docs/source/preprocessingmodules.rst` & `astro_ghost-2.0.2/docs/source/preprocessingmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/licenses/LICENSE.rst` & `astro_ghost-2.0.2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/setup.cfg` & `astro_ghost-2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/setup.py` & `astro_ghost-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 from setuptools import setup
 
-version = "2.0.1"
+version = "2.0.2"
 
 VERSION_TEMPLATE = """
  Note that we need to fall back to the hard-coded version if either
  setuptools_scm can't be imported or setuptools_scm can't determine the
  version, so we catch the generic 'Exception'.
 __version__ = '{version}'
 """.lstrip()
```

### Comparing `astro_ghost-2.0.1/tests/debug.py` & `astro_ghost-2.0.2/tests/debug.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/tests/test_tutorial.py` & `astro_ghost-2.0.2/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.1/tox.ini` & `astro_ghost-2.0.2/tox.ini`

 * *Files identical despite different names*

