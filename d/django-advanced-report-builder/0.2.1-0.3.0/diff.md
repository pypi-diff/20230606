# Comparing `tmp/django-advanced-report-builder-0.2.1.tar.gz` & `tmp/django-advanced-report-builder-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-advanced-report-builder-0.2.1.tar", last modified: Fri Apr 28 16:06:48 2023, max compression
+gzip compressed data, was "django-advanced-report-builder-0.3.0.tar", last modified: Tue Jun  6 20:57:44 2023, max compression
```

## Comparing `django-advanced-report-builder-0.2.1.tar` & `django-advanced-report-builder-0.3.0.tar`

### file list

```diff
@@ -1,200 +1,201 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.275588 django-advanced-report-builder-0.2.1/
--rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       91 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)      683 2023-04-28 16:06:48.275385 django-advanced-report-builder-0.2.1/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      171 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.167868 django-advanced-report-builder-0.2.1/advanced_report_builder/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4012 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/admin.py
--rw-r--r--   0 tom        (501) staff       (20)      218 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/apps.py
--rw-r--r--   0 tom        (501) staff       (20)     3394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/columns.py
--rw-r--r--   0 tom        (501) staff       (20)       40 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/customise.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.169879 django-advanced-report-builder-0.2.1/advanced_report_builder/data_merge/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/data_merge/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3830 2023-03-06 12:34:46.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/data_merge/utils.py
--rw-r--r--   0 tom        (501) staff       (20)      951 2023-03-29 16:03:43.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/data_merge/widget.py
--rw-r--r--   0 tom        (501) staff       (20)     5477 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/duplicate.py
--rw-r--r--   0 tom        (501) staff       (20)      192 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/exceptions.py
--rw-r--r--   0 tom        (501) staff       (20)    10853 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/field_types.py
--rw-r--r--   0 tom        (501) staff       (20)    13799 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/filter_query.py
--rw-r--r--   0 tom        (501) staff       (20)     8022 2023-04-28 15:54:22.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/globals.py
--rw-r--r--   0 tom        (501) staff       (20)     1308 2023-04-17 09:39:11.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/includes.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.186137 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/
--rw-r--r--   0 tom        (501) staff       (20)    14109 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)      591 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0002_auto_20220209_1657.py
--rw-r--r--   0 tom        (501) staff       (20)     1734 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0003_auto_20220215_1219.py
--rw-r--r--   0 tom        (501) staff       (20)      955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0004_customreport.py
--rw-r--r--   0 tom        (501) staff       (20)     3623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0005_auto_20220303_0958.py
--rw-r--r--   0 tom        (501) staff       (20)      914 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0006_auto_20220310_1147.py
--rw-r--r--   0 tom        (501) staff       (20)      607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0007_auto_20220322_1939.py
--rw-r--r--   0 tom        (501) staff       (20)      827 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0008_auto_20220404_1144.py
--rw-r--r--   0 tom        (501) staff       (20)     2485 2023-04-28 15:54:41.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0009_auto_20230428_1554.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    19474 2023-04-28 15:43:12.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/models.py
--rw-r--r--   0 tom        (501) staff       (20)      532 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/report_builder.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.134033 django-advanced-report-builder-0.2.1/advanced_report_builder/static/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.136030 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.134234 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.195069 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/
--rw-r--r--   0 tom        (501) staff       (20)   334540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js
--rw-r--r--   0 tom        (501) staff       (20)   405847 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js
--rw-r--r--   0 tom        (501) staff       (20)   193925 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js
--rw-r--r--   0 tom        (501) staff       (20)     1430 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js
--rw-r--r--   0 tom        (501) staff       (20)    12893 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.195790 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/
--rw-r--r--   0 tom        (501) staff       (20)    72125 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js
--rw-r--r--   0 tom        (501) staff       (20)     2352 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.134771 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.201811 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3/js/
--rw-r--r--   0 tom        (501) staff       (20)   575002 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js
--rw-r--r--   0 tom        (501) staff       (20)   275533 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.134564 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.199284 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/
--rw-r--r--   0 tom        (501) staff       (20)   205600 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js
--rw-r--r--   0 tom        (501) staff       (20)    58945 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.134977 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dashboard/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.203090 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dashboard/js/
--rw-r--r--   0 tom        (501) staff       (20)      563 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.135176 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.210951 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/
--rwxr-xr-x   0 tom        (501) staff       (20)      578 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore
--rwxr-xr-x   0 tom        (501) staff       (20)      122 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/.travis.yml
--rwxr-xr-x   0 tom        (501) staff       (20)     1176 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt
--rwxr-xr-x   0 tom        (501) staff       (20)     3291 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.211565 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/bin/
--rwxr-xr-x   0 tom        (501) staff       (20)     1442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer
--rwxr-xr-x   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/bower.json
--rwxr-xr-x   0 tom        (501) staff       (20)     5175 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3374 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1758 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js
--rwxr-xr-x   0 tom        (501) staff       (20)     5190 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/index.js
--rwxr-xr-x   0 tom        (501) staff       (20)      920 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/package.json
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.135838 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.212613 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/
--rwxr-xr-x   0 tom        (501) staff       (20)     4390 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1324 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.137145 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.224054 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/
--rwxr-xr-x   0 tom        (501) staff       (20)     3765 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3253 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3756 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3248 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.241217 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/
--rwxr-xr-x   0 tom        (501) staff       (20)     2962 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3082 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2494 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1431 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2309 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3273 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2672 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2662 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3216 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2917 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2952 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2522 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2299 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2645 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2787 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2451 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1310 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2627 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2782 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3062 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2503 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.244223 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.136899 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.244768 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/
--rwxr-xr-x   0 tom        (501) staff       (20)     1212 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js
--rwxr-xr-x   0 tom        (501) staff       (20)   191499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js
--rwxr-xr-x   0 tom        (501) staff       (20)    72607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js
--rwxr-xr-x   0 tom        (501) staff       (20)   201158 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js
--rwxr-xr-x   0 tom        (501) staff       (20)    77072 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.245554 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/
--rwxr-xr-x   0 tom        (501) staff       (20)      442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/dark.scss
--rwxr-xr-x   0 tom        (501) staff       (20)     3887 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.249710 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/
--rwxr-xr-x   0 tom        (501) staff       (20)      266 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-checkbox.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-tooltip-errors.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss
--rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_invert.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      469 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_sortable.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/bt-tooltip-errors.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss
--rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/invert.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      465 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/sortable.scss
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.138123 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.250526 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.252047 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.252477 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/bar/
--rw-r--r--   0 tom        (501) staff       (20)     4581 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.253279 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/
--rw-r--r--   0 tom        (501) staff       (20)     1362 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html
--rw-r--r--   0 tom        (501) staff       (20)     1007 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.253687 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/line/
--rw-r--r--   0 tom        (501) staff       (20)     4020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      486 2023-04-26 11:14:19.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/modal.html
--rw-r--r--   0 tom        (501) staff       (20)      273 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/modal_field.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.254181 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/pie/
--rw-r--r--   0 tom        (501) staff       (20)     2084 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      858 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/report.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.254544 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/data_merge/
--rw-r--r--   0 tom        (501) staff       (20)     2975 2023-03-29 15:59:37.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.256645 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.257471 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/fields/
--rw-r--r--   0 tom        (501) staff       (20)      254 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/fields/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     3320 2023-04-26 11:10:44.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html
--rw-r--r--   0 tom        (501) staff       (20)      377 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/modal.html
--rw-r--r--   0 tom        (501) staff       (20)      593 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html
--rw-r--r--   0 tom        (501) staff       (20)      256 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/query_modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1127 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/report.html
--rw-r--r--   0 tom        (501) staff       (20)     8185 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.259648 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/kanban/
--rw-r--r--   0 tom        (501) staff       (20)      499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/kanban/description_modal.html
--rw-r--r--   0 tom        (501) staff       (20)     2038 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      308 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/kanban/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1961 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/kanban/report.html
--rw-r--r--   0 tom        (501) staff       (20)     3468 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/query_builder.html
--rw-r--r--   0 tom        (501) staff       (20)     9491 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/select_column.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.260903 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/single_values/
--rw-r--r--   0 tom        (501) staff       (20)     1896 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1643 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/single_values/report.html
--rw-r--r--   0 tom        (501) staff       (20)      327 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/toggle.py
--rw-r--r--   0 tom        (501) staff       (20)     3830 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/urls.py
--rw-r--r--   0 tom        (501) staff       (20)     4447 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/utils.py
--rw-r--r--   0 tom        (501) staff       (20)    12521 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/variable_date.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.266459 django-advanced-report-builder-0.2.1/advanced_report_builder/views/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    11547 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/bar_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    18240 2023-04-28 15:13:27.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/charts_base.py
--rw-r--r--   0 tom        (501) staff       (20)     3020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/custom.py
--rw-r--r--   0 tom        (501) staff       (20)     8659 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/dashboard.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.267865 django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     6801 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/datatables.py
--rw-r--r--   0 tom        (501) staff       (20)    25412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/modal.py
--rw-r--r--   0 tom        (501) staff       (20)    11394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/utils.py
--rw-r--r--   0 tom        (501) staff       (20)     8731 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/funnel_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    32161 2023-03-29 16:04:49.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/kanban.py
--rw-r--r--   0 tom        (501) staff       (20)    12985 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/line_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    21031 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/modals_base.py
--rw-r--r--   0 tom        (501) staff       (20)     8692 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/pie_charts.py
--rw-r--r--   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/report.py
--rw-r--r--   0 tom        (501) staff       (20)     8210 2023-04-28 13:58:37.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/report_utils_mixin.py
--rw-r--r--   0 tom        (501) staff       (20)     4750 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/reports.py
--rw-r--r--   0 tom        (501) staff       (20)    22838 2023-04-28 15:43:12.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/single_values.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.270701 django-advanced-report-builder-0.2.1/advanced_report_builder/views/targets/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/targets/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3021 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/targets/utils.py
--rw-r--r--   0 tom        (501) staff       (20)      898 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/targets/views.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.274844 django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      683 2023-04-28 16:06:48.000000 django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)    10896 2023-04-28 16:06:48.000000 django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-04-28 16:06:48.000000 django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)      149 2023-04-28 16:06:48.000000 django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       24 2023-04-28 16:06:48.000000 django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-04-28 16:06:48.275641 django-advanced-report-builder-0.2.1/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      974 2023-04-28 16:04:12.000000 django-advanced-report-builder-0.2.1/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.909767 django-advanced-report-builder-0.3.0/
+-rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       91 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)      683 2023-06-06 20:57:44.909494 django-advanced-report-builder-0.3.0/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      171 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.841450 django-advanced-report-builder-0.3.0/advanced_report_builder/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4012 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)      218 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/apps.py
+-rw-r--r--   0 tom        (501) staff       (20)     3394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/columns.py
+-rw-r--r--   0 tom        (501) staff       (20)       40 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/customise.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.842621 django-advanced-report-builder-0.3.0/advanced_report_builder/data_merge/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/data_merge/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3830 2023-03-06 12:34:46.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/data_merge/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      951 2023-03-29 16:03:43.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/data_merge/widget.py
+-rw-r--r--   0 tom        (501) staff       (20)     5477 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/duplicate.py
+-rw-r--r--   0 tom        (501) staff       (20)      192 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/exceptions.py
+-rw-r--r--   0 tom        (501) staff       (20)    10853 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/field_types.py
+-rw-r--r--   0 tom        (501) staff       (20)    13799 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/filter_query.py
+-rw-r--r--   0 tom        (501) staff       (20)     8022 2023-04-28 15:54:22.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/globals.py
+-rw-r--r--   0 tom        (501) staff       (20)     1308 2023-04-17 09:39:11.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/includes.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.847729 django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)    14109 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)      591 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0002_auto_20220209_1657.py
+-rw-r--r--   0 tom        (501) staff       (20)     1734 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0003_auto_20220215_1219.py
+-rw-r--r--   0 tom        (501) staff       (20)      955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0004_customreport.py
+-rw-r--r--   0 tom        (501) staff       (20)     3623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0005_auto_20220303_0958.py
+-rw-r--r--   0 tom        (501) staff       (20)      914 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0006_auto_20220310_1147.py
+-rw-r--r--   0 tom        (501) staff       (20)      607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0007_auto_20220322_1939.py
+-rw-r--r--   0 tom        (501) staff       (20)      827 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0008_auto_20220404_1144.py
+-rw-r--r--   0 tom        (501) staff       (20)     2485 2023-04-28 15:54:41.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0009_auto_20230428_1554.py
+-rw-r--r--   0 tom        (501) staff       (20)      596 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0010_auto_20230428_2033.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    19594 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/models.py
+-rw-r--r--   0 tom        (501) staff       (20)      532 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/report_builder.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.795137 django-advanced-report-builder-0.3.0/advanced_report_builder/static/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.798145 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.795384 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.853871 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/
+-rw-r--r--   0 tom        (501) staff       (20)   334540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js
+-rw-r--r--   0 tom        (501) staff       (20)   405847 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js
+-rw-r--r--   0 tom        (501) staff       (20)   193925 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js
+-rw-r--r--   0 tom        (501) staff       (20)     1430 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js
+-rw-r--r--   0 tom        (501) staff       (20)    12893 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.855049 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/
+-rw-r--r--   0 tom        (501) staff       (20)    72125 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js
+-rw-r--r--   0 tom        (501) staff       (20)     2352 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.796123 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/d3/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.858061 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/d3/js/
+-rw-r--r--   0 tom        (501) staff       (20)   575002 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js
+-rw-r--r--   0 tom        (501) staff       (20)   275533 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.795793 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.856062 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/
+-rw-r--r--   0 tom        (501) staff       (20)   205600 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js
+-rw-r--r--   0 tom        (501) staff       (20)    58945 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.796443 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dashboard/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.858991 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dashboard/js/
+-rw-r--r--   0 tom        (501) staff       (20)      563 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.796782 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.863218 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/
+-rwxr-xr-x   0 tom        (501) staff       (20)      578 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore
+-rwxr-xr-x   0 tom        (501) staff       (20)      122 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/.travis.yml
+-rwxr-xr-x   0 tom        (501) staff       (20)     1176 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt
+-rwxr-xr-x   0 tom        (501) staff       (20)     3291 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.863520 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/bin/
+-rwxr-xr-x   0 tom        (501) staff       (20)     1442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer
+-rwxr-xr-x   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/bower.json
+-rwxr-xr-x   0 tom        (501) staff       (20)     5175 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3374 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1758 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     5190 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/index.js
+-rwxr-xr-x   0 tom        (501) staff       (20)      920 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/package.json
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.797912 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.876266 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/
+-rwxr-xr-x   0 tom        (501) staff       (20)     4390 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1324 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.804210 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.884713 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/
+-rwxr-xr-x   0 tom        (501) staff       (20)     3765 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3253 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3756 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3248 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.893039 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/
+-rwxr-xr-x   0 tom        (501) staff       (20)     2962 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3082 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2494 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1431 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2309 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3273 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2672 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2662 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3216 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2917 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2952 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2522 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2299 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2645 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2787 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2451 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1310 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2627 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2782 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3062 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2503 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.895060 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.803909 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.895376 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/
+-rwxr-xr-x   0 tom        (501) staff       (20)     1212 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js
+-rwxr-xr-x   0 tom        (501) staff       (20)   191499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js
+-rwxr-xr-x   0 tom        (501) staff       (20)    72607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js
+-rwxr-xr-x   0 tom        (501) staff       (20)   201158 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js
+-rwxr-xr-x   0 tom        (501) staff       (20)    77072 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.895830 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/
+-rwxr-xr-x   0 tom        (501) staff       (20)      442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/dark.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)     3887 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.898008 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/
+-rwxr-xr-x   0 tom        (501) staff       (20)      266 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-checkbox.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-tooltip-errors.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_invert.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      469 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_sortable.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/bt-tooltip-errors.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/invert.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      465 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/sortable.scss
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.804547 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.898425 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.899163 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.899484 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/bar/
+-rw-r--r--   0 tom        (501) staff       (20)     5124 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.899902 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/
+-rw-r--r--   0 tom        (501) staff       (20)     1362 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)     1007 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.900104 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/line/
+-rw-r--r--   0 tom        (501) staff       (20)     4020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      486 2023-04-26 11:14:19.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)      270 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/modal_field.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.900324 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/pie/
+-rw-r--r--   0 tom        (501) staff       (20)     2084 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      858 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/report.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.900541 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/data_merge/
+-rw-r--r--   0 tom        (501) staff       (20)     2975 2023-03-29 15:59:37.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.901676 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/datatables/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.902077 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/
+-rw-r--r--   0 tom        (501) staff       (20)      254 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     3320 2023-04-26 11:10:44.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html
+-rw-r--r--   0 tom        (501) staff       (20)      377 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/datatables/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)      593 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html
+-rw-r--r--   0 tom        (501) staff       (20)      256 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/datatables/query_modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1127 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/datatables/report.html
+-rw-r--r--   0 tom        (501) staff       (20)     8185 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.903016 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/kanban/
+-rw-r--r--   0 tom        (501) staff       (20)      499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/kanban/description_modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     2038 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      308 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/kanban/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1961 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/kanban/report.html
+-rw-r--r--   0 tom        (501) staff       (20)     3467 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/query_builder.html
+-rw-r--r--   0 tom        (501) staff       (20)    10552 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/select_column.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.903631 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/single_values/
+-rw-r--r--   0 tom        (501) staff       (20)     1896 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1643 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/single_values/report.html
+-rw-r--r--   0 tom        (501) staff       (20)      327 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/toggle.py
+-rw-r--r--   0 tom        (501) staff       (20)     4218 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/urls.py
+-rw-r--r--   0 tom        (501) staff       (20)     4447 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)    12521 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/variable_date.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.906929 django-advanced-report-builder-0.3.0/advanced_report_builder/views/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    20624 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/bar_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    18240 2023-04-28 15:13:27.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/charts_base.py
+-rw-r--r--   0 tom        (501) staff       (20)     3020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/custom.py
+-rw-r--r--   0 tom        (501) staff       (20)     8659 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/dashboard.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.907702 django-advanced-report-builder-0.3.0/advanced_report_builder/views/datatables/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/datatables/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     6801 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/datatables/datatables.py
+-rw-r--r--   0 tom        (501) staff       (20)    25731 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/datatables/modal.py
+-rw-r--r--   0 tom        (501) staff       (20)    11394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/datatables/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     8792 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/funnel_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    32161 2023-03-29 16:04:49.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/kanban.py
+-rw-r--r--   0 tom        (501) staff       (20)    13046 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/line_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    21031 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/modals_base.py
+-rw-r--r--   0 tom        (501) staff       (20)     8753 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/pie_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/report.py
+-rw-r--r--   0 tom        (501) staff       (20)     8210 2023-04-28 13:58:37.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/report_utils_mixin.py
+-rw-r--r--   0 tom        (501) staff       (20)     4750 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/reports.py
+-rw-r--r--   0 tom        (501) staff       (20)    22923 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/single_values.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.908260 django-advanced-report-builder-0.3.0/advanced_report_builder/views/targets/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/targets/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3021 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/targets/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      898 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.3.0/advanced_report_builder/views/targets/views.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-06 20:57:44.909222 django-advanced-report-builder-0.3.0/django_advanced_report_builder.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      683 2023-06-06 20:57:44.000000 django-advanced-report-builder-0.3.0/django_advanced_report_builder.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)    10958 2023-06-06 20:57:44.000000 django-advanced-report-builder-0.3.0/django_advanced_report_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-06 20:57:44.000000 django-advanced-report-builder-0.3.0/django_advanced_report_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)      149 2023-06-06 20:57:44.000000 django-advanced-report-builder-0.3.0/django_advanced_report_builder.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       24 2023-06-06 20:57:44.000000 django-advanced-report-builder-0.3.0/django_advanced_report_builder.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-06 20:57:44.909834 django-advanced-report-builder-0.3.0/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      974 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.3.0/setup.py
```

### Comparing `django-advanced-report-builder-0.2.1/LICENSE` & `django-advanced-report-builder-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/PKG-INFO` & `django-advanced-report-builder-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-report-builder
-Version: 0.2.1
+Version: 0.3.0
 Summary: Django app that allows you to build reports from modals
 Home-page: https://github.com/django-advance-utils/django-advanced-report-builder
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/admin.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/admin.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/columns.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/columns.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/data_merge/utils.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/data_merge/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/data_merge/widget.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/data_merge/widget.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/duplicate.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/duplicate.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/field_types.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/field_types.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/filter_query.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/filter_query.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/globals.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/globals.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/includes.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/includes.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0001_initial.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0002_auto_20220209_1657.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0002_auto_20220209_1657.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0003_auto_20220215_1219.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0003_auto_20220215_1219.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0004_customreport.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0004_customreport.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0005_auto_20220303_0958.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0005_auto_20220303_0958.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0006_auto_20220310_1147.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0006_auto_20220310_1147.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0007_auto_20220322_1939.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0007_auto_20220322_1939.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0008_auto_20220404_1144.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0008_auto_20220404_1144.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0009_auto_20230428_1554.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/migrations/0009_auto_20230428_1554.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/models.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,14 +287,17 @@
 
     bar_chart_orientation = models.PositiveSmallIntegerField(choices=BAR_CHART_ORIENTATION_CHOICES,
                                                              default=BAR_CHART_ORIENTATION_VERTICAL)
     stacked = models.BooleanField(default=False)
     show_totals = models.BooleanField(default=False)
     show_blank_dates = models.BooleanField(default=True)
 
