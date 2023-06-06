# Comparing `tmp/eea.kitkat-6.1.zip` & `tmp/eea.kitkat-6.2.zip`

## zipinfo {}

```diff
@@ -1,261 +1,263 @@
-Zip file size: 76275 bytes, number of entries: 259
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/docs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea.kitkat.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/
--rw-r--r--  2.0 unx       38 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/setup.cfg
--rw-r--r--  2.0 unx     2280 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/CONTRIBUTING.md
--rw-r--r--  2.0 unx    14140 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/PKG-INFO
--rw-r--r--  2.0 unx    10214 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/README.rst
--rw-r--r--  2.0 unx     1946 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/setup.py
--rw-r--r--  2.0 unx      126 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/MANIFEST.in
--rw-r--r--  2.0 unx     3055 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/docs/HISTORY.txt
--rw-r--r--  2.0 unx      909 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/docs/LICENSE.txt
--rw-r--r--  2.0 unx    18092 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/docs/LICENSE.GPL
--rw-r--r--  2.0 unx       53 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea.kitkat.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea.kitkat.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx    14140 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea.kitkat.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        4 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea.kitkat.egg-info/namespace_packages.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea.kitkat.egg-info/not-zip-safe
--rw-r--r--  2.0 unx      215 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea.kitkat.egg-info/requires.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea.kitkat.egg-info/top_level.txt
--rw-r--r--  2.0 unx     6873 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea.kitkat.egg-info/SOURCES.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/restapi/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/upgrades/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/browser/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/
--rw-r--r--  2.0 unx        4 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/version.txt
--rw-r--r--  2.0 unx      821 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/configure.zcml
--rw-r--r--  2.0 unx      903 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/events.py
--rw-r--r--  2.0 unx      662 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/setuphandlers.py
--rw-r--r--  2.0 unx     1500 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/interfaces.py
--rw-r--r--  2.0 unx      328 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/README.txt
--rw-r--r--  2.0 unx     1724 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles.zcml
--rw-r--r--  2.0 unx     1659 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/zh_TW/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/en/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/hr/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/es/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pt_BR/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/ro/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/eu/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/el/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/it/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/ru/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/is/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/lt/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/hu/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/nl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pt/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/fi/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/lv/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/mt/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/tr/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/no/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sv/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/bg/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/kl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/et/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sk/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/cs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/da/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/fr/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/de/
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/eea.pot
--rwxr-xr-x  2.0 unx      218 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/update.sh
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/plone-manual.pot
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/zh_TW/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/zh_TW/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/zh_TW/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/zh_TW/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/zh_TW/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/en/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/en/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/en/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/en/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/hr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/hr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/hr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/hr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/hr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/es/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/es/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/es/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/es/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/es/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pt_BR/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pt_BR/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pt_BR/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pt_BR/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pt_BR/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/ro/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/ro/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/ro/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/ro/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/ro/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/eu/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/eu/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/eu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/eu/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/eu/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/el/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/el/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/el/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/el/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/el/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/it/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/it/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/it/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/it/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/it/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/ru/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/ru/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/ru/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/ru/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/ru/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/is/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/is/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/is/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/is/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/is/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/lt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/lt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/lt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/lt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/lt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/hu/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/hu/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/hu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/hu/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/hu/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/nl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/nl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/nl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/nl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/nl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/fi/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/fi/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/fi/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/fi/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/fi/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/lv/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/lv/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/lv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/lv/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/lv/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/mt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/mt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/mt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/mt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/mt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/tr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/tr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/tr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/tr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/tr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/no/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/no/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/no/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/no/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/no/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sv/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sv/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sv/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sv/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/bg/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/bg/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/bg/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/bg/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/bg/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/kl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/kl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/kl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/kl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/kl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/et/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/et/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/et/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/et/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/et/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sk/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sk/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sk/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sk/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/sk/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/pl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/cs/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/cs/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/cs/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/cs/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/cs/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/da/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/da/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/da/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/da/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/da/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/fr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/fr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/fr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/fr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/fr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/de/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/de/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/de/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/de/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/locales/de/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx     1167 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/restapi/post.py
--rw-r--r--  2.0 unx     1614 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/restapi/configure.zcml
--rw-r--r--  2.0 unx     1875 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/restapi/update.py
--rw-r--r--  2.0 unx     2018 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/restapi/get.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/restapi/__init__.py
--rw-r--r--  2.0 unx     2015 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/upgrades/configure.zcml
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/upgrades/__init__.py
--rw-r--r--  2.0 unx     1608 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/tests/base.py
--rw-r--r--  2.0 unx      660 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/tests/test_doctests.py
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/tests/__init__.py
--rw-r--r--  2.0 unx      509 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/browser/configure.zcml
--rw-r--r--  2.0 unx     2924 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/browser/captcha.py
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/browser/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/uninstall/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/upgrades/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/default/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/testing/
--rw-r--r--  2.0 unx      191 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/uninstall/registry.xml
--rw-r--r--  2.0 unx      120 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/uninstall/browserlayer.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/upgrades/to_50/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/upgrades/to_60/
--rw-r--r--  2.0 unx      185 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/upgrades/to_50/actions.xml
--rw-r--r--  2.0 unx       90 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/upgrades/to_50/browserlayer.xml
--rw-r--r--  2.0 unx      126 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/upgrades/to_60/browserlayer.xml
--rw-r--r--  2.0 unx      666 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/default/metadata.xml
--rw-r--r--  2.0 unx     9539 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/default/actions.xml
--rw-r--r--  2.0 unx      235 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/default/registry.xml
--rw-r--r--  2.0 unx      156 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/default/browserlayer.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/testing/types/
--rw-r--r--  2.0 unx      112 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/testing/types.xml
--rw-r--r--  2.0 unx      178 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/testing/metadata.xml
--rw-r--r--  2.0 unx     2189 b- defN 23-Jun-01 15:19 eea.kitkat-6.1/eea/kitkat/profiles/testing/types/kitkat.xml
-259 files, 109976 bytes uncompressed, 31129 bytes compressed:  71.7%
+Zip file size: 76981 bytes, number of entries: 261
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea.kitkat.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/
+-rw-r--r--  2.0 unx       38 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/setup.cfg
+-rw-r--r--  2.0 unx     2280 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/CONTRIBUTING.md
+-rw-r--r--  2.0 unx    14275 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/PKG-INFO
+-rw-r--r--  2.0 unx    10214 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/README.rst
+-rw-r--r--  2.0 unx     1946 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/setup.py
+-rw-r--r--  2.0 unx      126 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/MANIFEST.in
+-rw-r--r--  2.0 unx     3190 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/docs/HISTORY.txt
+-rw-r--r--  2.0 unx      909 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/docs/LICENSE.txt
+-rw-r--r--  2.0 unx    18092 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/docs/LICENSE.GPL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea.kitkat.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea.kitkat.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx    14275 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea.kitkat.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea.kitkat.egg-info/namespace_packages.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea.kitkat.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx      215 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea.kitkat.egg-info/requires.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea.kitkat.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     6920 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea.kitkat.egg-info/SOURCES.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/restapi/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/upgrades/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/browser/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/version.txt
+-rw-r--r--  2.0 unx      821 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/configure.zcml
+-rw-r--r--  2.0 unx      903 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/events.py
+-rw-r--r--  2.0 unx      662 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/setuphandlers.py
+-rw-r--r--  2.0 unx     1500 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/interfaces.py
+-rw-r--r--  2.0 unx      328 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/README.txt
+-rw-r--r--  2.0 unx     1961 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles.zcml
+-rw-r--r--  2.0 unx     1659 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/zh_TW/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/en/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/hr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/es/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pt_BR/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/ro/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/eu/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/el/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/it/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/ru/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/is/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/lt/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/hu/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/nl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pt/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/fi/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/lv/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/mt/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/tr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/no/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sv/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/bg/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/kl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/et/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sk/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/cs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/da/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/fr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/de/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/eea.pot
+-rwxr-xr-x  2.0 unx      218 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/update.sh
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/plone-manual.pot
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/zh_TW/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/zh_TW/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/zh_TW/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/zh_TW/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/en/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/en/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/en/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/en/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/hr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/hr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/hr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/hr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/hr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/es/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/es/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/es/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/es/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/es/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pt_BR/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pt_BR/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pt_BR/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pt_BR/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/ro/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/ro/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/ro/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/ro/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/ro/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/eu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/eu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/eu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/eu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/eu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/el/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/el/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/el/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/el/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/el/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/it/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/it/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/it/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/it/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/it/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/ru/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/ru/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/ru/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/ru/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/ru/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/is/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/is/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/is/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/is/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/is/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/lt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/lt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/lt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/lt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/lt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/hu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/hu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/hu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/hu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/hu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/nl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/nl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/nl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/nl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/nl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/fi/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/fi/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/fi/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/fi/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/fi/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/lv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/lv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/lv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/lv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/lv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/mt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/mt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/mt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/mt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/mt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/tr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/tr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/tr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/tr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/tr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/no/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/no/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/no/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/no/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/no/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/bg/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/bg/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/bg/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/bg/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/bg/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/kl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/kl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/kl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/kl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/kl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/et/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/et/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/et/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/et/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/et/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sk/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sk/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sk/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sk/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/sk/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/pl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/cs/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/cs/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/cs/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/cs/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/cs/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/da/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/da/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/da/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/da/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/da/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/fr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/fr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/fr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/fr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/fr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/de/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/de/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/de/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/de/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/locales/de/LC_MESSAGES/plone.po
+-rw-r--r--  2.0 unx     1167 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/restapi/post.py
+-rw-r--r--  2.0 unx     1614 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/restapi/configure.zcml
+-rw-r--r--  2.0 unx     1875 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/restapi/update.py
+-rw-r--r--  2.0 unx     2018 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/restapi/get.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/restapi/__init__.py
+-rw-r--r--  2.0 unx     2281 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/upgrades/configure.zcml
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/upgrades/__init__.py
+-rw-r--r--  2.0 unx     1608 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/tests/base.py
+-rw-r--r--  2.0 unx      660 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/tests/test_doctests.py
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/tests/__init__.py
+-rw-r--r--  2.0 unx      509 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/browser/configure.zcml
+-rw-r--r--  2.0 unx     2924 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/browser/captcha.py
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/browser/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/uninstall/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/upgrades/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/default/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/testing/
+-rw-r--r--  2.0 unx      191 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/uninstall/registry.xml
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/uninstall/browserlayer.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/upgrades/to_50/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/upgrades/to_62/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/upgrades/to_60/
+-rw-r--r--  2.0 unx      185 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/upgrades/to_50/actions.xml
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/upgrades/to_50/browserlayer.xml
+-rw-r--r--  2.0 unx      221 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/upgrades/to_62/rolemap.xml
+-rw-r--r--  2.0 unx      126 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/upgrades/to_60/browserlayer.xml
+-rw-r--r--  2.0 unx      666 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/default/metadata.xml
+-rw-r--r--  2.0 unx     9539 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/default/actions.xml
+-rw-r--r--  2.0 unx      235 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/default/registry.xml
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/default/browserlayer.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/testing/types/
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/testing/types.xml
+-rw-r--r--  2.0 unx      178 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/testing/metadata.xml
+-rw-r--r--  2.0 unx     2189 b- defN 23-Jun-06 14:56 eea.kitkat-6.2/eea/kitkat/profiles/testing/types/kitkat.xml
+261 files, 111152 bytes uncompressed, 31461 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -1,778 +1,784 @@
-Filename: eea.kitkat-6.1/
+Filename: eea.kitkat-6.2/
 Comment: 
 
-Filename: eea.kitkat-6.1/docs/
+Filename: eea.kitkat-6.2/docs/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea.kitkat.egg-info/
+Filename: eea.kitkat-6.2/eea.kitkat.egg-info/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/
+Filename: eea.kitkat-6.2/eea/
 Comment: 
 
-Filename: eea.kitkat-6.1/setup.cfg
+Filename: eea.kitkat-6.2/setup.cfg
 Comment: 
 
-Filename: eea.kitkat-6.1/CONTRIBUTING.md
+Filename: eea.kitkat-6.2/CONTRIBUTING.md
 Comment: 
 
-Filename: eea.kitkat-6.1/PKG-INFO
+Filename: eea.kitkat-6.2/PKG-INFO
 Comment: 
 
-Filename: eea.kitkat-6.1/README.rst
+Filename: eea.kitkat-6.2/README.rst
 Comment: 
 
-Filename: eea.kitkat-6.1/setup.py
+Filename: eea.kitkat-6.2/setup.py
 Comment: 
 
-Filename: eea.kitkat-6.1/MANIFEST.in
+Filename: eea.kitkat-6.2/MANIFEST.in
 Comment: 
 
-Filename: eea.kitkat-6.1/docs/HISTORY.txt
+Filename: eea.kitkat-6.2/docs/HISTORY.txt
 Comment: 
 
-Filename: eea.kitkat-6.1/docs/LICENSE.txt
+Filename: eea.kitkat-6.2/docs/LICENSE.txt
 Comment: 
 
-Filename: eea.kitkat-6.1/docs/LICENSE.GPL
+Filename: eea.kitkat-6.2/docs/LICENSE.GPL
 Comment: 
 
-Filename: eea.kitkat-6.1/eea.kitkat.egg-info/entry_points.txt
+Filename: eea.kitkat-6.2/eea.kitkat.egg-info/entry_points.txt
 Comment: 
 
-Filename: eea.kitkat-6.1/eea.kitkat.egg-info/dependency_links.txt
+Filename: eea.kitkat-6.2/eea.kitkat.egg-info/dependency_links.txt
 Comment: 
 
-Filename: eea.kitkat-6.1/eea.kitkat.egg-info/PKG-INFO
+Filename: eea.kitkat-6.2/eea.kitkat.egg-info/PKG-INFO
 Comment: 
 
-Filename: eea.kitkat-6.1/eea.kitkat.egg-info/namespace_packages.txt
+Filename: eea.kitkat-6.2/eea.kitkat.egg-info/namespace_packages.txt
 Comment: 
 
-Filename: eea.kitkat-6.1/eea.kitkat.egg-info/not-zip-safe
+Filename: eea.kitkat-6.2/eea.kitkat.egg-info/not-zip-safe
 Comment: 
 
-Filename: eea.kitkat-6.1/eea.kitkat.egg-info/requires.txt
+Filename: eea.kitkat-6.2/eea.kitkat.egg-info/requires.txt
 Comment: 
 
-Filename: eea.kitkat-6.1/eea.kitkat.egg-info/top_level.txt
+Filename: eea.kitkat-6.2/eea.kitkat.egg-info/top_level.txt
 Comment: 
 
-Filename: eea.kitkat-6.1/eea.kitkat.egg-info/SOURCES.txt
+Filename: eea.kitkat-6.2/eea.kitkat.egg-info/SOURCES.txt
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/
+Filename: eea.kitkat-6.2/eea/kitkat/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/__init__.py
+Filename: eea.kitkat-6.2/eea/__init__.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/restapi/
+Filename: eea.kitkat-6.2/eea/kitkat/restapi/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/upgrades/
+Filename: eea.kitkat-6.2/eea/kitkat/upgrades/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/tests/
+Filename: eea.kitkat-6.2/eea/kitkat/tests/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/browser/
+Filename: eea.kitkat-6.2/eea/kitkat/browser/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/version.txt
+Filename: eea.kitkat-6.2/eea/kitkat/version.txt
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/configure.zcml
+Filename: eea.kitkat-6.2/eea/kitkat/configure.zcml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/events.py
+Filename: eea.kitkat-6.2/eea/kitkat/events.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/setuphandlers.py
+Filename: eea.kitkat-6.2/eea/kitkat/setuphandlers.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/interfaces.py
+Filename: eea.kitkat-6.2/eea/kitkat/interfaces.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/README.txt
+Filename: eea.kitkat-6.2/eea/kitkat/README.txt
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles.zcml
+Filename: eea.kitkat-6.2/eea/kitkat/profiles.zcml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/__init__.py
+Filename: eea.kitkat-6.2/eea/kitkat/__init__.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/zh_TW/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/zh_TW/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/en/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/en/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/hr/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/hr/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/es/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/es/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pt_BR/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pt_BR/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/ro/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/ro/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/eu/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/eu/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/el/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/el/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/it/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/it/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/ru/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/ru/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/is/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/is/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/lt/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/lt/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/hu/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/hu/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/nl/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/nl/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pt/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pt/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/fi/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/fi/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/lv/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/lv/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sl/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sl/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/mt/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/mt/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/tr/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/tr/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/no/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/no/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sv/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sv/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/bg/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/bg/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/kl/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/kl/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/et/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/et/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sk/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sk/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pl/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pl/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/cs/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/cs/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/da/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/da/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/fr/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/fr/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/de/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/de/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/eea.pot
+Filename: eea.kitkat-6.2/eea/kitkat/locales/eea.pot
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/update.sh
+Filename: eea.kitkat-6.2/eea/kitkat/locales/update.sh
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/plone-manual.pot
+Filename: eea.kitkat-6.2/eea/kitkat/locales/plone-manual.pot
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/__init__.py
+Filename: eea.kitkat-6.2/eea/kitkat/locales/__init__.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/zh_TW/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/zh_TW/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/zh_TW/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/zh_TW/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/zh_TW/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/zh_TW/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/zh_TW/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/zh_TW/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/zh_TW/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/zh_TW/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/en/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/en/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/en/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/en/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/en/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/en/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/en/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/en/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/en/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/en/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/hr/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/hr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/hr/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/hr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/hr/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/hr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/hr/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/hr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/hr/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/hr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/es/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/es/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/es/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/es/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/es/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/es/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/es/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/es/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/es/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/es/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pt_BR/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pt_BR/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pt_BR/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pt_BR/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pt_BR/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pt_BR/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pt_BR/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pt_BR/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pt_BR/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pt_BR/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/ro/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/ro/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/ro/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/ro/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/ro/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/ro/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/ro/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/ro/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/ro/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/ro/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/eu/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/eu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/eu/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/eu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/eu/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/eu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/eu/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/eu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/eu/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/eu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/el/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/el/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/el/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/el/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/el/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/el/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/el/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/el/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/el/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/el/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/it/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/it/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/it/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/it/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/it/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/it/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/it/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/it/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/it/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/it/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/ru/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/ru/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/ru/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/ru/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/ru/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/ru/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/ru/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/ru/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/ru/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/ru/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/is/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/is/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/is/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/is/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/is/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/is/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/is/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/is/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/is/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/is/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/lt/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/lt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/lt/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/lt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/lt/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/lt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/lt/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/lt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/lt/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/lt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/hu/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/hu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/hu/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/hu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/hu/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/hu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/hu/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/hu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/hu/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/hu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/nl/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/nl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/nl/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/nl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/nl/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/nl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/nl/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/nl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/nl/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/nl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pt/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pt/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pt/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pt/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pt/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/fi/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/fi/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/fi/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/fi/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/fi/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/fi/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/fi/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/fi/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/fi/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/fi/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/lv/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/lv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/lv/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/lv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/lv/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/lv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/lv/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/lv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/lv/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/lv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sl/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sl/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sl/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sl/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sl/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/mt/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/mt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/mt/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/mt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/mt/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/mt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/mt/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/mt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/mt/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/mt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/tr/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/tr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/tr/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/tr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/tr/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/tr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/tr/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/tr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/tr/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/tr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/no/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/no/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/no/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/no/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/no/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/no/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/no/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/no/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/no/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/no/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sv/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sv/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sv/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sv/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sv/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/bg/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/bg/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/bg/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/bg/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/bg/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/bg/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/bg/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/bg/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/bg/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/bg/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/kl/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/kl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/kl/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/kl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/kl/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/kl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/kl/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/kl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/kl/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/kl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/et/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/et/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/et/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/et/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/et/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/et/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/et/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/et/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/et/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/et/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sk/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sk/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sk/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sk/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sk/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sk/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sk/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sk/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/sk/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/sk/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pl/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pl/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pl/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pl/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/pl/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/pl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/cs/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/cs/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/cs/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/cs/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/cs/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/cs/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/cs/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/cs/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/cs/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/cs/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/da/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/da/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/da/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/da/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/da/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/da/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/da/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/da/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/da/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/da/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/fr/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/fr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/fr/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/fr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/fr/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/fr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/fr/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/fr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/fr/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/fr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/de/LC_MESSAGES/
+Filename: eea.kitkat-6.2/eea/kitkat/locales/de/LC_MESSAGES/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/de/LC_MESSAGES/plone.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/de/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/de/LC_MESSAGES/eea.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/de/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/de/LC_MESSAGES/eea.mo
+Filename: eea.kitkat-6.2/eea/kitkat/locales/de/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/locales/de/LC_MESSAGES/plone.po
+Filename: eea.kitkat-6.2/eea/kitkat/locales/de/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/restapi/post.py
+Filename: eea.kitkat-6.2/eea/kitkat/restapi/post.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/restapi/configure.zcml
+Filename: eea.kitkat-6.2/eea/kitkat/restapi/configure.zcml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/restapi/update.py
+Filename: eea.kitkat-6.2/eea/kitkat/restapi/update.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/restapi/get.py
+Filename: eea.kitkat-6.2/eea/kitkat/restapi/get.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/restapi/__init__.py
+Filename: eea.kitkat-6.2/eea/kitkat/restapi/__init__.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/upgrades/configure.zcml
+Filename: eea.kitkat-6.2/eea/kitkat/upgrades/configure.zcml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/upgrades/__init__.py
+Filename: eea.kitkat-6.2/eea/kitkat/upgrades/__init__.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/tests/base.py
+Filename: eea.kitkat-6.2/eea/kitkat/tests/base.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/tests/test_doctests.py
+Filename: eea.kitkat-6.2/eea/kitkat/tests/test_doctests.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/tests/__init__.py
+Filename: eea.kitkat-6.2/eea/kitkat/tests/__init__.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/browser/configure.zcml
+Filename: eea.kitkat-6.2/eea/kitkat/browser/configure.zcml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/browser/captcha.py
+Filename: eea.kitkat-6.2/eea/kitkat/browser/captcha.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/browser/__init__.py
+Filename: eea.kitkat-6.2/eea/kitkat/browser/__init__.py
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/uninstall/
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/uninstall/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/upgrades/
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/upgrades/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/default/
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/default/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/testing/
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/testing/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/uninstall/registry.xml
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/uninstall/registry.xml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/uninstall/browserlayer.xml
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/uninstall/browserlayer.xml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/upgrades/to_50/
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/upgrades/to_50/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/upgrades/to_60/
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/upgrades/to_62/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/upgrades/to_50/actions.xml
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/upgrades/to_60/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/upgrades/to_50/browserlayer.xml
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/upgrades/to_50/actions.xml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/upgrades/to_60/browserlayer.xml
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/upgrades/to_50/browserlayer.xml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/default/metadata.xml
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/upgrades/to_62/rolemap.xml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/default/actions.xml
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/upgrades/to_60/browserlayer.xml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/default/registry.xml
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/default/metadata.xml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/default/browserlayer.xml
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/default/actions.xml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/testing/types/
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/default/registry.xml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/testing/types.xml
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/default/browserlayer.xml
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/testing/metadata.xml
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/testing/types/
 Comment: 
 
-Filename: eea.kitkat-6.1/eea/kitkat/profiles/testing/types/kitkat.xml
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/testing/types.xml
+Comment: 
+
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/testing/metadata.xml
+Comment: 
+
+Filename: eea.kitkat-6.2/eea/kitkat/profiles/testing/types/kitkat.xml
 Comment: 
 
 Zip file comment:
```

