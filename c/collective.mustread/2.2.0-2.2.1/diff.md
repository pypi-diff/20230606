# Comparing `tmp/collective.mustread-2.2.0.tar.gz` & `tmp/collective.mustread-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.mustread-2.2.0.tar", last modified: Tue Oct  4 15:26:46 2022, max compression
+gzip compressed data, was "collective.mustread-2.2.1.tar", last modified: Tue Jun  6 15:07:37 2023, max compression
```

## Comparing `collective.mustread-2.2.0.tar` & `collective.mustread-2.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.900880 collective.mustread-2.2.0/
--rw-rw-r--   0 ale       (1000) ale       (1000)     1554 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/CHANGES.rst
--rw-rw-r--   0 ale       (1000) ale       (1000)      121 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/CONTRIBUTORS.rst
--rw-rw-r--   0 ale       (1000) ale       (1000)       97 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/MANIFEST.in
--rw-rw-r--   0 ale       (1000) ale       (1000)      173 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/Makefile
--rw-rw-r--   0 ale       (1000) ale       (1000)     9538 2022-10-04 15:26:46.900880 collective.mustread-2.2.0/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     7032 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/README.rst
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.896880 collective.mustread-2.2.0/docs/
--rw-rw-r--   0 ale       (1000) ale       (1000)    18092 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/docs/LICENSE.GPL
--rw-rw-r--   0 ale       (1000) ale       (1000)      668 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/docs/LICENSE.rst
--rw-rw-r--   0 ale       (1000) ale       (1000)       82 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/docs/index.rst
--rw-rw-r--   0 ale       (1000) ale       (1000)       62 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/requirements.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)      270 2022-10-04 15:26:46.900880 collective.mustread-2.2.0/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     1897 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/setup.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.896880 collective.mustread-2.2.0/src/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.896880 collective.mustread-2.2.0/src/collective/
--rw-rw-r--   0 ale       (1000) ale       (1000)       80 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.900880 collective.mustread-2.2.0/src/collective/mustread/
--rw-rw-r--   0 ale       (1000) ale       (1000)      137 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.900880 collective.mustread-2.2.0/src/collective/mustread/behaviors/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/behaviors/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      899 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/behaviors/configure.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)      612 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/behaviors/maybe.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1483 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/behaviors/track.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.900880 collective.mustread-2.2.0/src/collective/mustread/browser/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/browser/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      829 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/browser/configure.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)     1764 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/browser/init_db.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      631 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/browser/views.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1148 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/configure.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)     2945 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/db.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    14431 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/interfaces.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.900880 collective.mustread-2.2.0/src/collective/mustread/locales/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/locales/collective.mustread.pot
--rwxrwxr-x   0 ale       (1000) ale       (1000)      494 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/locales/update.sh
--rw-rw-r--   0 ale       (1000) ale       (1000)      763 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/models.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.896880 collective.mustread-2.2.0/src/collective/mustread/profiles/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.900880 collective.mustread-2.2.0/src/collective/mustread/profiles/default/
--rw-rw-r--   0 ale       (1000) ale       (1000)      183 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/profiles/default/browserlayer.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      123 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/profiles/default/metadata.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      120 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/profiles/default/registry.xml
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.900880 collective.mustread-2.2.0/src/collective/mustread/profiles/uninstall/
--rw-rw-r--   0 ale       (1000) ale       (1000)      129 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      687 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/setuphandlers.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4092 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/td.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4574 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/testing.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.900880 collective.mustread-2.2.0/src/collective/mustread/tests/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/tests/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.900880 collective.mustread-2.2.0/src/collective/mustread/tests/robot/
--rw-rw-r--   0 ale       (1000) ale       (1000)     2007 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/tests/robot/test_example.robot
--rw-rw-r--   0 ale       (1000) ale       (1000)     2052 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/tests/test_behaviors.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      571 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/tests/test_hit.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      878 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/tests/test_robot.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1829 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/tests/test_setup.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    23096 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/tests/test_tracker.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1079 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/tests/test_upgrades.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    10128 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/tracker.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.900880 collective.mustread-2.2.0/src/collective/mustread/upgrades/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/upgrades/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      891 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/upgrades/configure.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)     1825 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/upgrades/to1001.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1111 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/upgrades/to1002.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      433 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective/mustread/utils.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2022-10-04 15:26:46.896880 collective.mustread-2.2.0/src/collective.mustread.egg-info/
--rw-rw-r--   0 ale       (1000) ale       (1000)     9538 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective.mustread.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     2136 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective.mustread.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective.mustread.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)       40 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective.mustread.egg-info/entry_points.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)       11 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective.mustread.egg-info/namespace_packages.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective.mustread.egg-info/not-zip-safe
--rw-rw-r--   0 ale       (1000) ale       (1000)      206 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective.mustread.egg-info/requires.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)       11 2022-10-04 15:26:46.000000 collective.mustread-2.2.0/src/collective.mustread.egg-info/top_level.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.643827 collective.mustread-2.2.1/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1621 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/CHANGES.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)      121 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/CONTRIBUTORS.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)       97 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/MANIFEST.in
+-rw-rw-r--   0 ale       (1000) ale       (1000)      173 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/Makefile
+-rw-rw-r--   0 ale       (1000) ale       (1000)     9655 2023-06-06 15:07:37.643827 collective.mustread-2.2.1/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7032 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/README.rst
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.643827 collective.mustread-2.2.1/docs/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    18092 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/docs/LICENSE.GPL
+-rw-rw-r--   0 ale       (1000) ale       (1000)      668 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/docs/LICENSE.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)       82 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/docs/index.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)       62 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/requirements.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      270 2023-06-06 15:07:37.647827 collective.mustread-2.2.1/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1946 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/setup.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.639827 collective.mustread-2.2.1/src/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.643827 collective.mustread-2.2.1/src/collective/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       80 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.643827 collective.mustread-2.2.1/src/collective/mustread/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      137 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.643827 collective.mustread-2.2.1/src/collective/mustread/behaviors/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/behaviors/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      899 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/behaviors/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      612 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/behaviors/maybe.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1483 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/behaviors/track.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.643827 collective.mustread-2.2.1/src/collective/mustread/browser/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/browser/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      829 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/browser/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1764 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/browser/init_db.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      631 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/browser/views.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1148 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2945 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/db.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    14431 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/interfaces.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.643827 collective.mustread-2.2.1/src/collective/mustread/locales/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/locales/collective.mustread.pot
+-rwxrwxr-x   0 ale       (1000) ale       (1000)      494 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/locales/update.sh
+-rw-rw-r--   0 ale       (1000) ale       (1000)      763 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/models.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.639827 collective.mustread-2.2.1/src/collective/mustread/profiles/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.643827 collective.mustread-2.2.1/src/collective/mustread/profiles/default/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      183 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/profiles/default/browserlayer.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      123 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/profiles/default/metadata.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      120 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/profiles/default/registry.xml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.643827 collective.mustread-2.2.1/src/collective/mustread/profiles/uninstall/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      129 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      687 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/setuphandlers.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4092 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/td.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4574 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/testing.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.643827 collective.mustread-2.2.1/src/collective/mustread/tests/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/tests/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.643827 collective.mustread-2.2.1/src/collective/mustread/tests/robot/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2007 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/tests/robot/test_example.robot
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2052 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/tests/test_behaviors.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      571 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/tests/test_hit.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      878 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/tests/test_robot.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1829 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/tests/test_setup.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    23096 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/tests/test_tracker.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1079 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/tests/test_upgrades.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    10337 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/tracker.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.643827 collective.mustread-2.2.1/src/collective/mustread/upgrades/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/upgrades/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      891 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/upgrades/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1825 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/upgrades/to1001.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1111 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/upgrades/to1002.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      433 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective/mustread/utils.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-06 15:07:37.643827 collective.mustread-2.2.1/src/collective.mustread.egg-info/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     9655 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective.mustread.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2136 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective.mustread.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective.mustread.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       40 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective.mustread.egg-info/entry_points.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       11 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective.mustread.egg-info/namespace_packages.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective.mustread.egg-info/not-zip-safe
+-rw-rw-r--   0 ale       (1000) ale       (1000)      206 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective.mustread.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       11 2023-06-06 15:07:37.000000 collective.mustread-2.2.1/src/collective.mustread.egg-info/top_level.txt
```

### Comparing `collective.mustread-2.2.0/CHANGES.rst` & `collective.mustread-2.2.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog
 =========
 
 