+    show_breakdown = models.BooleanField(default=False)
+    breakdown_fields = models.JSONField(null=True, blank=True)
+
     def is_orientation_vertical(self):
         return self.bar_chart_orientation == self.BAR_CHART_ORIENTATION_VERTICAL
 
     def get_chart_scale(self):
         return ANNOTATION_CHART_SCALE[self.axis_scale]
```

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/report_builder.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/report_builder.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/README.md` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/README.md`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/index.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/index.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/package.json` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/dot/js/package.json`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss` & `django-advanced-report-builder-0.3.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 {% load ajax_helpers %}
 
 <canvas id="{{ datatable.table_id }}" width="400" height="400"></canvas>
 
 <script>
-
-
     (function () {
-
         var cell_data;
         var table = {{ datatable.model_table_setup }};
         table.find_column = django_datatables.PythonTable.prototype.find_column
-
         var labels = [];
         var datasets = [];
 
         for (var i = 0; i < table.initsetup.colOptions.length; i++) {
-
             if (i > 0) {
                 datasets[i - 1] = {
                     label: table.row_titles[i],
                     data: [],
                     borderWidth: 1,
                     datalabels: {
                         align: 'top',
@@ -67,42 +62,34 @@
                 },
             {% endif %}
             {% if datatable.bar_chart_report.show_blank_dates %}
                 type: 'time',
                 time: {
                     unit: '{{ datatable.bar_chart_report.get_chart_scale}}'
                 }
-
             {% endif %}
-
         };
-
         var y_axis = {
             {% if datatable.bar_chart_report.stacked %}stacked: true,{% endif %}
-
             display: true,
             {% if datatable.bar_chart_report.y_label %}
                 title: {
                     display: true,
                     text: '{% if datatable.bar_chart_report.is_orientation_vertical %}{{ datatable.bar_chart_report.y_label|safe|escapejs }}{% else %}{{ datatable.bar_chart_report.x_label|safe|escapejs }}{% endif %}',
                 }
             {% endif %}
         };
         var ctx{{ datatable.table_id }} = document.getElementById('{{ datatable.table_id }}').getContext('2d');
-
-
-
         var bar{{ datatable.table_id }} = new Chart(ctx{{ datatable.table_id }}, {
             {% if datatable.bar_chart_report.show_totals %}plugins: [ChartDataLabels],{% endif %}
             type: 'bar',
             data: {labels: labels, datasets: datasets},
             options: {
                 maintainAspectRatio: false,
                 {% if not datatable.bar_chart_report.is_orientation_vertical %}indexAxis: 'y',{% endif %}
-
                 scales: {
                     // This is because there is a bug in the library,
                     // where the axis label don't swap properly on orientation change.
                     {% if datatable.bar_chart_report.is_orientation_vertical %}
                         y: y_axis,
                         x: x_axis,
                     {% else %}
@@ -110,13 +97,23 @@
                         x: y_axis,
                     {% endif %}
                 },
                 responsive: true,
                 legend: {
                     position: 'top',
                     display: false
-                },
+                }{% if datatable.bar_chart_report.show_breakdown %},
+               onClick: function (e, items){
+                     if (items.length === 0) {
+                         return
+                     }
+                     let _date = (table['data'][items[0].index][0]).replaceAll("-", "_");
+                     let breakdown_url = "{{ datatable.breakdown_url }}".replace(
+                         "99999",  items[0].datasetIndex).replace("88888", _date);
+                     django_modal.show_modal(breakdown_url);
+               }
+              {% endif %}
             }
         });
 
     })();
 </script>
```

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/report.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/charts/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/report.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/datatables/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/kanban/report.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/kanban/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/query_builder.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/query_builder.html`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,13 @@
                 let results = query_builder.queryBuilder('getRules', {skip_empty: true});
                 $(field_id).val(JSON.stringify(results, null, 2));
                 return results;
             }
 
 }( window.{{ field.auto_id }} = window.{{ field.auto_id }} || {}, jQuery ));
 
-
     ajax_helpers.command_functions.save_query_builder_{{ field.auto_id }} = function (command) {
         {{ field.auto_id }}.save_query_builder();
     };
 
     </script>
 </div>
```

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/select_column.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/select_column.html`

 * *Files 22% similar despite different names*

```diff
@@ -61,152 +61,153 @@
             <div id="{{ field.auto_id }}_keys" class="col-3">
 
             </div>
         </div>
     </div>
             <script>
             $(function () {
-                let selection_fields_id_name = '#{{ field.auto_id }}_selection';
-                let available_fields_id_name = '#{{ field.auto_id }}_available_fields';
-                let table_field_keys = '#{{ field.auto_id }}_keys';
-                let main_field = '#{{ field.auto_id }}';
-                let available_fields_data = {};
-                let initial = true;
+                let {{ command_prefix }}selection_fields_id_name = '#{{ field.auto_id }}_selection';
+                let {{ command_prefix }}available_fields_id_name = '#{{ field.auto_id }}_available_fields';
+                let {{ command_prefix }}table_field_keys = '#{{ field.auto_id }}_keys';
+                let {{ command_prefix }}main_field = '#{{ field.auto_id }}';
+                let {{ command_prefix }}available_fields_data = {};
+                let {{ command_prefix }}initial = true;
 
-                function get_field_html(field_id, label, colour, attr) {
+                function {{ command_prefix }}get_field_html(field_id, label, colour, attr) {
                     let data_attr = '';
                     if(attr !== undefined && attr !== '') {
                         data_attr = ` data-attr="${attr}"`
                     }
                     return `<li class="ui-state-default" data-origin="${field_id}" style="background-color: ${colour}"${data_attr}>
-                            <a href="#" class="edit_field_link"><i class="edit-field fas fa-pencil-alt float-right" style="color:white;"></i></a><span>${label}</span></li>`
+                            <a href="#" class="{{ command_prefix }}edit_field_link"><i class="edit-field fas fa-pencil-alt float-right" style="color:white;"></i></a><span>${label}</span></li>`
                 }
 
-                ajax_helpers.command_functions.report_fields = function (command) {
+                ajax_helpers.command_functions.{{ command_prefix }}report_fields = function (command) {
                     let data = jQuery.parseJSON(command.data);
-                    $(selection_fields_id_name).empty();
-                    $(available_fields_id_name).empty();
-                    $(table_field_keys).empty();
-                    available_fields_data = {};
+                    $({{ command_prefix }}selection_fields_id_name).empty();
+                    $({{ command_prefix }}available_fields_id_name).empty();
+                    $({{ command_prefix }}table_field_keys).empty();
+                    {{ command_prefix }}available_fields_data = {};
                     $.each(data['fields'], function (key, value) {
-                        available_fields_data[value.field] = value;
-                        $(available_fields_id_name).append(get_field_html(value.field, value.label, value.colour, ''));
+                        {{ command_prefix }}available_fields_data[value.field] = value;
+                        $({{ command_prefix }}available_fields_id_name).append({{ command_prefix }}get_field_html(value.field, value.label, value.colour, ''));
                     });
                     $.each(data['tables'], function (key, value) {
-                        $(table_field_keys).append('<div class="col-sm-12" style=";font-size: 12px;">' +
+                        $({{ command_prefix }}table_field_keys).append('<div class="col-sm-12" style=";font-size: 12px;">' +
                             '<i class="fa fa-square fa-2x" style="opacity:1;color: ' + value.colour + '"></i>' +
                             ' <span>' + value.name + '</span></div>');
                     });
-                    if(initial) {
-                        load_section();
-                        initial = false;
+                    if({{ command_prefix }}initial) {
+                        {{ command_prefix }}load_section();
+                        {{ command_prefix }}initial = false;
                     } else {
-                        $(main_field).val('[]')
+                        $({{ command_prefix }}main_field).val('[]')
                     }
 
-                    $('.edit_field_link').click(function(){
+                    $('.{{ command_prefix }}edit_field_link').click(function(){
                         let selector = 's' + String(new Date().getTime());
                         let parent_li = $(this).parent()
                         parent_li.attr('id', selector);
-                        let field_info = get_field_dict(parent_li);
+                        let field_info = {{ command_prefix }}get_field_dict(parent_li);
                         let field_info_b64 = (btoa(JSON.stringify(field_info)));
                         let url = "{{ select_column_url }}";
                         django_modal.show_modal(url.replace('99999', selector).replace('REPORT_TYPE_ID', $('#id_report_type').val()).replace('FIELD_INFO', field_info_b64))
                     });
 
                 }
 
-                $(selection_fields_id_name + ', ' + available_fields_id_name).sortable({
+                $({{ command_prefix }}selection_fields_id_name + ', ' + {{ command_prefix }}available_fields_id_name).sortable({
                     connectWith: ".connectedSortable",
                     stop: function () {
-                        update_selection();
+                        {{ command_prefix }}update_selection();
                     },
                     receive: function (event, ui) { //only when dropped from one to another!
                         let sourceList = ui.sender;
                         if(sourceList.attr('id') === '{{ field.auto_id }}_available_fields') {
                             let clone = $(ui.item).clone();
                             sourceList.append(clone);  // adds it back to the end
                         } else {
                             ui.item.remove();  // removes it as it already in the list
                         }
                     }
 
                 });
 
                 $('#id_report_type').on('change', function (e) {
-                    get_fields(this.value);
+                    {{ command_prefix }}get_fields(this.value);
                 });
                 $(document).ready(function () {
-                    get_fields($('#id_report_type').val());
+                    {{ command_prefix }}get_fields($('#id_report_type').val());
                 });
 
-                function get_fields(report_type_id) {
+                function {{ command_prefix }}get_fields(report_type_id) {
                     if (report_type_id === '') {
-                        $(selection_fields_id_name).empty();
-                        $(available_fields_id_name).empty();
-                        $(table_field_keys).empty();
+                        $({{ command_prefix }}selection_fields_id_name).empty();
+                        $({{ command_prefix }}available_fields_id_name).empty();
+                        $({{ command_prefix }}table_field_keys).empty();
                     } else {
-                        django_modal.send_inputs({'ajax': 'get_fields'})
+                        django_modal.send_inputs({'ajax': 'get_{{ command_prefix }}fields', 'field_auto_id': '{{ field.auto_id }}'})
                     }
                 }
 
 
-                function update_selection() {
+                function {{ command_prefix }}update_selection() {
                     let fields_selection = [];
-                    $(selection_fields_id_name).children().each(function () {
-                        fields_selection.push(get_field_dict($(this)))
+                    $({{ command_prefix }}selection_fields_id_name).children().each(function () {
+                        fields_selection.push({{ command_prefix }}get_field_dict($(this)))
                     });
-                    $(main_field).val(JSON.stringify(fields_selection))
+                    $({{ command_prefix }}main_field).val(JSON.stringify(fields_selection))
                 }
 
-                function get_field_dict(field) {
+                function {{ command_prefix }}get_field_dict(field) {
                     let data_origin = field.attr('data-origin');
                     let title = field.children("span").text()
                     let result = {
                         'field': data_origin,
                         'title': title,
                     };
                     let data_attr = field.attr('data-attr');
 
                     if(data_attr) {
                         result['data_attr'] = data_attr;
                     }
                     return result;
                 }
 
-                function load_section() {
-                    if($(main_field).val() !== '') {
-                        let fields = JSON.parse($(main_field).val())
+                function {{ command_prefix }}load_section() {
+
+                    if($({{ command_prefix }}main_field).val() !== '') {
+                        let fields = JSON.parse($({{ command_prefix }}main_field).val())
                         $.each(fields, function (key, value) {
-                            let field_data = available_fields_data[value.field];
-                            $(selection_fields_id_name).append(get_field_html(value.field, value.title, field_data.colour, value.data_attr));
+                            let field_data = {{ command_prefix }}available_fields_data[value.field];
+                            $({{ command_prefix }}selection_fields_id_name).append({{ command_prefix }}get_field_html(value.field, value.title, field_data.colour, value.data_attr));
                         });
                     }
                 }
                 $('#{{ field.auto_id }}_selected_search_input').keyup(function() {
-                    search_fields(this.value, selection_fields_id_name);
+                    {{ command_prefix }}search_fields(this.value, {{ command_prefix }}selection_fields_id_name);
                 })
                 $('#{{ field.auto_id }}_field_search_input').keyup(function() {
-                    search_fields(this.value, available_fields_id_name);
+                    {{ command_prefix }}search_fields(this.value, {{ command_prefix }}available_fields_id_name);
                 })
 
 
-                function search_fields(searchString, area_id) {
+                function {{ command_prefix }}search_fields(searchString, area_id) {
                     searchString = searchString.toUpperCase();
                     $(area_id + " li").each(function (index, value) {
                         let currentName = $(value).text()
                         if (currentName.toUpperCase().indexOf(searchString) > -1) {
                             $(value).show();
                         } else {
                             $(value).hide();
                         }
                     });
                 }
 
-                ajax_helpers.command_functions.update_selection = function (command) {
+                ajax_helpers.command_functions.{{ command_prefix }}update_selection = function (command) {
 
-                    update_selection();
+                    {{ command_prefix }}update_selection();
                 };
             });
         </script>
 </div>
 <input type="hidden" name="{{ field.name }}" id="{{ field.auto_id }}" value="{% if field.value %}{{ field.value }}{% endif %}">
```

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/single_values/report.html` & `django-advanced-report-builder-0.3.0/advanced_report_builder/templates/advanced_report_builder/single_values/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/urls.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 from django.urls import path
 
-from advanced_report_builder.views.bar_charts import BarChartModal, BarChartFieldModal
+from advanced_report_builder.views.bar_charts import BarChartModal, BarChartFieldModal, BarChartShowBreakdownModal, \
+    BarChartBreakdownFieldModal
 from advanced_report_builder.views.custom import CustomModal
 from advanced_report_builder.views.dashboard import DashboardReportModal, DashboardModal, DashboardAddReportModal
 from advanced_report_builder.views.datatables.modal import TableModal, TableFieldModal, TablePivotModal, TableQueryModal
 from advanced_report_builder.views.funnel_charts import FunnelChartModal, FunnelChartFieldModal
 from advanced_report_builder.views.kanban import KanbanModal, KanbanLaneModal, KanbanLaneDuplicateModal, \
     KanbanDescriptionModal, KanbanDescriptionDuplicateModal
 from advanced_report_builder.views.line_charts import LineChartModal, LineChartFieldModal
 from advanced_report_builder.views.pie_charts import PieChartModal, PieChartFieldModal
 from advanced_report_builder.views.reports import DuplicateReportModal
-from advanced_report_builder.views.single_values import SingleValueModal, ShowBreakdownModal, SingleValueTableFieldModal
+from advanced_report_builder.views.single_values import SingleValueModal, SingleValueShowBreakdownModal, SingleValueTableFieldModal
 from advanced_report_builder.views.targets.views import TargetModal
 
 app_name = 'advanced_report_builder'
 
 
 urlpatterns = [
     path('table/modal/<str:slug>/', TableModal.as_view(), name='table_modal'),
     path('table/modal/field/<str:slug>/', TableFieldModal.as_view(), name='table_field_modal'),
     path('table/modal/pivot/<str:slug>/', TablePivotModal.as_view(), name='table_pivot_modal'),
     path('table/modal/query/<str:slug>', TableQueryModal.as_view(), name='table_query_modal'),
 
     path('single-value/modal/<str:slug>/', SingleValueModal.as_view(), name='single_value_modal'),
     path('single-value/modal/field/<str:slug>/', SingleValueTableFieldModal.as_view(), name='single_value_field_modal'),
-    path('single-value/show-breakdown/<str:slug>/', ShowBreakdownModal.as_view(), name='show_breakdown_modal'),
+    path('single-value/show-breakdown/<str:slug>/', SingleValueShowBreakdownModal.as_view(),
+         name='single_value_show_breakdown_modal'),
 
     path('bar-chart/modal/<str:slug>/', BarChartModal.as_view(), name='bar_chart_modal'),
     path('bar-chart/modal/field/<str:slug>/', BarChartFieldModal.as_view(), name='bar_chart_field_modal'),
+    path('bar-chart/modal/breakdown/field/<str:slug>/',
+         BarChartBreakdownFieldModal.as_view(), name='bar_chart_breakdown_field_modal'),
+    path('bar-chart/show-breakdown/<str:slug>/', BarChartShowBreakdownModal.as_view(),
+         name='bar_chart_show_breakdown_modal'),
 
     path('line-chart/modal/<str:slug>/', LineChartModal.as_view(), name='line_chart_modal'),
     path('line-chart/modal/field/<str:slug>/', LineChartFieldModal.as_view(), name='line_chart_field_modal'),
 
     path('pie-chart/modal/<str:slug>/', PieChartModal.as_view(), name='pie_chart_modal'),
     path('pie-chart/modal/field/<str:slug>/', PieChartFieldModal.as_view(), name='pie_chart_field_modal'),
```

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/utils.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/variable_date.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/variable_date.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/bar_charts.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/funnel_charts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,164 +1,108 @@
 import base64
 import json
 
 from crispy_forms.layout import Div
-from django.core.exceptions import FieldDoesNotExist
 from django.forms import CharField, ChoiceField, BooleanField
-from django.shortcuts import get_object_or_404
 from django.urls import reverse
 from django_menus.menu import MenuItem
 from django_modals.fields import FieldEx
 from django_modals.form_helpers import HorizontalNoEnterHelper
 from django_modals.modals import FormModal
 from django_modals.processes import PROCESS_EDIT_DELETE, PERMISSION_OFF
 from django_modals.widgets.colour_picker import ColourPickerWidget
 from django_modals.widgets.select2 import Select2Multiple
 
-from advanced_report_builder.exceptions import ReportError
-from advanced_report_builder.globals import DEFAULT_DATE_FORMAT, \
-    DATE_FORMAT_TYPES_DJANGO_FORMAT
-from advanced_report_builder.models import BarChartReport, ReportType
+from advanced_report_builder.models import FunnelChartReport
 from advanced_report_builder.toggle import RBToggle
 from advanced_report_builder.utils import split_attr, encode_attribute, decode_attribute
 from advanced_report_builder.views.charts_base import ChartBaseView, ChartBaseFieldForm
 from advanced_report_builder.views.modals_base import QueryBuilderModalBaseMixin, QueryBuilderModalBase
 
 
-class BarChartView(ChartBaseView):
+class FunnelChartView(ChartBaseView):
+    use_annotations = False
+
+    template_name = 'advanced_report_builder/charts/funnel/report.html'
 
     def dispatch(self, request, *args, **kwargs):
         self.report = kwargs.get('report')
-        self.chart_report = self.report.barchartreport
+        self.chart_report = self.report.funnelchartreport
         return super().dispatch(request, *args, **kwargs)
 
     def get_context_data(self, **kwargs):
-        try:
-            context = super().get_context_data(**kwargs)
-        except FieldDoesNotExist as e:
-            raise ReportError(e)
-        self.table.bar_chart_report = self.chart_report
-        self.table.datatable_template = 'advanced_report_builder/charts/bar/middle.html'
-        context['bar_chart_report'] = self.chart_report
+        context = super().get_context_data(**kwargs)
+        self.table.funnel_chart_report = self.chart_report
+        self.table.datatable_template = 'advanced_report_builder/charts/funnel/middle.html'
+        context['funnel_chart_report'] = self.chart_report
         return context
 
-    def get_date_format(self):
-        if self.chart_report.show_blank_dates:
-            date_format = '%Y-%m-%d'
-        else:
-            default_format_type = DEFAULT_DATE_FORMAT[self.chart_report.axis_scale]
-            date_format = DATE_FORMAT_TYPES_DJANGO_FORMAT[default_format_type]
-        return date_format
-
     def set_extra_number_field_kwargs(self, data_attr, options, multiple_index):
-        negative_bar_colour = data_attr.get('negative_bar_colour') or '801C70'
-        positive_bar_colour = data_attr.get('positive_bar_colour') or '801C70'
-        negative_bar_colour = self.add_colour_offset(negative_bar_colour, multiple_index=multiple_index)
-        positive_bar_colour = self.add_colour_offset(positive_bar_colour, multiple_index=multiple_index)
-
-        options.update({'colours': {'negative': negative_bar_colour,
-                                    'positive': positive_bar_colour}})
+        funnel_colour = data_attr.get('funnel_colour') or '801C70'
+        funnel_colour = self.add_colour_offset(funnel_colour, multiple_index=multiple_index)
+        options.update({'colour': funnel_colour})
 
     def edit_report_menu(self, request, chart_report_id, slug_str):
-        return [MenuItem(f'advanced_report_builder:bar_chart_modal,pk-{chart_report_id}{slug_str}',
+        return [MenuItem(f'advanced_report_builder:funnel_chart_modal,pk-{chart_report_id}{slug_str}',
                          menu_display='Edit',
                          font_awesome='fas fa-pencil-alt', css_classes=['btn-primary']),
-                *self.duplicate_menu(request=self.request, report_id=chart_report_id)
-                ]
+                *self.duplicate_menu(request=self.request, report_id=chart_report_id)]
+
+    def get_date_field(self, index, fields, base_model, table):
+        return None
 
 
-class BarChartModal(QueryBuilderModalBase):
+class FunnelChartModal(QueryBuilderModalBase):
     template_name = 'advanced_report_builder/charts/modal.html'
     process = PROCESS_EDIT_DELETE
     permission_delete = PERMISSION_OFF
-    model = BarChartReport
-    widgets = {'positive_bar_colour': ColourPickerWidget,
-               'negative_bar_colour': ColourPickerWidget,
-               'stacked': RBToggle,
-               'show_totals': RBToggle,
-               'show_blank_dates': RBToggle,
-               'report_tags': Select2Multiple}
+    model = FunnelChartReport
+    widgets = {'report_tags': Select2Multiple}
 
     form_fields = ['name',
                    'notes',
                    'report_type',
                    'report_tags',
-                   ('bar_chart_orientation', {'label': 'Orientation'}),
                    'axis_value_type',
-                   'axis_scale',
-                   'date_field',
                    'fields',
-                   'x_label',
-                   'y_label',
-                   'stacked',
-                   'show_totals',
-                   'show_blank_dates',
                    ]
 
     def form_setup(self, form, *_args, **_kwargs):
-        if 'data' in _kwargs:
-            date_field = _kwargs['data'].get('date_field')
-            report_type_id = _kwargs['data'].get('report_type')
-            report_type = get_object_or_404(ReportType, id=report_type_id)
-        else:
-            date_field = form.instance.date_field
-            report_type = form.instance.report_type
-
-        self.setup_field(field_type='date',
-                         form=form,
-                         field_name='date_field',
-                         selected_field_id=date_field,
-                         report_type=report_type)
-
-        form.fields['notes'].widget.attrs['rows'] = 3
 
         self.add_query_data(form)
-        url = reverse('advanced_report_builder:bar_chart_field_modal',
+
+        url = reverse('advanced_report_builder:funnel_chart_field_modal',
                       kwargs={'slug': 'selector-99999-data-FIELD_INFO-report_type_id-REPORT_TYPE_ID'})
 
         return ('name',
                 'notes',
                 'report_type',
                 'report_tags',
-                'bar_chart_orientation',
-                'axis_scale',
                 'axis_value_type',
-                'date_field',
                 FieldEx('fields',
                         template='advanced_report_builder/select_column.html',
-                        extra_context={'select_column_url': url}),
-                'x_label',
-                'y_label',
-                'stacked',
-                'show_totals',
-                'show_blank_dates',
+                        extra_context={'select_column_url': url,
+                                       'command_prefix': ''}),
                 FieldEx('query_data',
                         template='advanced_report_builder/query_builder.html'),
                 )
 
-    def select2_date_field(self, **kwargs):
-        return self.get_fields_for_select2(field_type='date',
-                                           report_type=kwargs['report_type'],
-                                           search_string=kwargs.get('search'))
 
-
-class BarChartFieldForm(ChartBaseFieldForm):
+class FunnelChartFieldForm(ChartBaseFieldForm):
 
     def setup_modal(self, *args, **kwargs):
         data = json.loads(base64.b64decode(self.slug['data']))
         report_type, base_model = self.get_report_type_details()
 
         data_attr = split_attr(data)
 
         self.fields['title'] = CharField(initial=data['title'])
 
-        self.fields['positive_bar_colour'] = CharField(required=False, widget=ColourPickerWidget)
-        self.fields['negative_bar_colour'] = CharField(required=False, widget=ColourPickerWidget)
-        self.fields['positive_bar_colour'].initial = data_attr.get('positive_bar_colour')
-        self.fields['negative_bar_colour'].initial = data_attr.get('negative_bar_colour')
+        self.fields['funnel_colour'] = CharField(required=False, widget=ColourPickerWidget)
+        self.fields['funnel_colour'].initial = data_attr.get('funnel_colour')
 
         self.fields['has_filter'] = BooleanField(required=False, widget=RBToggle())
         self.fields['filter'] = CharField(required=False)
 
         if data_attr.get('has_filter') == '1':
             self.fields['has_filter'].initial = True
             if 'filter' in data_attr:
@@ -180,35 +124,33 @@
 
         super().setup_modal(*args, **kwargs)
 
     def get_additional_attributes(self):
         attributes = []
         self.get_report_type_details()
 
-        attributes.append(f'positive_bar_colour-{self.cleaned_data["positive_bar_colour"]}')
-        attributes.append(f'negative_bar_colour-{self.cleaned_data["negative_bar_colour"]}')
+        attributes.append(f'funnel_colour-{self.cleaned_data["funnel_colour"]}')
 
         if self.cleaned_data['has_filter']:
             attributes.append('has_filter-1')
 
             if self.cleaned_data['filter']:
                 b64_filter = encode_attribute(self.cleaned_data['filter'])
                 attributes.append(f'filter-{b64_filter}')
-
             if self.cleaned_data['multiple_columns']:
                 attributes.append('multiple_columns-1')
                 attributes.append(f'multiple_column_field-{self.cleaned_data["multiple_column_field"]}')
 
         if attributes:
             return '-'.join(attributes)
         return None
 
 
-class BarChartFieldModal(QueryBuilderModalBaseMixin, FormModal):
-    form_class = BarChartFieldForm
+class FunnelChartFieldModal(QueryBuilderModalBaseMixin, FormModal):
+    form_class = FunnelChartFieldForm
     size = 'xl'
     template_name = 'advanced_report_builder/charts/modal_field.html'
     no_header_x = True
     helper_class = HorizontalNoEnterHelper
 
     @property
     def modal_title(self):
@@ -235,16 +177,15 @@
             {'selector': '#filter_fields_div', 'values': {'checked': 'show'}, 'default': 'hide'}])
 
         form.add_trigger('multiple_columns', 'onchange', [
             {'selector': '#multiple_columns_fields_div', 'values': {'checked': 'show'}, 'default': 'hide'},
         ])
 
         return ['title',
-                'positive_bar_colour',
-                'negative_bar_colour',
+                'funnel_colour',
                 Div(FieldEx('has_filter',
                             template='django_modals/fields/label_checkbox.html',
                             field_class='col-6 input-group-sm'),
                     Div(
                         FieldEx('filter',
                                 template='advanced_report_builder/datatables/fields/single_query_builder.html'),
                         FieldEx('multiple_columns',
```

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/charts_base.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/charts_base.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/custom.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/custom.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/dashboard.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/datatables.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/datatables/datatables.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/modal.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/datatables/modal.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,15 +96,16 @@
                   FieldEx('has_clickable_rows', template='django_modals/fields/label_checkbox.html'),
                   'link_field',
                   'order_by_field',
                   FieldEx('order_by_ascending', template='django_modals/fields/label_checkbox.html'),
                   FieldEx('page_length', template='django_modals/fields/label_checkbox.html'),
                   FieldEx('table_fields',
                           template='advanced_report_builder/select_column.html',
-                          extra_context={'select_column_url': url}),
+                          extra_context={'select_column_url': url,
+                                         'command_prefix': ''}),
                   FieldEx('pivot_fields',
                           template='advanced_report_builder/datatables/select_pivot.html',
                           extra_context={'select_column_url': pivot_url}),
                   ]
 
         if self.object.id:
 
@@ -279,17 +280,19 @@
             if 'date_format' in data_attr:
                 self.fields['date_format'].initial = data_attr['date_format']
         elif self.django_field is not None and isinstance(self.django_field, NUMBER_FIELDS):
             self.fields['annotations_type'] = ChoiceField(choices=[(0, '-----')] + ANNOTATIONS_CHOICES,
                                                           required=False)
             if 'annotations_type' in data_attr:
                 self.fields['annotations_type'].initial = data_attr['annotations_type']
-            self.fields['show_totals'] = BooleanField(required=False, widget=RBToggle())
+            self.fields['show_table_totals'] = BooleanField(required=False,
+                                                            widget=RBToggle(),
+                                                            label='Show totals')
             if 'show_totals' in data_attr and data_attr['show_totals'] == '1':
-                self.fields['show_totals'].initial = True
+                self.fields['show_table_totals'].initial = True
             self.fields['decimal_places'] = IntegerField()
             self.fields['decimal_places'].initial = int(data_attr.get('decimal_places', 0))
             self.fields['has_filter'] = BooleanField(required=False, widget=RBToggle())
 
             self.fields['filter'] = CharField(required=False)
 
             if data_attr.get('has_filter') == '1':
@@ -307,17 +310,19 @@
 
             self.fields['multiple_column_field'] = ChoiceField(choices=fields, required=False)
 
             if data_attr.get('multiple_columns') == '1':
                 self.fields['multiple_columns'].initial = True
                 self.fields['multiple_column_field'].initial = data_attr.get('multiple_column_field')
         elif isinstance(self.col_type_override, CURRENCY_COLUMNS):
-            self.fields['show_totals'] = BooleanField(required=False, widget=RBToggle())
+            self.fields['show_table_totals'] = BooleanField(required=False,
+                                                            widget=RBToggle(),
+                                                            label='Show totals')
             if 'show_totals' in data_attr and data_attr['show_totals'] == '1':
-                self.fields['show_totals'].initial = True
+                self.fields['show_table_totals'].initial = True
         elif isinstance(self.col_type_override, LINK_COLUMNS):
             self.fields['link_html'] = CharField(required=False)
             if 'link_html' in data_attr:
                 self.fields['link_html'].initial = decode_attribute(data_attr['link_html'])
             self.fields['link_css'] = CharField(required=False)
             if 'link_css' in data_attr:
                 self.fields['link_css'].initial = decode_attribute(data_attr['link_css'])
@@ -338,28 +343,28 @@
             if self.cleaned_data['annotations_value']:
                 attributes.append(f'annotations_value-{self.cleaned_data["annotations_value"]}')
             if self.cleaned_data['date_format']:
                 attributes.append(f'date_format-{self.cleaned_data["date_format"]}')
         elif self.django_field is not None and isinstance(self.django_field, NUMBER_FIELDS):
             if int(self.cleaned_data['annotations_type']) != 0:
                 attributes.append(f'annotations_type-{self.cleaned_data["annotations_type"]}')
-            if self.cleaned_data['show_totals'] and self.cleaned_data["show_totals"]:
+            if self.cleaned_data['show_table_totals']:
                 attributes.append('show_totals-1')
             if self.cleaned_data['decimal_places'] > 0:
                 attributes.append(f'decimal_places-{self.cleaned_data["decimal_places"]}')
             if self.cleaned_data['has_filter']:
                 attributes.append(f'has_filter-1')
                 if self.cleaned_data['filter']:
                     b64_filter = encode_attribute(self.cleaned_data['filter'])
                     attributes.append(f'filter-{b64_filter}')
                 if self.cleaned_data['multiple_columns']:
                     attributes.append('multiple_columns-1')
                     attributes.append(f'multiple_column_field-{self.cleaned_data["multiple_column_field"]}')
         elif isinstance(self.col_type_override, CURRENCY_COLUMNS):
-            if self.cleaned_data['show_totals'] and self.cleaned_data["show_totals"]:
+            if self.cleaned_data['show_table_totals']:
                 attributes.append('show_totals-1')
         elif isinstance(self.col_type_override, LINK_COLUMNS):
             if self.cleaned_data['link_css']:
                 b64_link_css = encode_attribute(self.cleaned_data['link_css'])
                 attributes.append(f'link_css-{b64_link_css}')
             if self.cleaned_data['link_html']:
                 b64_link_html = encode_attribute(self.cleaned_data['link_html'])
@@ -416,15 +421,15 @@
 
             form.add_trigger('multiple_columns', 'onchange', [
                 {'selector': '#multiple_columns_fields_div', 'values': {'checked': 'show'}, 'default': 'hide'},
             ])
 
             return ['title',
                     'annotations_type',
-                    'show_totals',
+                    'show_table_totals',
                     'decimal_places',
                     Div(FieldEx('has_filter',
                                 template='django_modals/fields/label_checkbox.html',
                                 field_class='col-6 input-group-sm'),
                         Div(
                             FieldEx('filter',
                                     template='advanced_report_builder/datatables/fields/single_query_builder.html'),
@@ -435,15 +440,15 @@
                                 FieldEx('multiple_column_field'),
                                 css_id='multiple_columns_fields_div'),
                             css_id='filter_fields_div'),
                         css_id='annotations_fields_div')
                     ]
         elif isinstance(col_type_override, CURRENCY_COLUMNS):
             return ['title',
-                    'show_totals']
+                    'show_table_totals']
         elif isinstance(col_type_override, LINK_COLUMNS):
             return ['title',
                     'link_css',
                     'link_html',
                     'is_icon']
 
     def ajax_get_query_builder_fields(self, **kwargs):
```

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/utils.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/datatables/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/funnel_charts.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/pie_charts.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,100 +8,101 @@
 from django_modals.fields import FieldEx
 from django_modals.form_helpers import HorizontalNoEnterHelper
 from django_modals.modals import FormModal
 from django_modals.processes import PROCESS_EDIT_DELETE, PERMISSION_OFF
 from django_modals.widgets.colour_picker import ColourPickerWidget
 from django_modals.widgets.select2 import Select2Multiple
 
-from advanced_report_builder.models import FunnelChartReport
+from advanced_report_builder.models import PieChartReport
 from advanced_report_builder.toggle import RBToggle
 from advanced_report_builder.utils import split_attr, encode_attribute, decode_attribute
 from advanced_report_builder.views.charts_base import ChartBaseView, ChartBaseFieldForm
 from advanced_report_builder.views.modals_base import QueryBuilderModalBaseMixin, QueryBuilderModalBase
 
 
-class FunnelChartView(ChartBaseView):
+class PieChartView(ChartBaseView):
     use_annotations = False
 
-    template_name = 'advanced_report_builder/charts/funnel/report.html'
-
     def dispatch(self, request, *args, **kwargs):
         self.report = kwargs.get('report')
-        self.chart_report = self.report.funnelchartreport
+        self.chart_report = self.report.piechartreport
         return super().dispatch(request, *args, **kwargs)
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
-        self.table.funnel_chart_report = self.chart_report
-        self.table.datatable_template = 'advanced_report_builder/charts/funnel/middle.html'
-        context['funnel_chart_report'] = self.chart_report
+        self.table.pie_chart_report = self.chart_report
+        self.table.datatable_template = 'advanced_report_builder/charts/pie/middle.html'
+        context['pie_chart_report'] = self.chart_report
         return context
 
     def set_extra_number_field_kwargs(self, data_attr, options, multiple_index):
-        funnel_colour = data_attr.get('funnel_colour') or '801C70'
-        funnel_colour = self.add_colour_offset(funnel_colour, multiple_index=multiple_index)
-        options.update({'colour': funnel_colour})
+        pie_colour = data_attr.get('pie_colour') or '801C70'
+        pie_colour = self.add_colour_offset(pie_colour, multiple_index=multiple_index)
+        options.update({'colour': pie_colour})
 
     def edit_report_menu(self, request, chart_report_id, slug_str):
-        return [MenuItem(f'advanced_report_builder:funnel_chart_modal,pk-{chart_report_id}{slug_str}',
+        return [MenuItem(f'advanced_report_builder:pie_chart_modal,pk-{chart_report_id}{slug_str}',
                          menu_display='Edit',
                          font_awesome='fas fa-pencil-alt', css_classes=['btn-primary']),
                 *self.duplicate_menu(request=self.request, report_id=chart_report_id)]
 
     def get_date_field(self, index, fields, base_model, table):
         return None
 
 
-class FunnelChartModal(QueryBuilderModalBase):
+class PieChartModal(QueryBuilderModalBase):
     template_name = 'advanced_report_builder/charts/modal.html'
     process = PROCESS_EDIT_DELETE
     permission_delete = PERMISSION_OFF
-    model = FunnelChartReport
+    model = PieChartReport
     widgets = {'report_tags': Select2Multiple}
 
     form_fields = ['name',
                    'notes',
                    'report_type',
                    'report_tags',
                    'axis_value_type',
+                   'style',
                    'fields',
                    ]
 
     def form_setup(self, form, *_args, **_kwargs):
 
         self.add_query_data(form)
 
-        url = reverse('advanced_report_builder:funnel_chart_field_modal',
+        url = reverse('advanced_report_builder:pie_chart_field_modal',
                       kwargs={'slug': 'selector-99999-data-FIELD_INFO-report_type_id-REPORT_TYPE_ID'})
-
+        form.fields['notes'].widget.attrs['rows'] = 3
         return ('name',
                 'notes',
                 'report_type',
                 'report_tags',
                 'axis_value_type',
+                'style',
                 FieldEx('fields',
                         template='advanced_report_builder/select_column.html',
-                        extra_context={'select_column_url': url}),
+                        extra_context={'select_column_url': url,
+                                       'command_prefix': ''}),
                 FieldEx('query_data',
                         template='advanced_report_builder/query_builder.html'),
                 )
 
 
-class FunnelChartFieldForm(ChartBaseFieldForm):
+class PieChartFieldForm(ChartBaseFieldForm):
 
     def setup_modal(self, *args, **kwargs):
         data = json.loads(base64.b64decode(self.slug['data']))
         report_type, base_model = self.get_report_type_details()
 
         data_attr = split_attr(data)
 
         self.fields['title'] = CharField(initial=data['title'])
 
-        self.fields['funnel_colour'] = CharField(required=False, widget=ColourPickerWidget)
-        self.fields['funnel_colour'].initial = data_attr.get('funnel_colour')
+        self.fields['pie_colour'] = CharField(required=False, widget=ColourPickerWidget)
+        self.fields['pie_colour'].initial = data_attr.get('pie_colour')
 
         self.fields['has_filter'] = BooleanField(required=False, widget=RBToggle())
         self.fields['filter'] = CharField(required=False)
 
         if data_attr.get('has_filter') == '1':
             self.fields['has_filter'].initial = True
             if 'filter' in data_attr:
@@ -123,15 +124,15 @@
 
         super().setup_modal(*args, **kwargs)
 
     def get_additional_attributes(self):
         attributes = []
         self.get_report_type_details()
 
-        attributes.append(f'funnel_colour-{self.cleaned_data["funnel_colour"]}')
+        attributes.append(f'pie_colour-{self.cleaned_data["pie_colour"]}')
 
         if self.cleaned_data['has_filter']:
             attributes.append('has_filter-1')
 
             if self.cleaned_data['filter']:
                 b64_filter = encode_attribute(self.cleaned_data['filter'])
                 attributes.append(f'filter-{b64_filter}')
@@ -140,16 +141,16 @@
                 attributes.append(f'multiple_column_field-{self.cleaned_data["multiple_column_field"]}')
 
         if attributes:
             return '-'.join(attributes)
         return None
 
 
-class FunnelChartFieldModal(QueryBuilderModalBaseMixin, FormModal):
-    form_class = FunnelChartFieldForm
+class PieChartFieldModal(QueryBuilderModalBaseMixin, FormModal):
+    form_class = PieChartFieldForm
     size = 'xl'
     template_name = 'advanced_report_builder/charts/modal_field.html'
     no_header_x = True
     helper_class = HorizontalNoEnterHelper
 
     @property
     def modal_title(self):
@@ -176,15 +177,15 @@
             {'selector': '#filter_fields_div', 'values': {'checked': 'show'}, 'default': 'hide'}])
 
         form.add_trigger('multiple_columns', 'onchange', [
             {'selector': '#multiple_columns_fields_div', 'values': {'checked': 'show'}, 'default': 'hide'},
         ])
 
         return ['title',
-                'funnel_colour',
+                'pie_colour',
                 Div(FieldEx('has_filter',
                             template='django_modals/fields/label_checkbox.html',
                             field_class='col-6 input-group-sm'),
                     Div(
                         FieldEx('filter',
                                 template='advanced_report_builder/datatables/fields/single_query_builder.html'),
                         FieldEx('multiple_columns',
```

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/kanban.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/kanban.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/line_charts.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/line_charts.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,16 @@
                 'report_type',
                 'report_tags',
                 'axis_scale',
                 'axis_value_type',
                 'date_field',
                 FieldEx('fields',
                         template='advanced_report_builder/select_column.html',
-                        extra_context={'select_column_url': url}),
+                        extra_context={'select_column_url': url,
+                                       'command_prefix': ''}),
                 'x_label',
                 'y_label',
                 'show_totals',
                 'has_targets',
                 'targets',
                 FieldEx('query_data',
                         template='advanced_report_builder/query_builder.html'),
