# Comparing `tmp/talisman-dm-1.0.0a8.tar.gz` & `tmp/talisman-dm-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/talisman-dm-1.0.0a8.tar", last modified: Tue May 23 20:53:41 2023, max compression
+gzip compressed data, was "dist/talisman-dm-1.0.0a9.tar", last modified: Tue May 30 13:05:13 2023, max compression
```

## Comparing `talisman-dm-1.0.0a8.tar` & `talisman-dm-1.0.0a9.tar`

### file list

```diff
@@ -1,140 +1,141 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-13 06:48:56.000000 talisman-dm-1.0.0a8/README.md
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/VERSION
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1195 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/talisman_dm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/talisman_dm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3717 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/talisman_dm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/talisman_dm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/talisman_dm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/talisman_dm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/abstract/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 20:53:34.000000 talisman-dm-1.0.0a8/tdm/abstract/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)     1060 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/directive.py
--rw-rw-rw-   0 root         (0) root         (0)     6818 2023-05-23 18:40:05.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/document.py
--rw-rw-rw-   0 root         (0) root         (0)     2269 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     5838 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/fact.py
--rw-rw-rw-   0 root         (0) root         (0)      604 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/identifiable.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/_helper.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/frozen.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/model.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/mention.py
--rw-rw-rw-   0 root         (0) root         (0)     1634 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/node.py
--rw-rw-rw-   0 root         (0) root         (0)      996 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/datamodel/value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4947 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/composite.py
--rw-rw-rw-   0 root         (0) root         (0)     1184 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     4854 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/
--rw-rw-rw-   0 root         (0) root         (0)      630 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1207 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/domain.py
--rw-rw-rw-   0 root         (0) root         (0)      737 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/identifiable.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/markup.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/mention.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      982 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/type_.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 20:53:34.000000 talisman-dm-1.0.0a8/tdm/datamodel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/common/
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2455 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/common/_container.py
--rw-rw-rw-   0 root         (0) root         (0)    10036 2023-05-23 18:40:05.000000 talisman-dm-1.0.0a8/tdm/datamodel/common/_impl.py
--rw-rw-rw-   0 root         (0) root         (0)      616 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/common/_state.py
--rw-rw-rw-   0 root         (0) root         (0)      808 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/common/_types.py
--rw-rw-rw-   0 root         (0) root         (0)     5206 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/common/_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/directives/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/directives/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/directives/account.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/directives/concept.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/directives/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/document/
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2023-05-23 18:40:05.000000 talisman-dm-1.0.0a8/tdm/datamodel/document/_factory.py
--rw-rw-rw-   0 root         (0) root         (0)    14014 2023-05-23 18:40:05.000000 talisman-dm-1.0.0a8/tdm/datamodel/document/_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     7193 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/document/_structure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/
--rw-rw-rw-   0 root         (0) root         (0)      643 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1936 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/_impl.py
--rw-rw-rw-   0 root         (0) root         (0)      303 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/_composite.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/_concept.py
--rw-rw-rw-   0 root         (0) root         (0)      576 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/_property.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/_relation.py
--rw-rw-rw-   0 root         (0) root         (0)      308 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/_slot.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/domain/types/_value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/facts/
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/facts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3436 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/facts/concept.py
--rw-rw-rw-   0 root         (0) root         (0)     1103 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/facts/links.py
--rw-rw-rw-   0 root         (0) root         (0)     1405 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/facts/mention.py
--rw-rw-rw-   0 root         (0) root         (0)     4384 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/facts/value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/links/
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/links/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/links/reference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/mentions/
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/mentions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/mentions/image.py
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/mentions/node.py
--rw-rw-rw-   0 root         (0) root         (0)      759 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/mentions/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/nodes/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/nodes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/nodes/base64.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/nodes/file.py
--rw-rw-rw-   0 root         (0) root         (0)     1113 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/nodes/structure.py
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/nodes/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/datamodel/values/
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/values/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/values/date.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/values/geo.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/values/link.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/datamodel/values/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     3253 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/json_schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 20:53:34.000000 talisman-dm-1.0.0a8/tdm/json_schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/json_schema/directives.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/json_schema/facts.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/json_schema/links.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/json_schema/mentions.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/json_schema/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/json_schema/values.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     3262 2023-05-23 12:53:48.000000 talisman-dm-1.0.0a8/tdm/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/v0/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/content.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4733 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/_facts.py
--rw-rw-rw-   0 root         (0) root         (0)     1630 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     4725 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/_nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     1481 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/directive.py
--rw-rw-rw-   0 root         (0) root         (0)     4071 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/document.py
--rw-rw-rw-   0 root         (0) root         (0)     1453 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/fact.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/v0/json_schema/metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/wrapper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 20:53:34.000000 talisman-dm-1.0.0a8/tdm/wrapper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 20:53:41.000000 talisman-dm-1.0.0a8/tdm/wrapper/node/
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/wrapper/node/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5509 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/wrapper/node/_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/wrapper/node/_delegate.py
--rw-rw-rw-   0 root         (0) root         (0)     1647 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/wrapper/node/_impl.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-23 07:11:28.000000 talisman-dm-1.0.0a8/tdm/wrapper/node/_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/VERSION
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/talisman_dm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/talisman_dm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/talisman_dm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/talisman_dm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/talisman_dm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/talisman_dm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 13:05:05.000000 talisman-dm-1.0.0a9/tdm/abstract/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/directive.py
+-rw-rw-rw-   0 root         (0) root         (0)     6818 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     2269 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     5838 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/fact.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/identifiable.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/markup/
+-rw-rw-rw-   0 root         (0) root         (0)      226 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/markup/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1016 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/markup/_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/markup/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/markup/frozen.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/markup/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/mention.py
+-rw-rw-rw-   0 root         (0) root         (0)     1634 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/node.py
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/datamodel/value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4947 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/composite.py
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4575 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/dataclass.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/identifiable.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/markup.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/mention.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      982 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/type_.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 13:05:05.000000 talisman-dm-1.0.0a9/tdm/datamodel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/datamodel/common/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/common/_container.py
+-rw-rw-rw-   0 root         (0) root         (0)    10036 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/common/_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)      616 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/common/_state.py
+-rw-rw-rw-   0 root         (0) root         (0)      808 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/common/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     5206 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/common/_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/datamodel/directives/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/directives/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/directives/account.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/directives/concept.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/directives/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/datamodel/document/
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/document/_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    14014 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/document/_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     7193 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/document/_structure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/datamodel/domain/
+-rw-rw-rw-   0 root         (0) root         (0)      643 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/domain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/domain/_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/domain/_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/datamodel/domain/types/
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/domain/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/domain/types/_composite.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/domain/types/_concept.py
+-rw-rw-rw-   0 root         (0) root         (0)      576 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/domain/types/_property.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/domain/types/_relation.py
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/domain/types/_slot.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/domain/types/_value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/datamodel/facts/
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/facts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3436 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/facts/concept.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/facts/links.py
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/facts/mention.py
+-rw-rw-rw-   0 root         (0) root         (0)     4384 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/facts/value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/datamodel/links/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/links/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/links/reference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/datamodel/mentions/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/mentions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/mentions/image.py
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/mentions/node.py
+-rw-rw-rw-   0 root         (0) root         (0)      759 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/mentions/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/datamodel/nodes/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/nodes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/nodes/base64.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/nodes/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1113 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/nodes/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/nodes/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/datamodel/values/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/values/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/values/date.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/values/geo.py
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/values/link.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/datamodel/values/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     3253 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/json_schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 13:05:05.000000 talisman-dm-1.0.0a9/tdm/json_schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/json_schema/directives.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/json_schema/facts.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/json_schema/links.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/json_schema/mentions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/json_schema/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/json_schema/values.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3301 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/v0/json_schema/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/v0/json_schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/v0/json_schema/content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/v0/json_schema/convert/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/v0/json_schema/convert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4733 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/v0/json_schema/convert/_facts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/v0/json_schema/convert/_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/v0/json_schema/convert/_nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1481 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/v0/json_schema/directive.py
+-rw-rw-rw-   0 root         (0) root         (0)     4071 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/v0/json_schema/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/v0/json_schema/fact.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/v0/json_schema/metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 13:05:05.000000 talisman-dm-1.0.0a9/tdm/wrapper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:05:13.000000 talisman-dm-1.0.0a9/tdm/wrapper/node/
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/wrapper/node/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5509 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/wrapper/node/_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/wrapper/node/_delegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/wrapper/node/_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-30 13:03:43.000000 talisman-dm-1.0.0a9/tdm/wrapper/node/_interface.py
```

### Comparing `talisman-dm-1.0.0a8/PKG-INFO` & `talisman-dm-1.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-dm
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Talisman Document Model python implementation
 Home-page: https://gitlab.at.ispras.ru/talisman/core/talisman-tdm
 Author: ISPRAS MODIS NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