+2.2.1 (2023-06-06)
+------------------
+
+- Remove deprecated code.
+
+
 2.2.0 (2022-10-04)
 ------------------
 
 - Make the test pass on Plone6
 
 
 2.1.0 (2022-08-05)
```

### Comparing `collective.mustread-2.2.0/PKG-INFO` & `collective.mustread-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.mustread
-Version: 2.2.0
+Version: 2.2.1
 Summary: Tracking user views on content items marked as must-read
 Home-page: https://pypi.org/project/collective.mustread/
 Author: Guido A.J. Stevens
 Author-email: guido.stevens@cosent.net
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Environment :: Web Environment
@@ -12,14 +12,15 @@
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.1
 Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Provides-Extra: test
 
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
@@ -214,14 +215,20 @@
 
 - Harald Friessnegger, harald@webmeisterei.com
 
 Changelog
 =========
 
 
+2.2.1 (2023-06-06)
+------------------
+
+- Remove deprecated code.
+
+
 2.2.0 (2022-10-04)
 ------------------
 
 - Make the test pass on Plone6
 
 
 2.1.0 (2022-08-05)
```

### Comparing `collective.mustread-2.2.0/README.rst` & `collective.mustread-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/docs/LICENSE.GPL` & `collective.mustread-2.2.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/docs/LICENSE.rst` & `collective.mustread-2.2.1/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/setup.py` & `collective.mustread-2.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,29 @@
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='collective.mustread',
-    version='2.2.0',
+    version='2.2.1',
     description="Tracking user views on content items marked as must-read",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
         "Framework :: Plone :: 5.1",
         "Framework :: Plone :: 5.2",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords='Python Plone',
     author='Guido A.J. Stevens',
     author_email='guido.stevens@cosent.net',
     url='https://pypi.org/project/collective.mustread/',
