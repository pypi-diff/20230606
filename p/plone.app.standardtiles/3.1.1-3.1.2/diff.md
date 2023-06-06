# Comparing `tmp/plone.app.standardtiles-3.1.1.tar.gz` & `tmp/plone.app.standardtiles-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.standardtiles-3.1.1.tar", last modified: Sat May 13 13:33:39 2023, max compression
+gzip compressed data, was "plone.app.standardtiles-3.1.2.tar", last modified: Tue Jun  6 09:30:48 2023, max compression
```

## Comparing `plone.app.standardtiles-3.1.1.tar` & `plone.app.standardtiles-3.1.2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-13 13:33:39.926773 plone.app.standardtiles-3.1.1/
--rw-r--r--   0 peterm     (501) staff       (20)    11029 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/CHANGES.rst
--rw-r--r--   0 peterm     (501) staff       (20)    12282 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/LICENSE.GPL
--rw-r--r--   0 peterm     (501) staff       (20)      750 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/LICENSE.txt
--rw-r--r--   0 peterm     (501) staff       (20)    13196 2023-05-13 13:33:39.926446 plone.app.standardtiles-3.1.1/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)     1061 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/README.rst
--rw-r--r--   0 peterm     (501) staff       (20)     2858 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/pyproject.toml
--rw-r--r--   0 peterm     (501) staff       (20)       38 2023-05-13 13:33:39.926844 plone.app.standardtiles-3.1.1/setup.cfg
--rw-r--r--   0 peterm     (501) staff       (20)     1992 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/setup.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-13 13:33:39.896553 plone.app.standardtiles-3.1.1/src/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-13 13:33:39.899836 plone.app.standardtiles-3.1.1/src/plone/
--rw-r--r--   0 peterm     (501) staff       (20)       56 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-13 13:33:39.902686 plone.app.standardtiles-3.1.1/src/plone/app/
--rw-r--r--   0 peterm     (501) staff       (20)       56 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-13 13:33:39.911808 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/
--rw-r--r--   0 peterm     (501) staff       (20)      122 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)     3763 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/attachment.py
--rw-r--r--   0 peterm     (501) staff       (20)    11182 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/common.py
--rw-r--r--   0 peterm     (501) staff       (20)     4184 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     5249 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/content.zcml
--rw-r--r--   0 peterm     (501) staff       (20)    10594 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/contentlisting.py
--rw-r--r--   0 peterm     (501) staff       (20)     2330 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/discussion.py
--rw-r--r--   0 peterm     (501) staff       (20)      739 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/embed.py
--rw-r--r--   0 peterm     (501) staff       (20)     8603 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/existingcontent.py
--rw-r--r--   0 peterm     (501) staff       (20)     5775 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/field.py
--rw-r--r--   0 peterm     (501) staff       (20)     2182 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/head.py
--rw-r--r--   0 peterm     (501) staff       (20)     1909 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/head.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     1425 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/html.py
--rw-r--r--   0 peterm     (501) staff       (20)      587 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/interfaces.py
--rw-r--r--   0 peterm     (501) staff       (20)     4359 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/layout.zcml
--rw-r--r--   0 peterm     (501) staff       (20)      981 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/linkintegrity.py
--rw-r--r--   0 peterm     (501) staff       (20)     1688 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/media.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     1361 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/metadata.py
--rw-r--r--   0 peterm     (501) staff       (20)    11827 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/navigation.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-13 13:33:39.914939 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/
--rw-r--r--   0 peterm     (501) staff       (20)        0 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)     3940 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/add.py
--rw-r--r--   0 peterm     (501) staff       (20)     1968 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/assignment.py
--rw-r--r--   0 peterm     (501) staff       (20)     2563 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)      317 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/delete.py
--rw-r--r--   0 peterm     (501) staff       (20)     1151 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/edit.py
--rw-r--r--   0 peterm     (501) staff       (20)     2298 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/portlet.py
--rw-r--r--   0 peterm     (501) staff       (20)     1799 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/portletmanager.py
--rw-r--r--   0 peterm     (501) staff       (20)     1970 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/utils.py
--rw-r--r--   0 peterm     (501) staff       (20)     1720 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/vocabularies.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-13 13:33:39.897381 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/profiles/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-13 13:33:39.916026 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/profiles/default/
--rw-r--r--   0 peterm     (501) staff       (20)      184 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/profiles/default/metadata.xml
--rw-r--r--   0 peterm     (501) staff       (20)      207 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/profiles/default/portlets.xml
--rw-r--r--   0 peterm     (501) staff       (20)     4557 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/profiles/default/registry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-13 13:33:39.916651 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/profiles/uninstall/
--rw-r--r--   0 peterm     (501) staff       (20)      239 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/profiles/uninstall/portlets..xml
--rw-r--r--   0 peterm     (501) staff       (20)      146 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/profiles/uninstall/registry.xml
--rw-r--r--   0 peterm     (501) staff       (20)     1382 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/rawembed.py
--rw-r--r--   0 peterm     (501) staff       (20)     8427 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/rss.py
--rw-r--r--   0 peterm     (501) staff       (20)      780 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/setuphandlers.py
--rw-r--r--   0 peterm     (501) staff       (20)     1000 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/sitemap.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-13 13:33:39.922479 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/
--rw-r--r--   0 peterm     (501) staff       (20)     1914 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/attachment_listing.pt
--rw-r--r--   0 peterm     (501) staff       (20)     2538 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/configlets.pt
--rw-r--r--   0 peterm     (501) staff       (20)      744 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/contentlisting_view.pt
--rw-r--r--   0 peterm     (501) staff       (20)      463 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/description.pt
--rw-r--r--   0 peterm     (501) staff       (20)     4337 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/existingcontent_view.pt
--rw-r--r--   0 peterm     (501) staff       (20)      771 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/image.pt
--rw-r--r--   0 peterm     (501) staff       (20)     3944 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/listing_view.pt
--rw-r--r--   0 peterm     (501) staff       (20)     6694 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/login.pt
--rw-r--r--   0 peterm     (501) staff       (20)     1254 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/namedimage.pt
--rw-r--r--   0 peterm     (501) staff       (20)     1675 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/navigation.pt
--rw-r--r--   0 peterm     (501) staff       (20)     2369 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/navigation_recurse.pt
--rw-r--r--   0 peterm     (501) staff       (20)      764 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/navigationlink.pt
--rw-r--r--   0 peterm     (501) staff       (20)      829 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/rawembed.pt
--rw-r--r--   0 peterm     (501) staff       (20)     1953 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/rss.pt
--rw-r--r--   0 peterm     (501) staff       (20)     6195 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/summary_view.pt
--rw-r--r--   0 peterm     (501) staff       (20)     4629 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/tabular_view.pt
--rw-r--r--   0 peterm     (501) staff       (20)      374 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/title.pt
--rw-r--r--   0 peterm     (501) staff       (20)     9746 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/testing.py
--rw-r--r--   0 peterm     (501) staff       (20)      698 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/testing.zcml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-13 13:33:39.926094 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/
--rw-r--r--   0 peterm     (501) staff       (20)     2921 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/RSS.xml
--rw-r--r--   0 peterm     (501) staff       (20)        0 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)      819 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt
--rw-r--r--   0 peterm     (501) staff       (20)      743 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/funky_display.pt
--rw-r--r--   0 peterm     (501) staff       (20)     7293 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/test_content.py
--rw-r--r--   0 peterm     (501) staff       (20)    14645 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/test_existing_content.py
--rw-r--r--   0 peterm     (501) staff       (20)    10979 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/test_field.py
--rw-r--r--   0 peterm     (501) staff       (20)     6241 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/test_head.py
--rw-r--r--   0 peterm     (501) staff       (20)    15107 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/test_layout.py
--rw-r--r--   0 peterm     (501) staff       (20)     7302 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/test_media.py
--rw-r--r--   0 peterm     (501) staff       (20)     1625 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/test_setup.py
--rw-r--r--   0 peterm     (501) staff       (20)      272 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/upgrades.py
--rw-r--r--   0 peterm     (501) staff       (20)      746 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/upgrades.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     1854 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/utils.py
--rw-r--r--   0 peterm     (501) staff       (20)     2488 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/viewletmanager.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-05-13 13:33:39.902356 plone.app.standardtiles-3.1.1/src/plone.app.standardtiles.egg-info/
--rw-r--r--   0 peterm     (501) staff       (20)    13196 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone.app.standardtiles.egg-info/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)     3957 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone.app.standardtiles.egg-info/SOURCES.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone.app.standardtiles.egg-info/dependency_links.txt
--rw-r--r--   0 peterm     (501) staff       (20)       40 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone.app.standardtiles.egg-info/entry_points.txt
--rw-r--r--   0 peterm     (501) staff       (20)       16 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone.app.standardtiles.egg-info/namespace_packages.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone.app.standardtiles.egg-info/not-zip-safe
--rw-r--r--   0 peterm     (501) staff       (20)      257 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone.app.standardtiles.egg-info/requires.txt
--rw-r--r--   0 peterm     (501) staff       (20)        6 2023-05-13 13:33:39.000000 plone.app.standardtiles-3.1.1/src/plone.app.standardtiles.egg-info/top_level.txt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.083565 plone.app.standardtiles-3.1.2/
+-rw-r--r--   0 peterm     (501) staff       (20)    11149 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/CHANGES.rst
+-rw-r--r--   0 peterm     (501) staff       (20)    12282 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/LICENSE.GPL
+-rw-r--r--   0 peterm     (501) staff       (20)      750 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/LICENSE.txt
+-rw-r--r--   0 peterm     (501) staff       (20)    13316 2023-06-06 09:30:48.083404 plone.app.standardtiles-3.1.2/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     1061 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/README.rst
+-rw-r--r--   0 peterm     (501) staff       (20)     2858 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/pyproject.toml
+-rw-r--r--   0 peterm     (501) staff       (20)       38 2023-06-06 09:30:48.083601 plone.app.standardtiles-3.1.2/setup.cfg
+-rw-r--r--   0 peterm     (501) staff       (20)     1992 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/setup.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.071757 plone.app.standardtiles-3.1.2/src/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.073222 plone.app.standardtiles-3.1.2/src/plone/
+-rw-r--r--   0 peterm     (501) staff       (20)       56 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.074312 plone.app.standardtiles-3.1.2/src/plone/app/
+-rw-r--r--   0 peterm     (501) staff       (20)       56 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.078128 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/
+-rw-r--r--   0 peterm     (501) staff       (20)      122 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     3763 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/attachment.py
+-rw-r--r--   0 peterm     (501) staff       (20)    11182 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/common.py
+-rw-r--r--   0 peterm     (501) staff       (20)     4184 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     5249 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/content.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)    10600 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/contentlisting.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2330 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/discussion.py
+-rw-r--r--   0 peterm     (501) staff       (20)      739 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/embed.py
+-rw-r--r--   0 peterm     (501) staff       (20)     8603 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/existingcontent.py
+-rw-r--r--   0 peterm     (501) staff       (20)     5775 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/field.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2182 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/head.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1909 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/head.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1425 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/html.py
+-rw-r--r--   0 peterm     (501) staff       (20)      587 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/interfaces.py
+-rw-r--r--   0 peterm     (501) staff       (20)     4359 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/layout.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)      981 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/linkintegrity.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1688 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/media.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1361 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/metadata.py
+-rw-r--r--   0 peterm     (501) staff       (20)    11827 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/navigation.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.079306 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     3940 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/add.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1968 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/assignment.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2563 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)      317 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/delete.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1151 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/edit.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2298 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/portlet.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1799 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/portletmanager.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1970 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/utils.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1720 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/vocabularies.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.072173 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.079659 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/default/
+-rw-r--r--   0 peterm     (501) staff       (20)      184 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/default/metadata.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      207 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/default/portlets.xml
+-rw-r--r--   0 peterm     (501) staff       (20)     4557 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/default/registry.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.079895 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/uninstall/
+-rw-r--r--   0 peterm     (501) staff       (20)      239 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/uninstall/portlets..xml
+-rw-r--r--   0 peterm     (501) staff       (20)      146 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/uninstall/registry.xml
+-rw-r--r--   0 peterm     (501) staff       (20)     1382 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/rawembed.py
+-rw-r--r--   0 peterm     (501) staff       (20)     8427 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/rss.py
+-rw-r--r--   0 peterm     (501) staff       (20)      780 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/setuphandlers.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1000 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/sitemap.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.081903 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/
+-rw-r--r--   0 peterm     (501) staff       (20)     1914 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/attachment_listing.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     2538 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/configlets.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      744 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/contentlisting_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      463 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/description.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     4337 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/existingcontent_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      771 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/image.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     3944 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/listing_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     6694 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/login.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     1254 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/namedimage.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     1675 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/navigation.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     2369 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/navigation_recurse.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      764 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/navigationlink.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      829 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/rawembed.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     1953 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/rss.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     6195 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/summary_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     4629 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/tabular_view.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      374 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/title.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     9746 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/testing.py
+-rw-r--r--   0 peterm     (501) staff       (20)      698 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/testing.zcml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.083222 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/
+-rw-r--r--   0 peterm     (501) staff       (20)     2921 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/RSS.xml
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)      819 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      743 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/funky_display.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     7293 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_content.py
+-rw-r--r--   0 peterm     (501) staff       (20)    14645 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_existing_content.py
+-rw-r--r--   0 peterm     (501) staff       (20)    10979 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_field.py
+-rw-r--r--   0 peterm     (501) staff       (20)     6241 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_head.py
+-rw-r--r--   0 peterm     (501) staff       (20)    15107 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_layout.py
+-rw-r--r--   0 peterm     (501) staff       (20)     7302 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_media.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1625 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_setup.py
+-rw-r--r--   0 peterm     (501) staff       (20)      272 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/upgrades.py
+-rw-r--r--   0 peterm     (501) staff       (20)      746 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/upgrades.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1854 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/utils.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2488 2023-06-06 09:30:47.000000 plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/viewletmanager.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-06-06 09:30:48.074195 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/
+-rw-r--r--   0 peterm     (501) staff       (20)    13316 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     3957 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/SOURCES.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/dependency_links.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       40 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/entry_points.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       16 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/namespace_packages.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/not-zip-safe
+-rw-r--r--   0 peterm     (501) staff       (20)      257 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/requires.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        6 2023-06-06 09:30:48.000000 plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/top_level.txt
```

### Comparing `plone.app.standardtiles-3.1.1/CHANGES.rst` & `plone.app.standardtiles-3.1.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+3.1.2 (2023-06-06)
+------------------
+
+- Fix missing `item_count` value when coming from older versions.
+  [petschki]
+
+
 3.1.1 (2023-05-13)
 ------------------
 
 - Fix boolean fields title/description/text to not be required.
   [petschki]