```

### Comparing `talisman-dm-1.0.0a8/setup.py` & `talisman-dm-1.0.0a9/setup.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/talisman_dm.egg-info/PKG-INFO` & `talisman-dm-1.0.0a9/talisman_dm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-dm
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Talisman Document Model python implementation
 Home-page: https://gitlab.at.ispras.ru/talisman/core/talisman-tdm
 Author: ISPRAS MODIS NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
```

### Comparing `talisman-dm-1.0.0a8/talisman_dm.egg-info/SOURCES.txt` & `talisman-dm-1.0.0a9/talisman_dm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 tdm/abstract/datamodel/markup/model.py
 tdm/abstract/json_schema/__init__.py
 tdm/abstract/json_schema/composite.py
 tdm/abstract/json_schema/decorator.py
 tdm/abstract/json_schema/model.py
 tdm/abstract/json_schema/serializers/__init__.py
 tdm/abstract/json_schema/serializers/abstract.py
+tdm/abstract/json_schema/serializers/dataclass.py
 tdm/abstract/json_schema/serializers/domain.py
 tdm/abstract/json_schema/serializers/identifiable.py
 tdm/abstract/json_schema/serializers/markup.py
 tdm/abstract/json_schema/serializers/mention.py
 tdm/abstract/json_schema/serializers/metadata.py
 tdm/abstract/json_schema/serializers/serializers.py
 tdm/abstract/json_schema/serializers/type_.py