```

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/modals_base.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/modals_base.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/report_utils_mixin.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/report_utils_mixin.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/reports.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/reports.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/single_values.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/single_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         self.table.datatable_template = 'advanced_report_builder/single_values/middle.html'
         self.table.breakdown_url = self.get_breakdown_url()
         context['single_value_report'] = self.chart_report
         return context
 
     def get_breakdown_url(self):
         if self.table.single_value.show_breakdown:
-            return show_modal('advanced_report_builder:show_breakdown_modal',
+            return show_modal('advanced_report_builder:single_value_show_breakdown_modal',
                               'pk-',
                               self.table.single_value.id,
                               '-enable_links-',
                               self.table.enable_links, href=True)
         return None
 
     def pod_dashboard_view_menu(self):
@@ -365,15 +365,16 @@
                         template='advanced_report_builder/query_builder.html',
                         ),
                 'tile_colour',
                 'decimal_places',
                 'show_breakdown',
                 FieldEx('breakdown_fields',
                         template='advanced_report_builder/select_column.html',
-                        extra_context={'select_column_url': url}),
+                        extra_context={'select_column_url': url,
+                                       'command_prefix': ''}),
                 FieldEx('query_data',
                         template='advanced_report_builder/query_builder.html')
                 )
 
     def select2_field(self, **kwargs):
         return self.get_fields_for_select2(field_type='number',
                                            report_type=kwargs['report_type'],
@@ -408,15 +409,15 @@
         self._get_fields(base_model=base_model,
                          fields=fields,
                          tables=tables,
                          report_builder_class=report_builder_fields)
         return self.command_response('report_fields', data=json.dumps({'fields': fields, 'tables': tables}))
 
 
-class ShowBreakdownModal(TableUtilsMixin, Modal):
+class SingleValueShowBreakdownModal(TableUtilsMixin, Modal):
     button_container_class = 'text-center'
     size = 'xl'
 
     def modal_title(self):
         return self.table_report.name
 
     def add_table(self, base_model):
```

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/targets/utils.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/targets/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/advanced_report_builder/views/targets/views.py` & `django-advanced-report-builder-0.3.0/advanced_report_builder/views/targets/views.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/PKG-INFO` & `django-advanced-report-builder-0.3.0/django_advanced_report_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-report-builder
-Version: 0.2.1
+Version: 0.3.0
 Summary: Django app that allows you to build reports from modals
 Home-page: https://github.com/django-advance-utils/django-advanced-report-builder
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/SOURCES.txt` & `django-advanced-report-builder-0.3.0/django_advanced_report_builder.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 advanced_report_builder/migrations/0003_auto_20220215_1219.py
 advanced_report_builder/migrations/0004_customreport.py
 advanced_report_builder/migrations/0005_auto_20220303_0958.py
 advanced_report_builder/migrations/0006_auto_20220310_1147.py
 advanced_report_builder/migrations/0007_auto_20220322_1939.py
 advanced_report_builder/migrations/0008_auto_20220404_1144.py
 advanced_report_builder/migrations/0009_auto_20230428_1554.py
+advanced_report_builder/migrations/0010_auto_20230428_2033.py
 advanced_report_builder/migrations/__init__.py
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js
```

### Comparing `django-advanced-report-builder-0.2.1/setup.py` & `django-advanced-report-builder-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-advanced-report-builder",
-    version="0.2.1",
+    version="0.3.0",
     author="Thomas Turner",
     description="Django app that allows you to build reports from modals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/django-advanced-report-builder",
     include_package_data=True,
     packages=['advanced_report_builder'],
```