```

### Comparing `plone.app.standardtiles-3.1.1/LICENSE.GPL` & `plone.app.standardtiles-3.1.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/LICENSE.txt` & `plone.app.standardtiles-3.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/PKG-INFO` & `plone.app.standardtiles-3.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.standardtiles
-Version: 3.1.1
+Version: 3.1.2
 Summary: Tiles for plone.app.blocks page composition
 Home-page: https://github.com/plone/plone.app.standardtiles
 Author: Rob Gietema
 Author-email: rob@fourdigits.nl
 License: GPL
 Keywords: tiles content plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,14 +58,21 @@
 -------
 
 The project is licensed under the GPLv2.
 
 Changelog
 =========
 
+3.1.2 (2023-06-06)
+------------------
+
+- Fix missing `item_count` value when coming from older versions.
+  [petschki]
+
+
 3.1.1 (2023-05-13)
 ------------------
 
 - Fix boolean fields title/description/text to not be required.
   [petschki]
```

### Comparing `plone.app.standardtiles-3.1.1/README.rst` & `plone.app.standardtiles-3.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/pyproject.toml` & `plone.app.standardtiles-3.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/setup.py` & `plone.app.standardtiles-3.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.1.1"
+version = "3.1.2"
 
 
 setup(
     name="plone.app.standardtiles",
     version=version,
     description="Tiles for plone.app.blocks page composition",
     long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
```

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/attachment.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/attachment.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/common.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/common.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/configure.zcml` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/content.zcml` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/content.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/contentlisting.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/contentlisting.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
         b_size=None,
         sort_on=None,
         limit=None,
         brains=False,
         custom_query=None,
     ):
         if not b_size:
-            b_size = self.item_count
+            b_size = self.item_count or 30
         if not sort_on:
             sort_on = self.sort_on
         if not limit:
             limit = self.limit
 
         builder = getMultiAdapter(
             (self.context, self.request), name="querybuilderresults"
```

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/discussion.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/discussion.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/embed.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/embed.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/existingcontent.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/existingcontent.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/field.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/field.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/head.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/head.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/head.zcml` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/head.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/html.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/html.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/interfaces.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/layout.zcml` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/layout.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/linkintegrity.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/linkintegrity.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/media.zcml` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/media.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/metadata.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/metadata.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/navigation.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/navigation.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/add.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/add.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/assignment.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/assignment.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/configure.zcml` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/edit.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/edit.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/portlet.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/portlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/portletmanager.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/portletmanager.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/utils.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/portlets/vocabularies.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/portlets/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/profiles/default/registry.xml` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/rawembed.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/rawembed.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/rss.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/rss.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/setuphandlers.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/sitemap.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/sitemap.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/attachment_listing.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/attachment_listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/configlets.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/configlets.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/contentlisting_view.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/contentlisting_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/existingcontent_view.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/existingcontent_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/image.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/image.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/listing_view.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/listing_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/login.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/login.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/namedimage.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/namedimage.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/navigation.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/navigation.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/navigation_recurse.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/navigation_recurse.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/navigationlink.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/navigationlink.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/rawembed.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/rawembed.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/rss.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/rss.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/summary_view.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/summary_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/templates/tabular_view.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/templates/tabular_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/testing.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/testing.zcml` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/RSS.xml` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/RSS.xml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/funky_display.pt` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/funky_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/test_content.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/test_existing_content.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_existing_content.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/test_field.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/test_head.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_head.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/test_layout.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/test_media.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_media.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/tests/test_setup.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/upgrades.zcml` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/utils.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone/app/standardtiles/viewletmanager.py` & `plone.app.standardtiles-3.1.2/src/plone/app/standardtiles/viewletmanager.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.1.1/src/plone.app.standardtiles.egg-info/PKG-INFO` & `plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.standardtiles
-Version: 3.1.1
+Version: 3.1.2
 Summary: Tiles for plone.app.blocks page composition
 Home-page: https://github.com/plone/plone.app.standardtiles
 Author: Rob Gietema
 Author-email: rob@fourdigits.nl
 License: GPL
 Keywords: tiles content plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,14 +58,21 @@
 -------
 
 The project is licensed under the GPLv2.
 
 Changelog
 =========
 
+3.1.2 (2023-06-06)
+------------------
+
+- Fix missing `item_count` value when coming from older versions.
+  [petschki]
+
+
 3.1.1 (2023-05-13)
 ------------------
 
 - Fix boolean fields title/description/text to not be required.
   [petschki]
```

### Comparing `plone.app.standardtiles-3.1.1/src/plone.app.standardtiles.egg-info/SOURCES.txt` & `plone.app.standardtiles-3.1.2/src/plone.app.standardtiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