```

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/datamodel/__init__.py` & `talisman-dm-1.0.0a9/tdm/abstract/datamodel/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/datamodel/document.py` & `talisman-dm-1.0.0a9/tdm/abstract/datamodel/document.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/datamodel/domain.py` & `talisman-dm-1.0.0a9/tdm/abstract/datamodel/domain.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/datamodel/fact.py` & `talisman-dm-1.0.0a9/tdm/abstract/datamodel/fact.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/datamodel/filter.py` & `talisman-dm-1.0.0a9/tdm/abstract/datamodel/filter.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/datamodel/identifiable.py` & `talisman-dm-1.0.0a9/tdm/abstract/datamodel/identifiable.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/datamodel/link.py` & `talisman-dm-1.0.0a9/tdm/abstract/datamodel/link.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/abstract.py` & `talisman-dm-1.0.0a9/tdm/abstract/datamodel/markup/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/datamodel/markup/frozen.py` & `talisman-dm-1.0.0a9/tdm/abstract/datamodel/markup/frozen.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/datamodel/node.py` & `talisman-dm-1.0.0a9/tdm/abstract/datamodel/node.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/datamodel/value.py` & `talisman-dm-1.0.0a9/tdm/abstract/datamodel/value.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/json_schema/composite.py` & `talisman-dm-1.0.0a9/tdm/abstract/json_schema/composite.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/json_schema/decorator.py` & `talisman-dm-1.0.0a9/tdm/abstract/json_schema/decorator.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/json_schema/model.py` & `talisman-dm-1.0.0a9/tdm/abstract/json_schema/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,16 @@
                 continue
             elif isinstance(value, Sequence):
                 _serialize = lambda s, value=value: type(value)(s.serialize(v) for v in value)
                 value_types = {type(v) for v in value}
             else:
                 _serialize = lambda s, value=value: s.serialize(value)
                 value_types = {type(value)}
-            for type_, serializer in BaseSerializers.items():
-                if all(issubclass(vt, type_) for vt in value_types):
+            for criteria, serializer in BaseSerializers.items():
+                if all(criteria(vt) for vt in value_types):
                     kwargs[key] = _serialize(serializer)
                     break
             else:
                 kwargs[key] = value
         return cls(**kwargs)
 
 
@@ -72,30 +72,26 @@
         default_value = field.default if field.default is not dataclasses.MISSING else ...
         field_type = type_vars.get(field.type, field.type)
         union_types = unfold_union(field_type)
         model_field = False
         f_t = []
         for t in map(lambda ut: type_vars.get(ut, ut), union_types):
             typing_type, real_type, arg = uniform_collection(t)
-            if real_type is type:
-                serializer = BaseSerializers[type]
-                f_t.append(serializer.field_type(arg))
-                special_fields[name].append(serializer.deserialize)
+            for criteria, serializer in BaseSerializers.items():
+                if not criteria(arg):
+                    continue
+                ft = serializer.field_type(arg)
+                if typing_type is None:
+                    f_t.append(ft)
+                    special_fields[name].append(serializer.deserialize)
+                else:
+                    f_t.append(typing_type[ft])
+                    special_fields[name].append(_wrap_deserializer(real_type, serializer))
                 model_field = True
-                continue
-            for _type, serializer in BaseSerializers.items():
-                if issubclass(arg, _type):
-                    if typing_type is None:
-                        f_t.append(serializer.field_type(arg))
-                        special_fields[name].append(serializer.deserialize)
-                    else:
-                        f_t.append(typing_type[serializer.field_type(arg)])
-                        special_fields[name].append(_wrap_deserializer(real_type, serializer))
-                    model_field = True
-                    break
+                break
             else:
                 f_t.append(t)
         if model_field:
             field_type = Union[tuple(f_t)]
 
         model_fields[name] = (field_type, default_value)
     if label:
```

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/__init__.py` & `talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
     'AbstractElementModel', 'AbstractElementSerializer', 'AbstractModelSerializer',
     'IdSerializer',
     'NodeMentionSerializer',
     'NodeMetadataSerializer',
     'BaseSerializers'
 ]
 