## Comparing `eea.kitkat-6.1/CONTRIBUTING.md` & `eea.kitkat-6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/PKG-INFO` & `eea.kitkat-6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eea.kitkat
-Version: 6.1
+Version: 6.2
 Summary: An add-on for Plone
 Home-page: https://github.com/eea/eea.kitkat
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
 Platform: UNKNOWN
@@ -277,14 +277,19 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+6.2 - (2023-06-06)
+---------------------------
+* Change: View comments permission only for authenticated
+  [dobri1408 - refs #251360]
+
 6.1 - (2023-06-01)
 ---------------------------
 * Bug fix: Hide Footer Login action if user is logged-in
   [avoinea - refs #253198]
 
 6.0 - (2023-05-31)
 ---------------------------
```

## Comparing `eea.kitkat-6.1/README.rst` & `eea.kitkat-6.2/README.rst`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/setup.py` & `eea.kitkat-6.2/setup.py`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/docs/HISTORY.txt` & `eea.kitkat-6.2/docs/HISTORY.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+6.2 - (2023-06-06)
+---------------------------
+* Change: View comments permission only for authenticated
+  [dobri1408 - refs #251360]
+
 6.1 - (2023-06-01)
 ---------------------------
 * Bug fix: Hide Footer Login action if user is logged-in
   [avoinea - refs #253198]
 
 6.0 - (2023-05-31)
 ---------------------------
```

## Comparing `eea.kitkat-6.1/docs/LICENSE.txt` & `eea.kitkat-6.2/docs/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/docs/LICENSE.GPL` & `eea.kitkat-6.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/eea.kitkat.egg-info/PKG-INFO` & `eea.kitkat-6.2/eea.kitkat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eea.kitkat
-Version: 6.1
+Version: 6.2
 Summary: An add-on for Plone
 Home-page: https://github.com/eea/eea.kitkat
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
 Platform: UNKNOWN
@@ -277,14 +277,19 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+6.2 - (2023-06-06)
+---------------------------
+* Change: View comments permission only for authenticated
+  [dobri1408 - refs #251360]
+
 6.1 - (2023-06-01)
 ---------------------------
 * Bug fix: Hide Footer Login action if user is logged-in
   [avoinea - refs #253198]
 
 6.0 - (2023-05-31)
 ---------------------------
```

## Comparing `eea.kitkat-6.1/eea.kitkat.egg-info/SOURCES.txt` & `eea.kitkat-6.2/eea.kitkat.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -161,14 +161,15 @@
 eea/kitkat/profiles/testing/types.xml
 eea/kitkat/profiles/testing/types/kitkat.xml
 eea/kitkat/profiles/uninstall/browserlayer.xml
 eea/kitkat/profiles/uninstall/registry.xml
 eea/kitkat/profiles/upgrades/to_50/actions.xml
 eea/kitkat/profiles/upgrades/to_50/browserlayer.xml
 eea/kitkat/profiles/upgrades/to_60/browserlayer.xml
+eea/kitkat/profiles/upgrades/to_62/rolemap.xml
 eea/kitkat/restapi/__init__.py
 eea/kitkat/restapi/configure.zcml
 eea/kitkat/restapi/get.py
 eea/kitkat/restapi/post.py
 eea/kitkat/restapi/update.py
 eea/kitkat/tests/__init__.py
 eea/kitkat/tests/base.py
```

## Comparing `eea.kitkat-6.1/eea/kitkat/configure.zcml` & `eea.kitkat-6.2/eea/kitkat/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/eea/kitkat/events.py` & `eea.kitkat-6.2/eea/kitkat/events.py`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/eea/kitkat/setuphandlers.py` & `eea.kitkat-6.2/eea/kitkat/setuphandlers.py`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/eea/kitkat/interfaces.py` & `eea.kitkat-6.2/eea/kitkat/interfaces.py`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/eea/kitkat/profiles.zcml` & `eea.kitkat-6.2/eea/kitkat/profiles.zcml`

 * *Files 9% similar despite different names*

```diff
@@ -45,13 +45,21 @@
       name="kitkat_60"
       title="Upgrade profile for eea.kitkat 6.0"
       description=""
       directory="profiles/upgrades/to_60"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       />
 
+  <genericsetup:registerProfile
+      name="kitkat_62"
+      title="Upgrade profile for eea.kitkat 6.2"
+      description=""
+      directory="profiles/upgrades/to_62"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      />
+
   <utility
       factory=".setuphandlers.HiddenProfiles"
       name="eea.kitkat-hiddenprofiles"
       />
 
 </configure>
```

## Comparing `eea.kitkat-6.1/eea/kitkat/__init__.py` & `eea.kitkat-6.2/eea/kitkat/__init__.py`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/eea/kitkat/restapi/post.py` & `eea.kitkat-6.2/eea/kitkat/restapi/post.py`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/eea/kitkat/restapi/configure.zcml` & `eea.kitkat-6.2/eea/kitkat/restapi/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/eea/kitkat/restapi/update.py` & `eea.kitkat-6.2/eea/kitkat/restapi/update.py`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/eea/kitkat/restapi/get.py` & `eea.kitkat-6.2/eea/kitkat/restapi/get.py`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/eea/kitkat/upgrades/configure.zcml` & `eea.kitkat-6.2/eea/kitkat/upgrades/configure.zcml`

 * *Files 6% similar despite different names*

```diff
@@ -80,11 +80,21 @@
     destination="6.0"
     profile="eea.kitkat:default">
 
     <genericsetup:upgradeDepends
       title="Remove eea.api.taxonomy"
       import_profile="eea.kitkat:kitkat_60"
       />
-
   </genericsetup:upgradeSteps>
 
+  <genericsetup:upgradeSteps
+    source="6.0"
+    destination="6.2"
+    profile="eea.kitkat:default">
+
+    <genericsetup:upgradeDepends
+      title="Update permissions for comments"
+      import_profile="eea.kitkat:kitkat_62"
+      />
+  </genericsetup:upgradeSteps>
 </configure>
+
```

## Comparing `eea.kitkat-6.1/eea/kitkat/tests/base.py` & `eea.kitkat-6.2/eea/kitkat/tests/base.py`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/eea/kitkat/tests/test_doctests.py` & `eea.kitkat-6.2/eea/kitkat/tests/test_doctests.py`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/eea/kitkat/browser/captcha.py` & `eea.kitkat-6.2/eea/kitkat/browser/captcha.py`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/eea/kitkat/profiles/default/metadata.xml` & `eea.kitkat-6.2/eea/kitkat/profiles/default/metadata.xml`

 * *Files 1% similar despite different names*

### Comparing `eea.kitkat-6.1/eea/kitkat/profiles/default/metadata.xml` & `eea.kitkat-6.2/eea/kitkat/profiles/default/metadata.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <metadata>
-  <version>6.0</version>
+  <version>6.2</version>
   <dependencies>
     <dependency>profile-collective.taxonomy:default</dependency>
     <dependency>profile-eea.api.layout:default</dependency>
     <dependency>profile-eea.banner:default</dependency>
     <dependency>profile-eea.coremetadata:default</dependency>
     <dependency>profile-eea.geolocation:default</dependency>
     <dependency>profile-eea.sentry:default</dependency>
```

## Comparing `eea.kitkat-6.1/eea/kitkat/profiles/default/actions.xml` & `eea.kitkat-6.2/eea/kitkat/profiles/default/actions.xml`

 * *Files identical despite different names*

## Comparing `eea.kitkat-6.1/eea/kitkat/profiles/testing/types/kitkat.xml` & `eea.kitkat-6.2/eea/kitkat/profiles/testing/types/kitkat.xml`

 * *Files identical despite different names*