```

### Comparing `collective.mustread-2.2.0/src/collective/mustread/behaviors/configure.zcml` & `collective.mustread-2.2.1/src/collective/mustread/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/behaviors/maybe.py` & `collective.mustread-2.2.1/src/collective/mustread/behaviors/maybe.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/behaviors/track.py` & `collective.mustread-2.2.1/src/collective/mustread/behaviors/track.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/browser/configure.zcml` & `collective.mustread-2.2.1/src/collective/mustread/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/browser/init_db.py` & `collective.mustread-2.2.1/src/collective/mustread/browser/init_db.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/browser/views.py` & `collective.mustread-2.2.1/src/collective/mustread/browser/views.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/configure.zcml` & `collective.mustread-2.2.1/src/collective/mustread/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/db.py` & `collective.mustread-2.2.1/src/collective/mustread/db.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/interfaces.py` & `collective.mustread-2.2.1/src/collective/mustread/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/models.py` & `collective.mustread-2.2.1/src/collective/mustread/models.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/setuphandlers.py` & `collective.mustread-2.2.1/src/collective/mustread/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/td.py` & `collective.mustread-2.2.1/src/collective/mustread/td.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/testing.py` & `collective.mustread-2.2.1/src/collective/mustread/testing.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/tests/robot/test_example.robot` & `collective.mustread-2.2.1/src/collective/mustread/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/tests/test_behaviors.py` & `collective.mustread-2.2.1/src/collective/mustread/tests/test_behaviors.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/tests/test_hit.py` & `collective.mustread-2.2.1/src/collective/mustread/tests/test_hit.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/tests/test_robot.py` & `collective.mustread-2.2.1/src/collective/mustread/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/tests/test_setup.py` & `collective.mustread-2.2.1/src/collective/mustread/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/tests/test_tracker.py` & `collective.mustread-2.2.1/src/collective/mustread/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/tests/test_upgrades.py` & `collective.mustread-2.2.1/src/collective/mustread/tests/test_upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/tracker.py` & `collective.mustread-2.2.1/src/collective/mustread/tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,33 @@
 from collective.mustread import td
 from collective.mustread import utils
 from collective.mustread.interfaces import ITracker
 from collective.mustread.models import MustRead
 from datetime import datetime
 from datetime import timedelta
 from plone import api