-from typing import Mapping
+from typing import Any, Callable, Mapping
 
 from immutabledict import immutabledict
 
 from .abstract import AbstractElementModel, AbstractElementSerializer, AbstractModelSerializer
 from .identifiable import IdSerializer
 from .mention import NodeMentionSerializer
 from .metadata import NodeMetadataSerializer
 from .serializers import build_serializers
 
-BaseSerializers: Mapping[type, AbstractElementSerializer] = immutabledict(build_serializers())
+BaseSerializers: Mapping[Callable[[Any], bool], AbstractElementSerializer] = immutabledict(build_serializers())
```

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/abstract.py` & `talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/domain.py` & `talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/domain.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/identifiable.py` & `talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/identifiable.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/markup.py` & `talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/markup.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/mention.py` & `talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/mention.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/metadata.py` & `talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/metadata.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/type_.py` & `talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/type_.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/abstract/json_schema/serializers/value.py` & `talisman-dm-1.0.0a9/tdm/abstract/json_schema/serializers/value.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/common/_container.py` & `talisman-dm-1.0.0a9/tdm/datamodel/common/_container.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/common/_impl.py` & `talisman-dm-1.0.0a9/tdm/datamodel/common/_impl.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/common/_state.py` & `talisman-dm-1.0.0a9/tdm/datamodel/common/_state.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/common/_types.py` & `talisman-dm-1.0.0a9/tdm/datamodel/common/_types.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/common/_view.py` & `talisman-dm-1.0.0a9/tdm/datamodel/common/_view.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/directives/concept.py` & `talisman-dm-1.0.0a9/tdm/datamodel/directives/concept.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/document/_factory.py` & `talisman-dm-1.0.0a9/tdm/datamodel/document/_factory.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/document/_impl.py` & `talisman-dm-1.0.0a9/tdm/datamodel/document/_impl.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/document/_structure.py` & `talisman-dm-1.0.0a9/tdm/datamodel/document/_structure.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/domain/__init__.py` & `talisman-dm-1.0.0a9/tdm/datamodel/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/domain/_impl.py` & `talisman-dm-1.0.0a9/tdm/datamodel/domain/_impl.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/domain/types/_property.py` & `talisman-dm-1.0.0a9/tdm/datamodel/domain/types/_property.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/facts/concept.py` & `talisman-dm-1.0.0a9/tdm/datamodel/facts/concept.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/facts/links.py` & `talisman-dm-1.0.0a9/tdm/datamodel/facts/links.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/facts/mention.py` & `talisman-dm-1.0.0a9/tdm/datamodel/facts/mention.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/facts/value.py` & `talisman-dm-1.0.0a9/tdm/datamodel/facts/value.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/links/reference.py` & `talisman-dm-1.0.0a9/tdm/datamodel/links/reference.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/mentions/image.py` & `talisman-dm-1.0.0a9/tdm/datamodel/mentions/image.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/mentions/text.py` & `talisman-dm-1.0.0a9/tdm/datamodel/mentions/text.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/nodes/__init__.py` & `talisman-dm-1.0.0a9/tdm/datamodel/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/nodes/file.py` & `talisman-dm-1.0.0a9/tdm/datamodel/nodes/file.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/nodes/structure.py` & `talisman-dm-1.0.0a9/tdm/datamodel/nodes/structure.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/nodes/text.py` & `talisman-dm-1.0.0a9/tdm/datamodel/nodes/text.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/values/date.py` & `talisman-dm-1.0.0a9/tdm/datamodel/values/date.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/values/geo.py` & `talisman-dm-1.0.0a9/tdm/datamodel/values/geo.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/datamodel/values/scalar.py` & `talisman-dm-1.0.0a9/tdm/datamodel/values/scalar.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/helper.py` & `talisman-dm-1.0.0a9/tdm/helper.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/json_schema/directives.py` & `talisman-dm-1.0.0a9/tdm/json_schema/directives.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/json_schema/facts.py` & `talisman-dm-1.0.0a9/tdm/json_schema/facts.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/json_schema/mentions.py` & `talisman-dm-1.0.0a9/tdm/json_schema/mentions.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/json_schema/nodes.py` & `talisman-dm-1.0.0a9/tdm/json_schema/nodes.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/json_schema/values.py` & `talisman-dm-1.0.0a9/tdm/json_schema/values.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/legacy.py` & `talisman-dm-1.0.0a9/tdm/legacy.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/model.py` & `talisman-dm-1.0.0a9/tdm/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import ClassVar, Dict, Optional, Tuple
 
 from immutabledict import immutabledict
 from pydantic import BaseModel, PrivateAttr, root_validator
 from typing_extensions import Literal
 
 from .abstract.datamodel import AbstractDomain, AbstractNode, TalismanDocument
+from .abstract.datamodel.markup import unfreeze
 from .datamodel.document import TalismanDocumentFactory
 from .json_schema.directives import DirectivesModel
 from .json_schema.facts import FactsModel
 from .json_schema.links import NodeLinksModel
 from .json_schema.nodes import NodeModel, fill_children, serialize_node
 from .legacy import DocumentMetadataModel
 
 
 class TalismanDocumentModel(BaseModel):
     class Config:
         json_encoders = {
-            immutabledict: lambda x: dict(x)
+            immutabledict: unfreeze
         }
 
     _DEFAULT_DOMAIN: ClassVar[AbstractDomain] = None
     _domain: AbstractDomain = PrivateAttr(None)
 
     VERSION: Literal['1.0'] = ...
     id: str
```

### Comparing `talisman-dm-1.0.0a8/tdm/v0/json_schema/content.py` & `talisman-dm-1.0.0a9/tdm/v0/json_schema/content.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/_facts.py` & `talisman-dm-1.0.0a9/tdm/v0/json_schema/convert/_facts.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/_metadata.py` & `talisman-dm-1.0.0a9/tdm/v0/json_schema/convert/_metadata.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/v0/json_schema/convert/_nodes.py` & `talisman-dm-1.0.0a9/tdm/v0/json_schema/convert/_nodes.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/v0/json_schema/directive.py` & `talisman-dm-1.0.0a9/tdm/v0/json_schema/directive.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/v0/json_schema/document.py` & `talisman-dm-1.0.0a9/tdm/v0/json_schema/document.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/v0/json_schema/fact.py` & `talisman-dm-1.0.0a9/tdm/v0/json_schema/fact.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/wrapper/node/__init__.py` & `talisman-dm-1.0.0a9/tdm/wrapper/node/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/wrapper/node/_decorator.py` & `talisman-dm-1.0.0a9/tdm/wrapper/node/_decorator.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/wrapper/node/_delegate.py` & `talisman-dm-1.0.0a9/tdm/wrapper/node/_delegate.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a8/tdm/wrapper/node/_impl.py` & `talisman-dm-1.0.0a9/tdm/wrapper/node/_impl.py`

 * *Files identical despite different names*