-from Products.CMFPlone.utils import safe_unicode
 from sqlalchemy import func
 from sqlalchemy import or_
 from zope.globalrequest import getRequest
 from zope.interface import implementer
 
 import csv
 import logging
 
+try:
+    from plone.base.utils import safe_text
+except ImportError:
+    try:
+        # Plone 5.2
+        from Products.CMFPlone.utils import safe_text
+    except ImportError:
+        # Plone 5.1
+        from Products.CMFPlone.utils import safe_unicode as safe_text
+
+
 
 log = logging.getLogger(__name__)
 
 
 @implementer(ITracker)
 class Tracker(object):
     '''
@@ -170,15 +180,15 @@
 
         path = '/'.join(api.portal.get().getPhysicalPath())
         if context is not None:
             path = '/'.join(context.getPhysicalPath())
         query = query.filter(MustRead.path.startswith(path))
 
         if userid is not None:
-            query = query.filter(MustRead.userid == safe_unicode(userid))
+            query = query.filter(MustRead.userid == safe_text(userid))
         if deadline_before:
             query = query.filter(MustRead.deadline < deadline_before)
         query = query.order_by(MustRead.path)
         uids = [r[0] for r in self.query_all(query)]
         result = []
         for uid in uids:
             obj = api.content.get(UID=uid)
@@ -216,15 +226,15 @@
 
         if start_date:
             query = query.filter(or_(
                 MustRead.scheduled_at >= start_date.date(),
                 MustRead.read_at >= start_date.date()))
 
         if userid:
-            query = query.filter(MustRead.userid == safe_unicode(userid))
+            query = query.filter(MustRead.userid == safe_text(userid))
         if include_children:
             query = query.filter(MustRead.path.startswith(path))
         else:
             query = query.filter(MustRead.path == path)
 
         query = query.order_by(MustRead.path)
 
@@ -285,9 +295,9 @@
             tdata.register(session)
         return session
 
     def _safe_unicode(self, **data):
         for key in data:
             value = data[key]
             if isinstance(value, str):
-                data[key] = safe_unicode(value)
+                data[key] = safe_text(value)
         return data
```

### Comparing `collective.mustread-2.2.0/src/collective/mustread/upgrades/configure.zcml` & `collective.mustread-2.2.1/src/collective/mustread/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/upgrades/to1001.py` & `collective.mustread-2.2.1/src/collective/mustread/upgrades/to1001.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective/mustread/upgrades/to1002.py` & `collective.mustread-2.2.1/src/collective/mustread/upgrades/to1002.py`

 * *Files identical despite different names*

### Comparing `collective.mustread-2.2.0/src/collective.mustread.egg-info/PKG-INFO` & `collective.mustread-2.2.1/src/collective.mustread.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.mustread
-Version: 2.2.0
+Version: 2.2.1
 Summary: Tracking user views on content items marked as must-read
 Home-page: https://pypi.org/project/collective.mustread/
 Author: Guido A.J. Stevens
 Author-email: guido.stevens@cosent.net
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Environment :: Web Environment
@@ -12,14 +12,15 @@
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.1
 Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Provides-Extra: test
 
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
@@ -214,14 +215,20 @@
 
 - Harald Friessnegger, harald@webmeisterei.com
 
 Changelog
 =========
 
 
+2.2.1 (2023-06-06)
+------------------
+
+- Remove deprecated code.
+
+
 2.2.0 (2022-10-04)
 ------------------
 
 - Make the test pass on Plone6
 
 
 2.1.0 (2022-08-05)
```

### Comparing `collective.mustread-2.2.0/src/collective.mustread.egg-info/SOURCES.txt` & `collective.mustread-2.2.1/src/collective.mustread.egg-info/SOURCES.txt`

 * *Files identical despite different names*

