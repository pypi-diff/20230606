# Comparing `tmp/seeq-spy-188.0.tar.gz` & `tmp/seeq-spy-188.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\seeq-spy-188.0.tar", last modified: Thu Jun  1 20:00:55 2023, max compression
+gzip compressed data, was "seeq-spy-188.2.tar", last modified: Tue Jun  6 19:49:37 2023, max compression
```

## Comparing `seeq-spy-188.0.tar` & `seeq-spy-188.2.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/
--rw-rw-rw-   0        0        0    33551 2023-03-17 02:53:52.000000 seeq-spy-188.0/LICENSE
--rw-rw-rw-   0        0        0      207 2023-03-17 02:53:52.000000 seeq-spy-188.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4541 2023-06-01 20:00:55.000000 seeq-spy-188.0/PKG-INFO
--rw-rw-rw-   0        0        0     4026 2023-03-17 02:53:52.000000 seeq-spy-188.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/base/
--rw-rw-rw-   0        0        0       36 2023-06-01 20:00:52.000000 seeq-spy-188.0/seeq/base/__init__.py
--rw-rw-rw-   0        0        0      875 2023-06-01 20:00:52.000000 seeq-spy-188.0/seeq/base/proputil.py
--rw-rw-rw-   0        0        0    31475 2023-06-01 20:00:52.000000 seeq-spy-188.0/seeq/base/seeq_names.py
--rw-rw-rw-   0        0        0    39742 2023-06-01 20:00:52.000000 seeq-spy-188.0/seeq/base/system.py
--rw-rw-rw-   0        0        0     4788 2023-06-01 20:00:52.000000 seeq-spy-188.0/seeq/base/util.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/scripts/
--rw-rw-rw-   0        0        0    12250 2023-06-01 20:00:52.000000 seeq-spy-188.0/seeq/scripts/create_monitoring_alerts.py
--rw-rw-rw-   0        0        0    49636 2023-06-01 20:00:52.000000 seeq-spy-188.0/seeq/scripts/create_monitoring_workbook.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/
--rw-rw-rw-   0        0        0     1953 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/__init__.py
--rw-rw-rw-   0        0        0    32016 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_common.py
--rw-rw-rw-   0        0        0     4687 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_config.py
--rw-rw-rw-   0        0        0     4424 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_datalab.py
--rw-rw-rw-   0        0        0     9686 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_errors.py
--rw-rw-rw-   0        0        0    48958 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_login.py
--rw-rw-rw-   0        0        0    92228 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_metadata.py
--rw-rw-rw-   0        0        0     5822 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_metadata_push_results.py
--rw-rw-rw-   0        0        0     2954 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_plot.py
--rw-rw-rw-   0        0        0    55589 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_pull.py
--rw-rw-rw-   0        0        0    68798 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_push.py
--rw-rw-rw-   0        0        0     5155 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_redaction.py
--rw-rw-rw-   0        0        0    44683 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_search.py
--rw-rw-rw-   0        0        0    20309 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_session.py
--rw-rw-rw-   0        0        0    15704 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_status.py
--rw-rw-rw-   0        0        0    20620 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_swap.py
--rw-rw-rw-   0        0        0     3471 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_upgrade.py
--rw-rw-rw-   0        0        0    10707 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/_url.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/acl/
--rw-rw-rw-   0        0        0      104 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/acl/__init__.py
--rw-rw-rw-   0        0        0    12126 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/acl/_pull.py
--rw-rw-rw-   0        0        0    11314 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/acl/_push.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/addons/
--rw-rw-rw-   0        0        0      188 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/addons/__init__.py
--rw-rw-rw-   0        0        0    26339 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/addons/_install.py
--rw-rw-rw-   0        0        0     2408 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/addons/_permissions.py
--rw-rw-rw-   0        0        0    12100 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/addons/_search.py
--rw-rw-rw-   0        0        0     5297 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/addons/_uninstall.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/assets/
--rw-rw-rw-   0        0        0      336 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/__init__.py
--rw-rw-rw-   0        0        0     3638 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_brochure.py
--rw-rw-rw-   0        0        0    12369 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_build.py
--rw-rw-rw-   0        0        0     3133 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_context.py
--rw-rw-rw-   0        0        0    48189 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_model.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/assets/_trees/
--rw-rw-rw-   0        0        0       69 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/__init__.py
--rw-rw-rw-   0        0        0     1375 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_constants.py
--rw-rw-rw-   0        0        0     7325 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_csv.py
--rw-rw-rw-   0        0        0    22068 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_match.py
--rw-rw-rw-   0        0        0     2629 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_pandas.py
--rw-rw-rw-   0        0        0     6458 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_path.py
--rw-rw-rw-   0        0        0    23200 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_properties.py
--rw-rw-rw-   0        0        0    13389 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_pull.py
--rw-rw-rw-   0        0        0    59025 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_tree.py
--rw-rw-rw-   0        0        0     5885 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_utils.py
--rw-rw-rw-   0        0        0    25528 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/_trees/_validate.py
--rw-rw-rw-   0        0        0     2538 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/assets/brochure.html
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/docs/
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Administration/
--rw-rw-rw-   0        0        0     6577 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Administration/User Migration.ipynb
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/
--rw-rw-rw-   0        0        0    17428 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
--rw-rw-rw-   0        0        0    33412 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
--rw-rw-rw-   0        0        0    16700 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
--rw-rw-rw-   0        0        0     8406 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
--rw-rw-rw-   0        0        0    38889 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
--rw-rw-rw-   0        0        0      870 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
--rw-rw-rw-   0        0        0   186560 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
--rw-rw-rw-   0        0        0   239024 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
--rw-rw-rw-   0        0        0   229026 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
--rw-rw-rw-   0        0        0    24627 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/
--rw-rw-rw-   0        0        0   135771 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
--rw-rw-rw-   0        0        0   152116 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
--rw-rw-rw-   0        0        0   207271 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
--rw-rw-rw-   0        0        0      325 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/Readme.txt
--rw-rw-rw-   0        0        0   141516 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
--rw-rw-rw-   0        0        0   439966 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
--rw-rw-rw-   0        0        0   189377 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
--rw-rw-rw-   0        0        0    15177 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Command Reference.ipynb
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/
--rw-rw-rw-   0        0        0    94677 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/Example Export.zip
--rw-rw-rw-   0        0        0   111771 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip
--rw-rw-rw-   0        0        0   113084 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip
--rw-rw-rw-   0        0        0  1083835 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv
--rw-rw-rw-   0        0        0      429 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/spy_tree_example.csv
--rw-rw-rw-   0        0        0   674467 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Tutorial.ipynb
--rw-rw-rw-   0        0        0    11595 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Version Considerations.ipynb
--rw-rw-rw-   0        0        0  1557151 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/Workbook Templates.ipynb
--rw-rw-rw-   0        0        0    54071 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.acl.ipynb
--rw-rw-rw-   0        0        0    11195 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.jobs.ipynb
--rw-rw-rw-   0        0        0    13015 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.login.ipynb
--rw-rw-rw-   0        0        0   128103 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.pull.ipynb
--rw-rw-rw-   0        0        0    99541 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.push.ipynb
--rw-rw-rw-   0        0        0    57289 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.search.ipynb
--rw-rw-rw-   0        0        0    95777 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.swap.ipynb
--rw-rw-rw-   0        0        0    10829 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.widgets.ipynb
--rw-rw-rw-   0        0        0    69828 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/Documentation/spy.workbooks.ipynb
--rw-rw-rw-   0        0        0       60 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/docs/_copy.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/jobs/
--rw-rw-rw-   0        0        0      491 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/jobs/__init__.py
--rw-rw-rw-   0        0        0     9869 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/jobs/_execute.py
--rw-rw-rw-   0        0        0     6111 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/jobs/_pull.py
--rw-rw-rw-   0        0        0     9363 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/jobs/_push.py
--rw-rw-rw-   0        0        0    25686 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/jobs/_schedule.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/notifications/
--rw-rw-rw-   0        0        0      153 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/notifications/__init__.py
--rw-rw-rw-   0        0        0    11927 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/notifications/_emails.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/utils/
--rw-rw-rw-   0        0        0     1569 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/widgets/
--rw-rw-rw-   0        0        0      200 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/widgets/__init__.py
--rw-rw-rw-   0        0        0     4158 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/widgets/_ipy_utils.py
--rw-rw-rw-   0        0        0    30480 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/widgets/_widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq/spy/workbooks/
--rw-rw-rw-   0        0        0     3012 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/__init__.py
--rw-rw-rw-   0        0        0    43729 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_annotation.py
--rw-rw-rw-   0        0        0    34087 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_content.py
--rw-rw-rw-   0        0        0    40974 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_data.py
--rw-rw-rw-   0        0        0     6639 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_folder.py
--rw-rw-rw-   0        0        0    14611 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_item.py
--rw-rw-rw-   0        0        0     5448 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_item_map.py
--rw-rw-rw-   0        0        0     3033 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_load.py
--rw-rw-rw-   0        0        0     3456 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_mustache.py
--rw-rw-rw-   0        0        0    14138 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_pull.py
--rw-rw-rw-   0        0        0    23051 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_push.py
--rw-rw-rw-   0        0        0     6316 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_render.py
--rw-rw-rw-   0        0        0    27127 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_report_content_utilities.py
--rw-rw-rw-   0        0        0     4729 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_save.py
--rw-rw-rw-   0        0        0    15508 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_search.py
--rw-rw-rw-   0        0        0    37445 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_template.py
--rw-rw-rw-   0        0        0    11995 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_user.py
--rw-rw-rw-   0        0        0    52462 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_workbook.py
--rw-rw-rw-   0        0        0    48819 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_worksheet.py
--rw-rw-rw-   0        0        0    51518 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/_workstep.py
--rw-rw-rw-   0        0        0   427362 2023-06-01 20:00:53.000000 seeq-spy-188.0/seeq/spy/workbooks/app.css
-drwxrwxrwx   0        0        0        0 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq_spy.egg-info/
--rw-rw-rw-   0        0        0     4541 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq_spy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4785 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq_spy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq_spy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-05 20:35:05.000000 seeq-spy-188.0/seeq_spy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      311 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq_spy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-01 20:00:55.000000 seeq-spy-188.0/seeq_spy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 20:00:55.000000 seeq-spy-188.0/setup.cfg
--rw-rw-rw-   0        0        0     1677 2023-06-01 19:56:18.000000 seeq-spy-188.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.775716 seeq-spy-188.2/
+-rw-rw-rw-   0        0        0    33551 2023-02-10 21:28:23.000000 seeq-spy-188.2/LICENSE
+-rw-rw-rw-   0        0        0      207 2023-02-10 21:28:23.000000 seeq-spy-188.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4606 2023-06-06 19:49:37.775716 seeq-spy-188.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4091 2023-04-18 17:55:42.000000 seeq-spy-188.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.449722 seeq-spy-188.2/seeq/
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.477723 seeq-spy-188.2/seeq/base/
+-rw-rw-rw-   0        0        0       36 2023-06-06 19:49:28.000000 seeq-spy-188.2/seeq/base/__init__.py
+-rw-rw-rw-   0        0        0      875 2023-06-06 19:49:28.000000 seeq-spy-188.2/seeq/base/proputil.py
+-rw-rw-rw-   0        0        0    32534 2023-06-06 19:49:28.000000 seeq-spy-188.2/seeq/base/seeq_names.py
+-rw-rw-rw-   0        0        0      157 2023-06-06 19:49:28.000000 seeq-spy-188.2/seeq/base/system.py
+-rw-rw-rw-   0        0        0     4788 2023-06-06 19:49:28.000000 seeq-spy-188.2/seeq/base/util.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.481722 seeq-spy-188.2/seeq/scripts/
+-rw-rw-rw-   0        0        0    12250 2023-06-06 19:49:28.000000 seeq-spy-188.2/seeq/scripts/create_monitoring_alerts.py
+-rw-rw-rw-   0        0        0    49636 2023-06-06 19:49:28.000000 seeq-spy-188.2/seeq/scripts/create_monitoring_workbook.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.530479 seeq-spy-188.2/seeq/spy/
+-rw-rw-rw-   0        0        0     1953 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/__init__.py
+-rw-rw-rw-   0        0        0    32016 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_common.py
+-rw-rw-rw-   0        0        0     4687 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_config.py
+-rw-rw-rw-   0        0        0     4424 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_datalab.py
+-rw-rw-rw-   0        0        0     9914 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_errors.py
+-rw-rw-rw-   0        0        0    49041 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_login.py
+-rw-rw-rw-   0        0        0    92226 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_metadata.py
+-rw-rw-rw-   0        0        0     5822 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_metadata_push_results.py
+-rw-rw-rw-   0        0        0     2954 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_plot.py
+-rw-rw-rw-   0        0        0    55640 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_pull.py
+-rw-rw-rw-   0        0        0    68835 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_push.py
+-rw-rw-rw-   0        0        0     5155 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_redaction.py
+-rw-rw-rw-   0        0        0    44741 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_search.py
+-rw-rw-rw-   0        0        0    20309 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_session.py
+-rw-rw-rw-   0        0        0    16507 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_status.py
+-rw-rw-rw-   0        0        0    20657 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_swap.py
+-rw-rw-rw-   0        0        0     3471 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_upgrade.py
+-rw-rw-rw-   0        0        0    10707 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_url.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.540480 seeq-spy-188.2/seeq/spy/acl/
+-rw-rw-rw-   0        0        0      104 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/acl/__init__.py
+-rw-rw-rw-   0        0        0    12172 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/acl/_pull.py
+-rw-rw-rw-   0        0        0    11351 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/acl/_push.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.558480 seeq-spy-188.2/seeq/spy/addons/
+-rw-rw-rw-   0        0        0      188 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/addons/__init__.py
+-rw-rw-rw-   0        0        0    26376 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/addons/_install.py
+-rw-rw-rw-   0        0        0     2408 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/addons/_permissions.py
+-rw-rw-rw-   0        0        0    12137 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/addons/_search.py
+-rw-rw-rw-   0        0        0     5334 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/addons/_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.572480 seeq-spy-188.2/seeq/spy/assets/
+-rw-rw-rw-   0        0        0      336 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/__init__.py
+-rw-rw-rw-   0        0        0     3638 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/assets/_brochure.py
+-rw-rw-rw-   0        0        0    12419 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/assets/_build.py
+-rw-rw-rw-   0        0        0     3133 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/assets/_context.py
+-rw-rw-rw-   0        0        0    48189 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/assets/_model.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.594478 seeq-spy-188.2/seeq/spy/assets/_trees/
+-rw-rw-rw-   0        0        0       69 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/__init__.py
+-rw-rw-rw-   0        0        0     1375 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_constants.py
+-rw-rw-rw-   0        0        0     7325 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_csv.py
+-rw-rw-rw-   0        0        0    22068 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_match.py
+-rw-rw-rw-   0        0        0     2629 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_pandas.py
+-rw-rw-rw-   0        0        0     6458 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_path.py
+-rw-rw-rw-   0        0        0    23208 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_properties.py
+-rw-rw-rw-   0        0        0    13381 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_pull.py
+-rw-rw-rw-   0        0        0    58791 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_tree.py
+-rw-rw-rw-   0        0        0     5897 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_utils.py
+-rw-rw-rw-   0        0        0    25525 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_validate.py
+-rw-rw-rw-   0        0        0     2538 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/assets/brochure.html
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.598480 seeq-spy-188.2/seeq/spy/docs/
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.637479 seeq-spy-188.2/seeq/spy/docs/Documentation/
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.639477 seeq-spy-188.2/seeq/spy/docs/Documentation/Administration/
+-rw-rw-rw-   0        0        0     6577 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Administration/User Migration.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.651479 seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/
+-rw-rw-rw-   0        0        0    17428 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
+-rw-rw-rw-   0        0        0    33412 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
+-rw-rw-rw-   0        0        0    16700 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
+-rw-rw-rw-   0        0        0     8406 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
+-rw-rw-rw-   0        0        0    38889 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
+-rw-rw-rw-   0        0        0      870 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
+-rw-rw-rw-   0        0        0   186560 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
+-rw-rw-rw-   0        0        0   239024 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
+-rw-rw-rw-   0        0        0   229026 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
+-rw-rw-rw-   0        0        0    24627 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.665478 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/
+-rw-rw-rw-   0        0        0   135771 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
+-rw-rw-rw-   0        0        0   152116 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
+-rw-rw-rw-   0        0        0   207271 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
+-rw-rw-rw-   0        0        0      325 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/Readme.txt
+-rw-rw-rw-   0        0        0   141516 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
+-rw-rw-rw-   0        0        0   439966 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
+-rw-rw-rw-   0        0        0   189377 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
+-rw-rw-rw-   0        0        0    15177 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Command Reference.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.679478 seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/
+-rw-rw-rw-   0        0        0    94677 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/Example Export.zip
+-rw-rw-rw-   0        0        0   111771 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip
+-rw-rw-rw-   0        0        0   113084 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip
+-rw-rw-rw-   0        0        0  1083835 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv
+-rw-rw-rw-   0        0        0      429 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/spy_tree_example.csv
+-rw-rw-rw-   0        0        0   674467 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Tutorial.ipynb
+-rw-rw-rw-   0        0        0    11595 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Version Considerations.ipynb
+-rw-rw-rw-   0        0        0  1557151 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Workbook Templates.ipynb
+-rw-rw-rw-   0        0        0    54071 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.acl.ipynb
+-rw-rw-rw-   0        0        0    11195 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.jobs.ipynb
+-rw-rw-rw-   0        0        0    13015 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.login.ipynb
+-rw-rw-rw-   0        0        0   128103 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.pull.ipynb
+-rw-rw-rw-   0        0        0    99541 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.push.ipynb
+-rw-rw-rw-   0        0        0    57289 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.search.ipynb
+-rw-rw-rw-   0        0        0    95777 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.swap.ipynb
+-rw-rw-rw-   0        0        0    10829 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.widgets.ipynb
+-rw-rw-rw-   0        0        0    69828 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.workbooks.ipynb
+-rw-rw-rw-   0        0        0       60 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/_copy.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.688481 seeq-spy-188.2/seeq/spy/jobs/
+-rw-rw-rw-   0        0        0      491 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/jobs/__init__.py
+-rw-rw-rw-   0        0        0     9869 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/jobs/_execute.py
+-rw-rw-rw-   0        0        0     6111 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/jobs/_pull.py
+-rw-rw-rw-   0        0        0     9398 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/jobs/_push.py
+-rw-rw-rw-   0        0        0    25737 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/jobs/_schedule.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.692479 seeq-spy-188.2/seeq/spy/notifications/
+-rw-rw-rw-   0        0        0      153 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/notifications/__init__.py
+-rw-rw-rw-   0        0        0    11927 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/notifications/_emails.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.694723 seeq-spy-188.2/seeq/spy/utils/
+-rw-rw-rw-   0        0        0     1569 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.701716 seeq-spy-188.2/seeq/spy/widgets/
+-rw-rw-rw-   0        0        0      200 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4158 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/widgets/_ipy_utils.py
+-rw-rw-rw-   0        0        0    30480 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/widgets/_widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.759717 seeq-spy-188.2/seeq/spy/workbooks/
+-rw-rw-rw-   0        0        0     3012 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/__init__.py
+-rw-rw-rw-   0        0        0    43729 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_annotation.py
+-rw-rw-rw-   0        0        0    34087 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_content.py
+-rw-rw-rw-   0        0        0    40974 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_data.py
+-rw-rw-rw-   0        0        0     6639 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_folder.py
+-rw-rw-rw-   0        0        0    14611 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_item.py
+-rw-rw-rw-   0        0        0     5448 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_item_map.py
+-rw-rw-rw-   0        0        0     3033 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_load.py
+-rw-rw-rw-   0        0        0     3456 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_mustache.py
+-rw-rw-rw-   0        0        0    14175 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_pull.py
+-rw-rw-rw-   0        0        0    23088 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_push.py
+-rw-rw-rw-   0        0        0     6316 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_render.py
+-rw-rw-rw-   0        0        0    27127 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_report_content_utilities.py
+-rw-rw-rw-   0        0        0     4729 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_save.py
+-rw-rw-rw-   0        0        0    15545 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_search.py
+-rw-rw-rw-   0        0        0    37445 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_template.py
+-rw-rw-rw-   0        0        0    11995 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_user.py
+-rw-rw-rw-   0        0        0    52462 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_workbook.py
+-rw-rw-rw-   0        0        0    48819 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_worksheet.py
+-rw-rw-rw-   0        0        0    51518 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_workstep.py
+-rw-rw-rw-   0        0        0   427362 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/workbooks/app.css
+drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.773716 seeq-spy-188.2/seeq_spy.egg-info/
+-rw-rw-rw-   0        0        0     4606 2023-06-06 19:49:37.000000 seeq-spy-188.2/seeq_spy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4785 2023-06-06 19:49:37.000000 seeq-spy-188.2/seeq_spy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 19:49:37.000000 seeq-spy-188.2/seeq_spy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-26 16:53:37.000000 seeq-spy-188.2/seeq_spy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      311 2023-06-06 19:49:37.000000 seeq-spy-188.2/seeq_spy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-06 19:49:37.000000 seeq-spy-188.2/seeq_spy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 19:49:37.776716 seeq-spy-188.2/setup.cfg
+-rw-rw-rw-   0        0        0     1677 2023-06-06 19:45:32.000000 seeq-spy-188.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `seeq-spy-188.0/LICENSE` & `seeq-spy-188.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/PKG-INFO` & `seeq-spy-188.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 188.0
+Version: 188.2
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -31,14 +31,16 @@
 - Import data in a programmatic way (when Seeq Workbench's *CSV Import* capability won't cut it)
 - Calculate new data in Python and push it into Seeq
 - Create an asset model
 - Programmatically create and manipulate Workbench Analyses or Organizer Topics
 
 **Use of the SPy module requires Python 3.7 or later.**
 
+**SPy version 187 and higher is compatible with Pandas 2.x.**
+
 To start exploring the SPy module, execute the following lines of code in Jupyter:
 
 ```
 from seeq import spy
 spy.docs.copy()
 ```
```

### Comparing `seeq-spy-188.0/README.md` & `seeq-spy-188.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 - Import data in a programmatic way (when Seeq Workbench's *CSV Import* capability won't cut it)
 - Calculate new data in Python and push it into Seeq
 - Create an asset model
 - Programmatically create and manipulate Workbench Analyses or Organizer Topics
 
 **Use of the SPy module requires Python 3.7 or later.**
 
+**SPy version 187 and higher is compatible with Pandas 2.x.**
+
 To start exploring the SPy module, execute the following lines of code in Jupyter:
 
 ```
 from seeq import spy
 spy.docs.copy()
 ```
```

### Comparing `seeq-spy-188.0/seeq/base/proputil.py` & `seeq-spy-188.2/seeq/base/proputil.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/base/seeq_names.py` & `seeq-spy-188.2/seeq/base/seeq_names.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,24 @@
 class SeeqNames:
     class Database:
         class Schemas:
             materialized_tables = 'materialized_tables'
         
     
     class MaterializedTables:
-        datum_id_column = 'datum_id'
-        item_id_column = 'item_id'
+        datum_id_column = 'datum id'
+        item_id_column = 'item id'
+        context_table_prefix = 'context_'
+        class Rules:
+            ancestor = 'ancestor'
+            concat_columns = 'concatColumns'
+            event_property = 'eventProperty'
+            item_property = 'itemProperty'
+            path = 'path'
+        
     
     class Injection:
         everyone_user_group = 'EveryoneUserGroup'
         system_state = 'SystemState'
         system_user = 'SystemUser'
     
     class Connectors:
@@ -218,19 +226,23 @@
         system = 'System'
         import_ = 'Import'
         monitors = 'Monitors'
         projects = 'Projects'
         content = 'Content'
         report_templates = 'ReportTemplates'
         condition_monitors = 'ConditionMonitors'
+        item_finders = 'ItemFinders'
         plugins = 'Plugins'
         displays = 'Displays'
         display_templates = 'DisplayTemplates'
         notification_configurations = 'NotificationConfigurations'
+        label = 'Label'
+        context = 'Context'
         table_definitions = 'TableDefinitions'
+        graph_q_l = 'GraphQL'
     
     class Channels:
         agents_status = 'agents-status'
         datasources_status = 'datasources-status'
         broadcast = 'broadcast'
         live_screenshot = 'live-screenshot'
         async_response = 'async-response'
@@ -245,14 +257,15 @@
         agents = '/agents'
         audit = '/audit'
         auth = '/auth'
         assets = '/assets'
         folders = '/folders'
         networks = '/networks'
         items = '/items'
+        item_finders = '/finders'
         reports = '/reports'
         jobs = '/jobs'
         logs = '/logs'
         batch = '/batch'
         trees = '/trees'
         asset_trees = '/trees/assets'
         signals = '/signals'
@@ -298,15 +311,21 @@
         date_ranges = '/date-ranges'
         asset_selections = '/asset-selections'
         plugins = '/plugins'
         displays = '/displays'
         display_templates = '/display-templates'
         usage = '/usage'
         notification_configurations = '/notification-configurations'
+        labels = '/labels'
+        context = '/context'
+        context_comments = '/comments'
+        context_labels = '/labels'
+        context_opaque = '/opaque'
         table_definitions = '/table-definitions'
+        graph_q_l = '/graphql'
         class ErrorMessages:
             attempted_to_set_scope_on_a_globally_scoped_item = 'Attempted to set scope on a globally scoped item'
         
         class AddOnToolLinkType:
             window = 'window'
             tab = 'tab'
             none = 'none'
@@ -364,14 +383,19 @@
                 cache_capsules_read = 'Cache Capsules Read'
                 cache_in_memory_samples_read = 'Cache In-Memory Samples Read'
                 cache_in_memory_capsules_read = 'Cache In-Memory Capsules Read'
                 database_items_read = 'Database Items Read'
                 database_relationships_read = 'Database Relationships Read'
             
         
+        class Flags:
+            all_properties = '@allProperties'
+            exclude_globally_scoped = '@excludeGloballyScoped'
+            include_unsearchable = '@includeUnsearchable'
+        
     
     class UnitTest:
         timestamp1 = '1990-03-07T09:58:20.888888Z'
         timestamp2 = '1990-04-08T10:59:21.999999Z'
         non_existent_guid = '1CB64296-FC3E-4221-9A7F-947A0AB99807'
     
     class Edges:
@@ -414,14 +438,15 @@
         source_worksheet = 'source worksheet'
         source_workstep = 'source workstep'
         has_asset = 'has asset'
         has_asset_selection = 'has asset selection'
         has_asset_selections = 'has asset selections'
         has_condition = 'has condition'
         monitors = 'monitors'
+        has_item_finder = 'has item finder'
         has_content = 'has content'
         has_date_range = 'has date range'
         has_date_ranges = 'has date ranges'
         has_scheduled_notebook = 'has scheduled notebook'
         has_template = 'has template'
         subscribed_to = 'subscribed to'
     
@@ -444,14 +469,15 @@
         project_link = 'ProjectLink'
         add_on_tool = 'AddOnTool'
         base_annotation = 'BaseAnnotation'
         report = 'Report'
         report_template = 'ReportTemplate'
         journal = 'Journal'
         reply = 'Reply'
+        item_finder = 'ItemFinder'
         condition = 'Condition'
         condition_monitor = 'ConditionMonitor'
         capsule = 'Capsule'
         stored_condition = 'StoredCondition'
         calculated_condition = 'CalculatedCondition'
         scalar = 'ScalarItem'
         literal_scalar = 'LiteralScalar'
@@ -538,14 +564,15 @@
         archived_reason = 'Archived Reason'
         sync_token = 'Sync Token'
         number_format = 'Number Format'
         source_number_format = 'Source Number Format'
         string_format = 'String Format'
         source_string_format = 'Source String Format'
         storage_location = 'Storage Location'
+        executor_id = 'Executor ID'
         creator_id = 'Creator ID'
         creator_first_name = 'Creator First Name'
         creator_last_name = 'Creator Last Name'
         historical_data_version = 'Historical Data Version'
         manual_cdc = 'Manual CDC'
         scoped_to = 'Scoped To'
         asset = 'asset'
@@ -597,15 +624,15 @@
         previous_index_at = 'Previous Index At'
         sync_result = 'Sync Result'
         indexing_schedule_supported = 'Indexing Schedule Supported'
         asset_tree_search_index_needs_updating = 'Asset Tree Search Index Needs Updating'
         sync_mode = 'Sync Mode'
         items_archived_count = 'Items Archived Count'
         indexing_duration = 'Indexing Duration'
-        current_indexing_started_at = 'Current Indexing Started At'
+        indexing_progress_timestamp = 'Indexing Progress Timestamp'
         asset_progress = 'Asset Progress'
         asset_count = 'Asset Count'
         previous_asset_count = 'Previous Asset Count'
         signal_progress = 'Signal Progress'
         signal_count = 'Signal Count'
         previous_signal_count = 'Previous Signal Count'
         condition_progress = 'Condition Progress'
@@ -726,14 +753,16 @@
         summary_value = 'Summary Value'
         current_filename = 'Current Filename'
         last_result_hash = 'Last Result Hash'
         asset_path_depth = 'Asset Path Depth'
         last_run_at = 'Last Run At'
         last_run_state = 'Last Run State'
         query_range_look_ahead = 'Query Range Look Ahead'
+        finder_configurations = 'Finder Configurations'
+        last_run_warnings = 'Last Run Warnings'
         resource_size = 'Resource Size'
         project_type = 'Project Type'
         cron_schedule = 'Cron Schedule'
         background = 'Background'
         condition_formula_now = 'Condition Formula Now'
         notebook_path = 'Notebook Path'
         previous_run_time = 'Previous Run Time'
```

### Comparing `seeq-spy-188.0/seeq/base/util.py` & `seeq-spy-188.2/seeq/base/util.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/scripts/create_monitoring_alerts.py` & `seeq-spy-188.2/seeq/scripts/create_monitoring_alerts.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/scripts/create_monitoring_workbook.py` & `seeq-spy-188.2/seeq/scripts/create_monitoring_workbook.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/__init__.py` & `seeq-spy-188.2/seeq/spy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,8 @@
 """
 
 __all__ = ['acl', 'addons', 'assets', 'docs', 'workbooks', 'widgets', 'login', 'logout', 'plot', 'pull', 'push',
            'search', 'swap', 'PATH_ROOT', 'DEFAULT_WORKBOOK_PATH', 'GLOBALS_ONLY', 'GLOBALS_AND_ALL_WORKBOOKS',
            'INHERIT_FROM_WORKBOOK', 'Session', 'Status', 'options', 'session', 'client', 'user', 'server_version',
            'jobs', 'notifications', 'upgrade', 'utils', 'errors']
 
-__version__ = '%d.%d' % (int('188'), int('0'))
+__version__ = '%d.%d' % (int('188'), int('2'))
```

### Comparing `seeq-spy-188.0/seeq/spy/_common.py` & `seeq-spy-188.2/seeq/spy/_common.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/_config.py` & `seeq-spy-188.2/seeq/spy/_config.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/_datalab.py` & `seeq-spy-188.2/seeq/spy/_datalab.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/_errors.py` & `seeq-spy-188.2/seeq/spy/_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,29 +8,36 @@
 import ipywidgets as widgets
 from IPython.core.getipython import get_ipython
 from IPython.display import display
 
 from seeq.sdk.rest import ApiException
 from seeq.spy import _datalab
 
-__all__ = ['SPyDependencyNotFound', 'SPyException', 'SPyRuntimeError', 'SPyValueError', 'SPyTypeError',
-           'SchedulePostingError', 'ApiException', 'get_api_exception_message']
+__all__ = ['SPyDependencyNotFound', 'SPyException', 'SPyKeyboardInterrupt', 'SPyRuntimeError', 'SPyValueError',
+           'SPyTypeError', 'SchedulePostingError', 'ApiException', 'get_api_exception_message']
 
 
 class SPyDependencyNotFound(Exception):
     pass
 
 
 class SPyException(Exception):
     """
     Base exception class of all errors internally handled and raised by SPy
     """
     pass
 
 
+class SPyKeyboardInterrupt(SPyException, KeyboardInterrupt):
+    """
+    Raised when the kernel is interrupted, e.g. by pressing Ctrl+C or by clicking Stop in a Jupyter Notebook
+    """
+    pass
+
+
 class SPyRuntimeError(SPyException, RuntimeError):
     """
     Raised when an error is detected by SPy that does not fall in any of the other categories
     """
     pass
```

### Comparing `seeq-spy-188.0/seeq/spy/_login.py` & `seeq-spy-188.2/seeq/spy/_login.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from seeq.spy._errors import *
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 
 AUTOMATIC_PROXY_DETECTION = '__auto__'
 
 
+@Status.handle_keyboard_interrupt()
 def login(username=None, password=None, *, access_key=None, url=None, directory='Seeq',
           ignore_ssl_errors=False, proxy=AUTOMATIC_PROXY_DETECTION, credentials_file=None, force=True,
           quiet=None, status=None, session: Session = None, private_url=None, auth_token=None, csrf_token=None,
           request_origin_label=None, request_origin_url=None):
     """
     Establishes a connection with Seeq Server and logs in with a set of
     credentials. At least one set of credentials must be provided.
@@ -424,14 +425,15 @@
         if is_datalab_functions_project() and not request_origin_label.startswith("[Data Lab Functions]"):
             request_origin_label = f"[Data Lab Functions] {request_origin_label}"
         _client.set_default_header('x-sq-origin-label', request_origin_label)
     if request_origin_url is not None:
         _client.set_default_header('x-sq-origin-url', request_origin_url)
 
 
+@Status.handle_keyboard_interrupt()
 def logout(quiet=None, status=None, session: Session = None):
     """
     Logs you out of your current session.
 
     Parameters
     ----------
 
@@ -999,17 +1001,18 @@
 
     if input_datetime.tz is None:
         input_datetime = input_datetime.tz_localize(timezone)
 
     return input_datetime
 
 
-def validate_start_and_end(session: Session,
-                           start: Union[pd.Timestamp, datetime.date, str, int, float],
-                           end: Union[pd.Timestamp, datetime.date, str, int, float]):
+def validate_start_and_end(
+        session: Session,
+        start: Union[pd.Timestamp, datetime.date, str, int, float],
+        end: Union[pd.Timestamp, datetime.date, str, int, float]) -> Tuple[pd.Timestamp, pd.Timestamp]:
     """
     Takes a pair of start and end times, either of which could be None, and uses some default logic
     to produce a "cleaned up" start and end. For example, if start is after end, then end is reset to
     one hour after start.
     :param session: The login session (necessary to fulfill this call).
     :param start: The start value, or None if you want a default to be calculated.
     :param end: The end value, or None if you want a default to be calculated.
```

### Comparing `seeq-spy-188.0/seeq/spy/_metadata.py` & `seeq-spy-188.2/seeq/spy/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     # We need the index to be regular (unique, integer, ascending) so that we can add Asset entries to the bottom.
     # This is tested by _metadata.test_metadata_dataframe_weird_index()
     original_index_name = metadata_df.index.name
     metadata_df.index.set_names([ORIGINAL_INDEX_COLUMN], inplace=True)
     metadata_df.reset_index(inplace=True)
 
     if 'Type' not in metadata_df.columns:
-        metadata_df['Type'] = pd.Series(np.nan, dtype='object')
+        metadata_df['Type'] = pd.Series(np.nan, dtype=object)
 
     push_results = PushResults(metadata_df)
 
     previous_results = None
     if state_file is not None and os.path.exists(state_file):
         # noinspection PyBroadException
         try:
```

### Comparing `seeq-spy-188.0/seeq/spy/_metadata_push_results.py` & `seeq-spy-188.2/seeq/spy/_metadata_push_results.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/_plot.py` & `seeq-spy-188.2/seeq/spy/_plot.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/_pull.py` & `seeq-spy-188.2/seeq/spy/_pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 
 ENUM_REGEX = r'ENUM{{(\d+)\|(.+?)}}'
 ENUM_PATTERN = re.compile(ENUM_REGEX)
 
 
+@Status.handle_keyboard_interrupt()
 def pull(items, *, start=None, end=None, grid='15min', header='__auto__', group_by=None, shape='auto',
          capsule_properties=None, tz_convert=None, calculation=None, bounding_values=False,
          invalid_values_as=np.nan, enums_as='string', errors=None, quiet=None, status: Status = None,
          session: Optional[Session] = None, capsules_as=None):
     """
     Retrieves signal, condition or scalar data from Seeq Server and returns it
     in a DataFrame.
@@ -745,15 +746,15 @@
                                    (columns[item_name].index <= pd_capsule_end)] = 1
 
             for prop in capsule['properties']:  # type: dict
                 # We need to create a column name that is unique for the item / property combination
                 colname = '%s - %s' % (item_name, prop['name'])
                 if colname not in columns:
                     # Here we start with a NaN-filled series, since we're populating property values (not 1s and 0s).
-                    columns[colname] = pd.Series(np.nan, index_to_use)
+                    columns[colname] = pd.Series(np.nan, index_to_use, dtype=object)
 
                 # Note here that overlapping capsules with different properties will result in "last one wins"
                 columns[colname].loc[(columns[colname].index >= pd_capsule_start) &
                                      (columns[colname].index <= pd_capsule_end)] = prop['value']
 
         column_names[item_id] = list()
         for col, series in columns.items():
```

### Comparing `seeq-spy-188.0/seeq/spy/_push.py` & `seeq-spy-188.2/seeq/spy/_push.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from seeq.spy._status import Status
 from seeq.spy.workbooks import _folder, _workbook
 
 # This constant is set to be slightly below numArchivedItemsPerCommit in DatasourceQueriesV1.java
 DATASOURCE_CLEANUP_ITEM_COUNT_THRESHOLD = 19_000
 
 
+@Status.handle_keyboard_interrupt()
 def push(data=None, *, metadata=None, replace=None, workbook=_common.DEFAULT_WORKBOOK_PATH,
          worksheet=_common.DEFAULT_WORKSHEET_NAME, datasource=None, archive=False, type_mismatches='raise',
          metadata_state_file: Optional[str] = None, include_workbook_inventory: Optional[bool] = None,
          errors=None, quiet=None, status=None, session: Optional[Session] = None):
     """
     Imports metadata and/or data into Seeq Server, possibly scoped to a
     workbook and/or datasource.
```

### Comparing `seeq-spy-188.0/seeq/spy/_redaction.py` & `seeq-spy-188.2/seeq/spy/_redaction.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/_search.py` & `seeq-spy-188.2/seeq/spy/_search.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
+import datetime
 import types
-from typing import List, Dict, Union, Mapping, Optional
+from dataclasses import dataclass
+from typing import List, Dict, Union, Mapping, Optional, Set
 
 import pandas as pd
 
 from seeq import spy
 from seeq.sdk import *
 from seeq.spy import _common, _login, _metadata, _push, _swap
 from seeq.spy._errors import *
@@ -13,17 +15,70 @@
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 
 RESERVED_SEARCH_COLUMN_NAMES = ['Path', 'Asset', 'Type', 'Depth', 'Estimated Sample Period', 'Formula Parameters',
                                 'Datasource Name']
 
 
+@dataclass
+class SearchContext:
+    session: Session
+    status: Status
+
+    all_properties: bool
+    workbook: str
+    recursive: bool
+    ignore_unindexed_properties: bool
+    include_archived: bool
+    estimate_sample_period: dict
+    include_swap_info: bool
+    old_asset_format: bool
+    order_by: Optional[Union[str, list]]
+
+    status_index: int
+    columns: List[str]
+    metadata: List
+    ids: Set
+    comparison: str
+    dupe_count: int
+    sample_periods: Dict
+    workbook_id: str
+    pd_start: Optional[pd.Timestamp]
+    pd_end: Optional[pd.Timestamp]
+    use_search_items_api: bool
+    timer: datetime.datetime
+
+    items_api: ItemsApi
+    trees_api: TreesApi
+    formulas_api: FormulasApi
+    displays_api: DisplaysApi
+    display_templates_api: DisplayTemplatesApi
+
+    def __init__(self, session: Session, status: Status):
+        self.session = session
+        self.status = status
+
+        self.columns = list()
+        self.metadata = list()
+        self.ids = set()
+        self.datasource_ids = dict()
+        self.dupe_count = 0
+        self.sample_periods = dict()
+
+        self.items_api = ItemsApi(session.client)
+        self.trees_api = TreesApi(session.client)
+        self.formulas_api = FormulasApi(session.client)
+        self.displays_api = DisplaysApi(session.client)
+        self.display_templates_api = DisplayTemplatesApi(session.client)
+
+
+@Status.handle_keyboard_interrupt()
 def search(query, *, all_properties=False, workbook=_common.DEFAULT_WORKBOOK_PATH, recursive=True,
            ignore_unindexed_properties=True, include_archived=False, include_swappable_assets=False,
-           estimate_sample_period=None, old_asset_format=None, order_by=None, quiet=None, errors=None, status=None,
+           estimate_sample_period=None, old_asset_format=None, order_by=None, errors=None, quiet=None, status=None,
            session: Optional[Session] = None):
     """
     Issues a query to the Seeq Server to retrieve metadata for signals,
     conditions, scalars and assets. This metadata can then be used to retrieve
     samples, capsules for a particular time range via spy.pull().
 
     Parameters
@@ -232,657 +287,658 @@
         (session, 'session', Session)
     ])
 
     status = Status.validate(status, quiet, errors)
     session = Session.validate(session)
     _login.validate_login(session, status)
 
-    try:
-        return _search(session, query, all_properties=all_properties, workbook=workbook, recursive=recursive,
-                       ignore_unindexed_properties=ignore_unindexed_properties, include_archived=include_archived,
-                       estimate_sample_period=estimate_sample_period, include_swap_info=include_swappable_assets,
-                       old_asset_format=old_asset_format, order_by=order_by, status=status, input_args=input_args)
-
-    except KeyboardInterrupt:
-        status.update('Search canceled', Status.CANCELED)
-
-
-def _search(session: Session, query, *, all_properties, workbook, recursive, ignore_unindexed_properties,
-            include_archived, estimate_sample_period, include_swap_info, old_asset_format, order_by, status,
-            input_args):
-    if order_by:
-        order_by = _validate_order_by(order_by)
+    context = SearchContext(session, status)
+    context.all_properties = all_properties
+    context.workbook = workbook
+    context.recursive = recursive
+    context.ignore_unindexed_properties = ignore_unindexed_properties
+    context.include_archived = include_archived
+    context.estimate_sample_period = estimate_sample_period
+    context.include_swap_info = include_swappable_assets
+    context.old_asset_format = old_asset_format
+    context.order_by = order_by
+
+    if context.order_by:
+        context.order_by = _validate_order_by(context.order_by)
 
-    if estimate_sample_period is not None:
-        if estimate_sample_period.keys() != {'Start', 'End'}:  # strict comparison, allowing only these two keys
+    if context.estimate_sample_period is not None:
+        if context.estimate_sample_period.keys() != {'Start', 'End'}:  # strict comparison, allowing only these two keys
             raise SPyValueError(f"estimate_sample_period must have 'Start' and 'End' keys but got "
-                                f"{estimate_sample_period.keys()}")
-        pd_start, pd_end = _login.validate_start_and_end(session,
-                                                         estimate_sample_period['Start'],
-                                                         estimate_sample_period['End'])
+                                f"{context.estimate_sample_period.keys()}")
+        context.pd_start, context.pd_end = _login.validate_start_and_end(context.session,
+                                                                         context.estimate_sample_period['Start'],
+                                                                         context.estimate_sample_period['End'])
 
-    if not recursive and 'Path' not in query:
+    if not context.recursive and 'Path' not in query:
         raise SPyValueError("'Path' must be included in query when recursive=False")
 
-    old_asset_format__resolved = old_asset_format
-    if old_asset_format__resolved is None:
+    context.old_asset_format = old_asset_format
+    if context.old_asset_format is None:
         # In the future, we may wish to change this default to False, in which case we should use
         # spy.options.compatibility and keep it True for users expecting older behavior.
-        old_asset_format__resolved = True
-
-    items_api = ItemsApi(session.client)
-    trees_api = TreesApi(session.client)
-    formulas_api = FormulasApi(session.client)
-    displays_api = DisplaysApi(session.client)
-    display_templates_api = DisplayTemplatesApi(session.client)
+        context.old_asset_format = True
 
     queries: List[Union[Dict, Mapping]]
     if isinstance(query, pd.DataFrame):
         queries = query.to_dict(orient='records')
-        comparison = '=='
+        context.comparison = '=='
     elif isinstance(query, pd.Series):
         queries = [query.to_dict()]
-        comparison = '=='
+        context.comparison = '=='
     elif isinstance(query, list):
         queries = query
-        comparison = '~='
+        context.comparison = '~='
     elif isinstance(query, str):
-        worksheet = spy.utils.get_analysis_worksheet_from_url(query, include_archived, quiet=status.quiet)
+        worksheet = spy.utils.get_analysis_worksheet_from_url(query, context.include_archived,
+                                                              quiet=context.status.quiet)
         queries = worksheet.display_items.to_dict(orient='records')
-        comparison = '=='
+        context.comparison = '=='
     else:
         queries = [query]
-        comparison = '~='
-
-    #
-    # This function makes use of a lot of inner function definitions that utilize variables from the outer scope.
-    # In order to keep things straight, all variables confined to the inner scope are prefixed with an underscore.
-    #
-
-    metadata = list()
-    columns = list()
-    ids = set()
-    dupe_count = 0
-    sample_periods = dict()
-
-    status.df = pd.DataFrame(queries)
-    status.df['Time'] = 0
-    status.df['Count'] = 0
-    status.df['Pages'] = 0
-    status.df['Result'] = 'Queued'
-    status.update('Initializing', Status.RUNNING)
-
-    def _add_to_dict(_dict, _key, _val):
-        if _key in ['Archived', 'Cache Enabled', 'Enabled', 'Unsearchable'] and isinstance(_val, str):
-            _val = _val.lower() == 'true'
-        _dict[_key] = _common.none_to_nan(_val)
-
-        # We want the columns to appear in a certain order (the order we added them in) for readability
-        if _key not in columns:
-            columns.append(_key)
-
-    def _add_ancestors_to_prop_dict_from_item_output(_item_output, _prop_dict):
-        _ancestors = [a.name for a in _item_output.ancestors]
-        _add_ancestors_to_prop_dict(_item_output.type, _item_output.name, _ancestors, _prop_dict)
-
-    def _add_ancestors_to_prop_dict(_type, _name, _ancestors, _prop_dict):
-        _common.add_ancestors_to_definition(_type, _name, _ancestors, _prop_dict, old_asset_format__resolved)
-        for _key in ['Path', 'Asset']:
-            if _key in _prop_dict and _key not in columns:
-                columns.append(_key)
-
-    def _add_to_metadata(_prop_dict):
-        if _prop_dict['ID'] not in ids:
-            metadata.append(_prop_dict)
-            ids.add(_prop_dict['ID'])
-        else:
-            nonlocal dupe_count
-            dupe_count += 1
+        context.comparison = '~='
 
-    def _estimate_sample_period(_signal_id, _signal_name):
-        sampling_formula = f"$signal.estimateSamplePeriod(capsule('{pd_start.isoformat()}','{pd_end.isoformat()}'))"
-
-        formula_run_output = safely(
-            lambda: formulas_api.run_formula(formula=sampling_formula, parameters=[f"signal={_signal_id}"]),
-            action_description='estimate sample period',
-            status=status,
-            additional_errors=[400])
-
-        if formula_run_output is not None and formula_run_output.scalar.value is not None:
-            sample_periods[_signal_id] = pd.to_timedelta(
-                formula_run_output.scalar.value, unit=formula_run_output.scalar.uom)
+    context.status.df = pd.DataFrame(queries)
+    context.status.df['Time'] = 0
+    context.status.df['Count'] = 0
+    context.status.df['Pages'] = 0
+    context.status.df['Result'] = 'Queued'
+    context.status.update('Initializing', Status.RUNNING)
+
+    context.workbook_id = None
+    if context.workbook:
+        if _common.is_guid(context.workbook):
+            context.workbook_id = _common.sanitize_guid(context.workbook)
         else:
-            status.warn(
-                f'Could not determine the sample period for signal "{_signal_name}" {_signal_id} within the '
-                f'time period {pd_start.isoformat()} to {pd_end.isoformat()}. There might not be enough data '
-                f'in the specified time range. Modify the time period with the `estimate_start` '
-                f'and `estimate_end` arguments.'
-            )
-            sample_periods[_signal_id] = pd.NaT
-
-    def _add_all_properties(_id, _prop_dict):
-
-        def _add_error_message_and_warn(msg):
-            _add_to_dict(_prop_dict, 'Pull Result', msg)
-            status.warn(msg)
-
-        @request_safely(action_description=f'get all item properties for {_id}',
-                        status=status,
-                        on_error=_add_error_message_and_warn)
-        def _request_item_properties():
-            _item = items_api.get_item_and_all_properties(id=_id)  # type: ItemOutputV1
-            # Name and Type don't appear in additional properties
-            _add_to_dict(_prop_dict, 'Name', _item.name)
-            _add_to_dict(_prop_dict, 'Type', _item.type)
-            _add_to_dict(_prop_dict, 'Scoped To', _common.none_to_nan(_item.scoped_to))
-            for _prop in _item.properties:  # type: PropertyOutputV1
-                if _prop.name not in RESERVED_SEARCH_COLUMN_NAMES:
-                    _add_to_dict(_prop_dict, _prop.name, _prop.value)
-
-            if _item.type in ['CalculatedSignal', 'CalculatedCondition', 'CalculatedScalar', 'LiteralScalar']:
-                _formula_output = formulas_api.get_item(id=_id)  # type: FormulaItemOutputV1
-                _add_to_dict(_prop_dict, 'Formula Parameters', [
-                    '%s=%s' % (_p.name, _p.item.id if _p.item else _p.formula) for _p in _formula_output.parameters
-                ])
-
-            elif _item.type == 'ThresholdMetric':
-                _formula_parameters = _metadata.formula_parameters_dict_from_threshold_metric(session, _id)
-                for _key, _value in _formula_parameters.items():
-                    _add_to_dict(_prop_dict, _key, _value)
-
-            elif _item.type == 'Display':
-                _display_output = displays_api.get_display(id=_id)
-                _add_to_dict(_prop_dict, 'Template ID', _display_output.template.id)
-                if _display_output.swap is not None:
-                    _add_to_dict(_prop_dict, 'Swap Out Asset ID', _display_output.swap.swap_out)
-                    _add_to_dict(_prop_dict, 'Swap In Asset ID', _display_output.swap.swap_in)
-                else:
-                    _add_to_dict(_prop_dict, 'Swap Out Asset ID', _display_output.template.swap_source_asset_id)
+            search_query, _ = _push.create_analysis_search_query(context.workbook)
+            search_df = spy.workbooks.search(search_query,
+                                             status=context.status.create_inner('Find Workbook', quiet=True),
+                                             session=context.session)
+            context.workbook_id = search_df.iloc[0]['ID'] if len(search_df) > 0 else None
+            if context.workbook == _common.DEFAULT_WORKBOOK_PATH and context.workbook_id is None:
+                context.workbook_id = _common.GLOBALS_ONLY
 
-            elif _item.type == 'DisplayTemplate':
-                _display_template_output = display_templates_api.get_display_template(id=_id)
-                _add_to_dict(_prop_dict, 'Source Workstep ID', _display_template_output.source_workstep_id)
-
-        _request_item_properties()
-        return _prop_dict
-
-    def _add_tree(_id, _prop_dict):
-        _item_output = None
-        if include_swap_info:
-            _item_dependency_output = safely(lambda: items_api.get_formula_dependencies(id=_id),
-                                             action_description=f'get dependencies for {_id}',
-                                             status=status)  # type: ItemDependencyOutputV1
-            if _item_dependency_output is not None:
-                _item_output = _item_dependency_output
-
-            _dependencies_with_relevant_assets = _swap.get_swappable_assets(_item_dependency_output)
-
-            def _swappable_asset_dict(d):
-                _leaf_asset = d.ancestors[-1]
-                return {
-                    'ID': _leaf_asset.id,
-                    'Type': _leaf_asset.type,
-                    'Path': _common.path_list_to_string([a.name for a in d.ancestors[0:-1]]),
-                    'Asset': _leaf_asset.name
-                }
+    context.use_search_items_api = False
 
-            _swappable_assets = pd.DataFrame([_swappable_asset_dict(d) for d in _dependencies_with_relevant_assets],
-                                             columns=['ID', 'Type', 'Path', 'Asset'])
+    for status_index in range(len(queries)):
+        context.status_index = status_index
+        _process_query(context, queries[status_index])
 
-            _add_to_dict(_prop_dict, 'Swappable Assets', _swappable_assets)
-        else:
-            _asset_tree_output = safely(lambda: trees_api.get_tree(id=_id),
-                                        action_description=f'get asset tree ancestors for {_id}',
-                                        status=status)  # type: AssetTreeOutputV1
-            if _asset_tree_output is not None:
-                _item_output = _asset_tree_output.item
-        if _item_output is not None:
-            _add_ancestors_to_prop_dict_from_item_output(_item_output, _prop_dict)
-        return _prop_dict
-
-    workbook_id = None
-    if workbook:
-        if _common.is_guid(workbook):
-            workbook_id = _common.sanitize_guid(workbook)
+    if context.dupe_count > 0:
+        if context.use_search_items_api:
+            arg_to_use = context.order_by if context.order_by else []
+            if 'ID' in arg_to_use:
+                context.status.warn(
+                    f'{context.dupe_count} duplicates removed from returned DataFrame. If you used a list of '
+                    f'searches, those searches may have had overlap.')
+            else:
+                arg_to_use.append('ID')
+                context.status.warn(
+                    f'{context.dupe_count} duplicates removed from returned DataFrame. Use order_by={arg_to_use} in '
+                    f'your spy.search to ensure results are not missing any items.')
         else:
-            search_query, _ = _push.create_analysis_search_query(workbook)
-            search_df = spy.workbooks.search(search_query, status=status.create_inner('Find Workbook', quiet=True),
-                                             session=session)
-            workbook_id = search_df.iloc[0]['ID'] if len(search_df) > 0 else None
-            if workbook == _common.DEFAULT_WORKBOOK_PATH and workbook_id is None:
-                workbook_id = _common.GLOBALS_ONLY
-
-    datasource_ids = dict()
-    use_search_items_api = False
-
-    for status_index in range(len(queries)):
-        timer = _common.timer_start()
+            context.status.warn(f'{context.dupe_count} duplicates removed from returned DataFrame.')
 
-        current_query = queries[status_index]
+    context.status.update('Query successful', Status.SUCCESS)
 
-        if _common.present(current_query, 'ID'):
-            # If ID is specified, short-circuit everything and just get the item directly.
-            _prop_dict = dict()
-            current_id = current_query['ID']
-            _add_all_properties(current_id, _prop_dict)
-
-            # Since this method bypasses the search_items() route that would normally supply the asset ancestors, we
-            # specifically call _add_tree() to make the trees_api call that will fetch the ancestors.
-            _add_tree(current_id, _prop_dict)
-
-            # Still need to determine sample period for signals and have NaT for non-signal items
-            if estimate_sample_period is not None:
-                if 'Signal' in current_query['Type']:
-                    _estimate_sample_period(current_id, _prop_dict['Name'])
-                else:
-                    sample_periods[current_query['ID']] = pd.NaT
+    if len(context.columns) == 0:
+        context.columns = ['ID', 'Type']
+    output_df = pd.DataFrame(data=context.metadata, columns=context.columns)
+    if context.order_by and not output_df.empty:
+        output_df.sort_values(context.order_by, ignore_index=True, inplace=True)
 
-                _add_to_dict(_prop_dict, 'Estimated Sample Period', sample_periods[current_query['ID']])
+    if old_asset_format is None:
+        type_column = output_df['Type']
+        if len(type_column.loc[type_column == 'Asset']) > 0:
+            context.status.warn(
+                'This search result includes Assets. Consider passing in "old_asset_format=False" so that the '
+                '"Path" and "Asset" columns are populated in a way that is consistent with all other aspects '
+                'of SPy. The default behavior without this argument emulates the (incorrect) way SPy would '
+                'return such results historically.')
+            context.status.display()
 
-            _add_to_metadata(_prop_dict)
+    output_df_properties = types.SimpleNamespace(
+        func='spy.search',
+        kwargs=input_args,
+        old_asset_format=context.old_asset_format,
+        status=context.status)
 
-            status.df.at[status_index, 'Time'] = _common.timer_elapsed(timer)
-            status.df.at[status_index, 'Count'] = 1
-            status.df.at[status_index, 'Result'] = 'Success'
-            continue
+    _common.put_properties_on_df(output_df, output_df_properties)
 
-        # If the user wants a recursive search or there's no 'Path' in the query, then use the ItemsApi.search_items API
-        use_search_items_api = recursive or not _common.present(current_query, 'Path')
+    return output_df
 
-        if not use_search_items_api and include_archived:
-            # As you can see in the code below, the TreesApi.get_tree() API doesn't have the ability to request
-            # archived items
-            raise SPyValueError('include_archived=True can only be used with recursive searches or searches that do '
-                                'not involve a Path parameter')
-
-        allowed_properties = ['Type', 'Name', 'Description', 'Path', 'Asset', 'Datasource Class', 'Datasource ID',
-                              'Datasource Name', 'Data ID', 'Cache Enabled', 'Scoped To']
-
-        disallowed_properties = list()
-        for key, value in current_query.items():
-            if key not in allowed_properties:
-                disallowed_properties.append(key)
-
-        for key in disallowed_properties:
-            del current_query[key]
-
-        allowed_properties_str = '", "'.join(allowed_properties)
-        if len(disallowed_properties) > 0:
-            disallowed_properties_str = '", "'.join(disallowed_properties)
-            message = f'The following properties are not indexed' \
-                      f'{" and will be ignored" if ignore_unindexed_properties else ""}:\n' \
-                      f'"{disallowed_properties_str}"\n' \
-                      f'Use any of the following searchable properties and then filter further using DataFrame ' \
-                      f'operations:\n"{allowed_properties_str}"'
 
-            if not ignore_unindexed_properties:
-                raise SPyValueError(message)
-            else:
-                status.warn(message)
+def _process_query(context: SearchContext, current_query):
+    context.timer = _common.timer_start()
 
-        if len(current_query) == 0:
-            raise SPyValueError('No recognized properties present in "query" argument. You must provide a dict or a '
-                                'DataFrame with keys or columns with at least one of the following properties: \n' +
-                                allowed_properties_str)
-
-        item_types = list()
-        clauses: Dict = dict()
-
-        if _common.present(current_query, 'Type'):
-            item_type_specs = list()
-            if isinstance(current_query['Type'], list):
-                item_type_specs.extend(current_query['Type'])
+    if _common.present(current_query, 'ID'):
+        # If ID is specified, short-circuit everything and just get the item directly.
+        prop_dict = dict()
+        current_id = current_query['ID']
+        _add_all_properties(context, current_id, prop_dict)
+
+        # Since this method bypasses the search_items() route that would normally supply the asset ancestors, we
+        # specifically call _add_tree() to make the trees_api call that will fetch the ancestors.
+        _add_tree(context, current_id, prop_dict)
+
+        # Still need to determine sample period for signals and have NaT for non-signal items
+        if context.estimate_sample_period is not None:
+            if 'Signal' in current_query['Type']:
+                _estimate_sample_period(context, current_id, prop_dict['Name'])
             else:
-                item_type_specs.append(current_query['Type'])
-
-            valid_types = ['StoredSignal', 'CalculatedSignal',
-                           'StoredCondition', 'CalculatedCondition',
-                           'LiteralScalar', 'CalculatedScalar',
-                           'Datasource',
-                           'ThresholdMetric', 'Chart', 'Asset',
-                           'Workbook', 'Worksheet',
-                           'Display', 'DisplayTemplate']
-
-            for item_type_spec in item_type_specs:
-                if item_type_spec == 'Signal':
-                    item_types.extend(['StoredSignal', 'CalculatedSignal'])
-                elif item_type_spec == 'Condition':
-                    item_types.extend(['StoredCondition', 'CalculatedCondition'])
-                elif item_type_spec == 'Scalar':
-                    item_types.extend(['LiteralScalar', 'CalculatedScalar'])
-                elif item_type_spec == 'Datasource':
-                    item_types.extend(['Datasource'])
-                elif item_type_spec == 'Metric':
-                    item_types.extend(['ThresholdMetric'])
-                elif item_type_spec not in valid_types:
-                    raise SPyValueError(f'Type field value not recognized: {item_type_spec}\n'
-                                        f'Valid types: {", ".join(valid_types)}')
-                else:
-                    item_types.append(item_type_spec)
-
-            del current_query['Type']
+                context.sample_periods[current_query['ID']] = pd.NaT
 
-        for prop_name in ['Name', 'Description', 'Datasource Class', 'Datasource ID', 'Data ID']:
-            if prop_name in current_query and not pd.isna(current_query[prop_name]):
-                clauses[prop_name] = (comparison, current_query[prop_name])
-
-        if _common.present(current_query, 'Datasource Name'):
-            datasource_name = _common.get(current_query, 'Datasource Name')
-            if datasource_name in datasource_ids:
-                clauses['Datasource ID'], clauses['Datasource Class'] = datasource_ids[datasource_name]
-            else:
-                _filters = ['Name == %s' % datasource_name]
-                if _common.present(current_query, 'Datasource ID'):
-                    _filters.append('Datasource ID == %s' % _common.get(current_query, 'Datasource ID'))
-                if _common.present(current_query, 'Datasource Class'):
-                    _filters.append('Datasource Class == %s' % _common.get(current_query, 'Datasource Class'))
-
-                _filter_list = [' && '.join(_filters)]
-                if include_archived:
-                    _filter_list.append('@includeUnsearchable')
-
-                datasource_results = items_api.search_items(filters=_filter_list,
-                                                            types=['Datasource'],
-                                                            limit=100000)  # type: ItemSearchPreviewPaginatedListV1
-
-                if len(datasource_results.items) > 1:
-                    raise SPyRuntimeError('Multiple datasources found that match "%s"' % datasource_name)
-                elif len(datasource_results.items) == 0:
-                    raise SPyRuntimeError('No datasource found that matches "%s"' % datasource_name)
-
-                datasource = datasource_results.items[0]  # type: ItemSearchPreviewV1
-
-                @request_safely(action_description=f'get datasource details for "{datasource_name}" {datasource.id}',
-                                status=status)
-                def request_datasource_and_set_clause():
-                    property_output = items_api.get_property(id=datasource.id, property_name='Datasource Class')
-                    clauses['Datasource Class'] = ('==', property_output.value)
-                    property_output = items_api.get_property(id=datasource.id, property_name='Datasource ID')
-                    clauses['Datasource ID'] = ('==', property_output.value)
-                    datasource_ids[datasource_name] = (clauses['Datasource ID'], clauses['Datasource Class'])
-
-                request_datasource_and_set_clause()
-
-            del current_query['Datasource Name']
-
-        filters = list()
-        if len(clauses.items()) > 0:
-            filters.append(' && '.join([p + c + v for p, (c, v) in clauses.items()]))
-
-        if include_archived:
-            filters.append('@includeUnsearchable')
-
-        kwargs = {
-            'filters': filters,
-            'types': item_types,
-            'limit': session.options.search_page_size
-        }
-
-        if workbook:
-            if workbook_id:
-                kwargs['scope'] = workbook_id
-            elif workbook != _common.DEFAULT_WORKBOOK_PATH:
-                raise SPyRuntimeError('Workbook "%s" not found, or is not accessible by you' % workbook)
-
-        if _common.present(current_query, 'Scoped To'):
-            kwargs['scope'] = current_query['Scoped To']
-            kwargs['filters'].append('@excludeGloballyScoped')
+            _add_to_dict(
+                context, prop_dict, 'Estimated Sample Period', context.sample_periods[current_query['ID']])
 
-        if _common.present(current_query, 'Asset'):
-            if _common.is_guid(_common.get(current_query, 'Asset')):
-                kwargs['asset'] = _common.get(current_query, 'Asset')
-            elif not _common.present(current_query, 'Path'):
-                raise SPyValueError('"Path" query parameter must be present when "Asset" name parameter present')
-
-        path_to_query = None
-        if _common.present(current_query, 'Path'):
-            path_to_query = current_query['Path']
-            if _common.present(current_query, 'Asset'):
-                path_to_query = path_to_query + ' >> ' + current_query['Asset']
-
-        def _do_search(_offset):
-            kwargs['offset'] = _offset
-            if 'scope' in kwargs and isinstance(kwargs['scope'], str):
-                kwargs['scope'] = [kwargs['scope']]
-            if use_search_items_api:
-                if order_by:
-                    kwargs['order_by'] = order_by
-                return items_api.search_items(**kwargs)
-
-            _kwargs2 = {
-                'offset': kwargs['offset'],
-                'limit': kwargs['limit'],
-                'scope': _common.get(kwargs, 'scope'),
-                'exclude_globally_scoped': ('@excludeGloballyScoped' in kwargs['filters'])
-            }
-            if 'asset' in kwargs:
-                _kwargs2['id'] = kwargs['asset']
-                tree_output = trees_api.get_tree(**_kwargs2)
-            else:
-                tree_output = trees_api.get_tree_root_nodes(**_kwargs2)
-            if len(kwargs['types']) > 0:
-                tree_output.children = [x for x in tree_output.children if x.type in kwargs['types']]
-            return tree_output
-
-        def _iterate_over_output(_output_func, _collection_name, _action_func):
-            _offset = 0
-            while True:
-                _output = _output_func(_offset)
-
-                _collection = getattr(_output, _collection_name)
-                # Determine sample period for all signals and have NaT for non-signal items
-                if estimate_sample_period is not None:
-                    for _item in _collection:
-                        if 'Signal' in _item.type:
-                            _estimate_sample_period(_item.id, _item.name)
-                        else:
-                            sample_periods[_item.id] = pd.NaT
-
-                status.df.at[status_index, 'Time'] = _common.timer_elapsed(timer)
-                status.df.at[status_index, 'Count'] = _offset + len(_collection)
-                status.df.at[status_index, 'Pages'] += 1
-                status.df.at[status_index, 'Result'] = 'Querying'
-                status.update('Querying Seeq Server for items', Status.RUNNING)
-
-                for _item in _collection:
-                    _action_func(_item)
-
-                if len(_collection) != _output.limit:
-                    break
-
-                _offset += _output.limit
-
-        def _gather_results(_actual_path_list=None):
-            def _gather_results_via_item_search(_result):
-                _item_search_preview = _result  # type: ItemSearchPreviewV1
-                __prop_dict = dict()
-
-                _add_to_dict(__prop_dict, 'ID', _item_search_preview.id)
-                _add_ancestors_to_prop_dict_from_item_output(_item_search_preview, __prop_dict)
-
-                _add_to_dict(__prop_dict, 'Name', _item_search_preview.name)
-                _add_to_dict(__prop_dict, 'Description', _item_search_preview.description)
-                _add_to_dict(__prop_dict, 'Type', _item_search_preview.type)
-                _uom = _item_search_preview.value_unit_of_measure if _item_search_preview.value_unit_of_measure \
-                    else _item_search_preview.source_value_unit_of_measure
-                _add_to_dict(__prop_dict, 'Value Unit Of Measure', _uom)
-                _datasource_item_preview = _item_search_preview.datasource  # type: ItemPreviewV1
-                _add_to_dict(__prop_dict, 'Datasource Name',
-                             _datasource_item_preview.name if _datasource_item_preview else None)
-                _add_to_dict(__prop_dict, 'Archived', _item_search_preview.is_archived)
-                if all_properties:
-                    _add_all_properties(_item_search_preview.id, __prop_dict)
-                if include_swap_info:
-                    _add_tree(_item_search_preview.id, __prop_dict)
-                if estimate_sample_period is not None:
-                    _add_to_dict(__prop_dict, 'Estimated Sample Period', sample_periods[_item_search_preview.id])
-                _add_to_metadata(__prop_dict)
-
-            def _gather_results_via_get_tree(_result):
-                _tree_item_output = _result  # type: TreeItemOutputV1
-                __prop_dict = dict()
-
-                for _prop, _attr in [('Name', 'name'), ('Description', 'description')]:
-                    if _prop not in current_query:
-                        continue
-
-                    if not _common.does_query_fragment_match(current_query[_prop],
-                                                             getattr(_tree_item_output, _attr),
-                                                             contains=(comparison == '~=')):
-                        return
-
-                _add_to_dict(__prop_dict, 'ID', _tree_item_output.id)
-                _add_ancestors_to_prop_dict(
-                    _tree_item_output.type, _tree_item_output.name, _actual_path_list, __prop_dict)
-
-                _add_to_dict(__prop_dict, 'Name', _tree_item_output.name)
-                _add_to_dict(__prop_dict, 'Description', _tree_item_output.description)
-                _add_to_dict(__prop_dict, 'Type', _tree_item_output.type)
-                _add_to_dict(__prop_dict, 'Value Unit Of Measure', _tree_item_output.value_unit_of_measure)
-                _add_to_dict(__prop_dict, 'Archived', _tree_item_output.is_archived)
-
-                if all_properties:
-                    _add_all_properties(_tree_item_output.id, __prop_dict)
-                if include_swap_info:
-                    _add_tree(_tree_item_output.id, __prop_dict)
-                if estimate_sample_period is not None:
-                    _add_to_dict(__prop_dict, 'Estimated Sample Period', sample_periods[_tree_item_output.id])
-                _add_to_metadata(__prop_dict)
+        _add_to_metadata(context, prop_dict)
 
-            if use_search_items_api:
-                _iterate_over_output(_do_search, 'items', _gather_results_via_item_search)
-            else:
-                _iterate_over_output(_do_search, 'children', _gather_results_via_get_tree)
+        context.status.df.at[context.status_index, 'Time'] = _common.timer_elapsed(context.timer)
+        context.status.df.at[context.status_index, 'Count'] = 1
+        context.status.df.at[context.status_index, 'Result'] = 'Success'
+        return
+
+    # If the user wants a recursive search or there's no 'Path' in the query, then use the ItemsApi.search_items API
+    context.use_search_items_api = context.recursive or not _common.present(current_query, 'Path')
+
+    if not context.use_search_items_api and context.include_archived:
+        # As you can see in the code below, the TreesApi.get_tree() API doesn't have the ability to request
+        # archived items
+        raise SPyValueError('include_archived=True can only be used with recursive searches or searches that do '
+                            'not involve a Path parameter')
+
+    allowed_properties = ['Type', 'Name', 'Description', 'Path', 'Asset', 'Datasource Class', 'Datasource ID',
+                          'Datasource Name', 'Data ID', 'Cache Enabled', 'Scoped To']
+
+    disallowed_properties = list()
+    for key, value in current_query.items():
+        if key not in allowed_properties:
+            disallowed_properties.append(key)
+
+    for key in disallowed_properties:
+        del current_query[key]
+
+    allowed_properties_str = '", "'.join(allowed_properties)
+    if len(disallowed_properties) > 0:
+        disallowed_properties_str = '", "'.join(disallowed_properties)
+        message = f'The following properties are not indexed' \
+                  f'{" and will be ignored" if context.ignore_unindexed_properties else ""}:\n' \
+                  f'"{disallowed_properties_str}"\n' \
+                  f'Use any of the following searchable properties and then filter further using DataFrame ' \
+                  f'operations:\n"{allowed_properties_str}"'
 
-        if not _common.present(current_query, 'Path'):
-            # If there's no 'Path' property in the query, we can immediately proceed to the results gathering stage.
-            _gather_results()
+        if not context.ignore_unindexed_properties:
+            raise SPyValueError(message)
         else:
-            # If there is a 'Path' property in the query, then first we have to drill down through the tree to the
-            # appropriate depth so we can find the asset ID to use for the results gathering stage.
-
-            # We define a function here so we can use recursion through the path.
-            def _process_query_path_string(_remaining_query_path_string, _actual_path_list, _asset_id=None):
-                _query_path_list = _common.path_string_to_list(_remaining_query_path_string)
-
-                _query_path_part = _query_path_list[0]
-
-                _tree_kwargs = dict()
-                _tree_kwargs['limit'] = kwargs['limit']
-                _tree_kwargs['offset'] = 0
-
-                if 'scope' in kwargs and isinstance(kwargs['scope'], str):
-                    _tree_kwargs['scope'] = [kwargs['scope']]
-
-                while True:
-                    if not _asset_id:
-                        _tree_output = trees_api.get_tree_root_nodes(**_tree_kwargs)  # type: AssetTreeOutputV1
-                    else:
-                        _tree_kwargs['id'] = _asset_id
-                        _tree_output = trees_api.get_tree(**_tree_kwargs)  # type: AssetTreeOutputV1
-
-                    for _child in _tree_output.children:  # type: TreeItemOutputV1
-                        if not _asset_id:
-                            @request_safely(action_description=f'check if "{_child.name}" {_child.id} has '
-                                                               f'datasource matching request',
-                                            status=status,
-                                            default_value=True)
-                            def _is_item_in_filter_datasources():
-                                _child_item_output = items_api.get_item_and_all_properties(
-                                    id=_child.id)  # type: ItemOutputV1
-                                for _prop in ['Datasource Class', 'Datasource ID']:
-                                    if _prop in clauses:
-                                        _, _val = clauses[_prop]
-                                        _p_list = [_p.value for _p in _child_item_output.properties if
-                                                   _p.name == _prop]
-                                        if len(_p_list) == 0 or _p_list[0] != _val:
-                                            return False
-                                return True
-
-                            # We only filter out datasource at the top level, in case the tree is mixed
-                            if not _is_item_in_filter_datasources():
-                                continue
-
-                        if _common.does_query_fragment_match(_query_path_part, _child.name, contains=False):
-                            _actual_path_list_for_child = _actual_path_list.copy()
-                            _actual_path_list_for_child.append(_child.name)
-                            if len(_query_path_list) == 1:
-                                kwargs['asset'] = _child.id
-                                _gather_results(_actual_path_list_for_child)
-                            else:
-                                _process_query_path_string(_common.path_list_to_string(_query_path_list[1:]),
-                                                           _actual_path_list_for_child,
-                                                           _child.id)
+            context.status.warn(message)
 
-                    if len(_tree_output.children) < _tree_kwargs['limit']:
-                        break
-
-                    _tree_kwargs['offset'] += _tree_kwargs['limit']
+    if len(current_query) == 0:
+        raise SPyValueError('No recognized properties present in "query" argument. You must provide a dict or a '
+                            'DataFrame with keys or columns with at least one of the following properties: \n' +
+                            allowed_properties_str)
+
+    item_types = list()
+    clauses: Dict = dict()
+
+    if _common.present(current_query, 'Type'):
+        item_type_specs = list()
+        if isinstance(current_query['Type'], list):
+            item_type_specs.extend(current_query['Type'])
+        else:
+            item_type_specs.append(current_query['Type'])
 
-            if len(path_to_query) == 0:
-                _gather_results(list())
+        valid_types = ['StoredSignal', 'CalculatedSignal',
+                       'StoredCondition', 'CalculatedCondition',
+                       'LiteralScalar', 'CalculatedScalar',
+                       'Datasource',
+                       'ThresholdMetric', 'Chart', 'Asset',
+                       'Workbook', 'Worksheet',
+                       'Display', 'DisplayTemplate']
+
+        for item_type_spec in item_type_specs:
+            if item_type_spec == 'Signal':
+                item_types.extend(['StoredSignal', 'CalculatedSignal'])
+            elif item_type_spec == 'Condition':
+                item_types.extend(['StoredCondition', 'CalculatedCondition'])
+            elif item_type_spec == 'Scalar':
+                item_types.extend(['LiteralScalar', 'CalculatedScalar'])
+            elif item_type_spec == 'Datasource':
+                item_types.extend(['Datasource'])
+            elif item_type_spec == 'Metric':
+                item_types.extend(['ThresholdMetric'])
+            elif item_type_spec not in valid_types:
+                raise SPyValueError(f'Type field value not recognized: {item_type_spec}\n'
+                                    f'Valid types: {", ".join(valid_types)}')
             else:
-                _process_query_path_string(path_to_query, list())
+                item_types.append(item_type_spec)
 
-        status.df.at[status_index, 'Result'] = 'Success'
+        del current_query['Type']
 
-    if dupe_count > 0:
-        if use_search_items_api:
-            arg_to_use = order_by if order_by else []
-            if 'ID' in arg_to_use:
-                status.warn(f'{dupe_count} duplicates removed from returned DataFrame. If you used a list of '
-                            f'searches, those searches may have had overlap.')
-            else:
-                arg_to_use.append('ID')
-                status.warn(
-                    f'{dupe_count} duplicates removed from returned DataFrame. Use order_by={arg_to_use} in your '
-                    f'spy.search to ensure results are not missing any items.')
+    for prop_name in ['Name', 'Description', 'Datasource Class', 'Datasource ID', 'Data ID']:
+        if prop_name in current_query and not pd.isna(current_query[prop_name]):
+            clauses[prop_name] = (context.comparison, current_query[prop_name])
+
+    if _common.present(current_query, 'Datasource Name'):
+        datasource_name = _common.get(current_query, 'Datasource Name')
+        if datasource_name in context.datasource_ids:
+            clauses['Datasource ID'], clauses['Datasource Class'] = context.datasource_ids[datasource_name]
         else:
-            status.warn(f'{dupe_count} duplicates removed from returned DataFrame.')
-
-    status.update('Query successful', Status.SUCCESS)
-
-    if len(columns) == 0:
-        columns = ['ID', 'Type']
-    output_df = pd.DataFrame(data=metadata, columns=columns)
-    if order_by and not output_df.empty:
-        output_df.sort_values(order_by, ignore_index=True, inplace=True)
-
-    if old_asset_format is None:
-        type_column = output_df['Type']
-        if len(type_column.loc[type_column == 'Asset']) > 0:
-            status.warn('This search result includes Assets. Consider passing in "old_asset_format=False" so that the '
-                        '"Path" and "Asset" columns are populated in a way that is consistent with all other aspects '
-                        'of SPy. The default behavior without this argument emulates the (incorrect) way SPy would '
-                        'return such results historically.')
-            status.display()
+            filters = ['Name == %s' % datasource_name]
+            if _common.present(current_query, 'Datasource ID'):
+                filters.append('Datasource ID == %s' % _common.get(current_query, 'Datasource ID'))
+            if _common.present(current_query, 'Datasource Class'):
+                filters.append('Datasource Class == %s' % _common.get(current_query, 'Datasource Class'))
+
+            filter_list = [' && '.join(filters)]
+            if context.include_archived:
+                filter_list.append('@includeUnsearchable')
+
+            datasource_results = context.items_api.search_items(
+                filters=filter_list, types=['Datasource'], limit=100000)  # type: ItemSearchPreviewPaginatedListV1
+
+            if len(datasource_results.items) > 1:
+                raise SPyRuntimeError('Multiple datasources found that match "%s"' % datasource_name)
+            elif len(datasource_results.items) == 0:
+                raise SPyRuntimeError('No datasource found that matches "%s"' % datasource_name)
+
+            datasource = datasource_results.items[0]  # type: ItemSearchPreviewV1
+
+            @request_safely(action_description=f'get datasource details for "{datasource_name}" {datasource.id}',
+                            status=context.status)
+            def request_datasource_and_set_clause():
+                property_output = context.items_api.get_property(id=datasource.id, property_name='Datasource Class')
+                clauses['Datasource Class'] = ('==', property_output.value)
+                property_output = context.items_api.get_property(id=datasource.id, property_name='Datasource ID')
+                clauses['Datasource ID'] = ('==', property_output.value)
+                context.datasource_ids[datasource_name] = (clauses['Datasource ID'], clauses['Datasource Class'])
+
+            request_datasource_and_set_clause()
+
+        del current_query['Datasource Name']
+
+    filters = list()
+    if len(clauses.items()) > 0:
+        filters.append(' && '.join([p + c + v for p, (c, v) in clauses.items()]))
+
+    if context.include_archived:
+        filters.append('@includeUnsearchable')
+
+    kwargs = {
+        'filters': filters,
+        'types': item_types,
+        'limit': context.session.options.search_page_size
+    }
+
+    if context.workbook:
+        if context.workbook_id:
+            kwargs['scope'] = context.workbook_id
+        elif context.workbook != _common.DEFAULT_WORKBOOK_PATH:
+            raise SPyRuntimeError(f'Workbook "{context.workbook}" not found, or is not accessible by you')
+
+    if _common.present(current_query, 'Scoped To'):
+        kwargs['scope'] = current_query['Scoped To']
+        kwargs['filters'].append('@excludeGloballyScoped')
+
+    if _common.present(current_query, 'Asset'):
+        if _common.is_guid(_common.get(current_query, 'Asset')):
+            kwargs['asset'] = _common.get(current_query, 'Asset')
+        elif not _common.present(current_query, 'Path'):
+            raise SPyValueError('"Path" query parameter must be present when "Asset" name parameter present')
+
+    path_to_query = None
+    if _common.present(current_query, 'Path'):
+        path_to_query = current_query['Path']
+        if _common.present(current_query, 'Asset'):
+            path_to_query = path_to_query + ' >> ' + current_query['Asset']
 
-    output_df_properties = types.SimpleNamespace(
-        func='spy.search',
-        kwargs=input_args,
-        old_asset_format=old_asset_format__resolved,
-        status=status)
+    if not _common.present(current_query, 'Path'):
+        # If there's no 'Path' property in the query, we can immediately proceed to the results gathering stage.
+        _gather_results(context, current_query, kwargs)
+    else:
+        # If there is a 'Path' property in the query, then first we have to drill down through the tree to the
+        # appropriate depth so we can find the asset ID to use for the results gathering stage.
 
-    _common.put_properties_on_df(output_df, output_df_properties)
+        if len(path_to_query) == 0:
+            _gather_results(context, current_query, kwargs, list())
+        else:
+            _process_query_path_string(context, current_query, kwargs, path_to_query, list(), clauses)
 
-    return output_df
+    context.status.df.at[context.status_index, 'Result'] = 'Success'
 
 
 def _validate_order_by(order_by):
     """
     Validate and process order_by arg of spy.search
     :param order_by: {str, list}
     :return: list
     """
     # convert string order_by to a list
     if isinstance(order_by, str):
         order_by = [order_by]
 
     # validate order_by
-    _order_fields = ['ID', 'Name', 'Description']
-    invalid_fields = [x for x in order_by if x not in _order_fields]
+    order_fields = ['ID', 'Name', 'Description']
+    invalid_fields = [x for x in order_by if x not in order_fields]
     if len(invalid_fields) > 0:
         raise SPyValueError(
             f"Invalid order_by fields: {invalid_fields}. Search results can only be ordered on "
-            f"{_order_fields} fields.")
+            f"{order_fields} fields.")
 
     return order_by
+
+
+def _add_to_dict(context: SearchContext, _dict, key, val):
+    if key in ['Archived', 'Cache Enabled', 'Enabled', 'Unsearchable'] and isinstance(val, str):
+        val = val.lower() == 'true'
+    _dict[key] = _common.none_to_nan(val)
+
+    # We want the columns to appear in a certain order (the order we added them in) for readability
+    if key not in context.columns:
+        context.columns.append(key)
+
+
+def _add_ancestors_to_prop_dict_from_item_output(context: SearchContext, item_output, prop_dict):
+    _ancestors = [a.name for a in item_output.ancestors]
+    _add_ancestors_to_prop_dict(context, item_output.type, item_output.name, _ancestors, prop_dict)
+
+
+def _add_ancestors_to_prop_dict(context: SearchContext, _type, name, ancestors, prop_dict):
+    _common.add_ancestors_to_definition(_type, name, ancestors, prop_dict, context.old_asset_format)
+    for key in ['Path', 'Asset']:
+        if key in prop_dict and key not in context.columns:
+            context.columns.append(key)
+
+
+def _add_to_metadata(context: SearchContext, prop_dict):
+    if prop_dict['ID'] not in context.ids:
+        context.metadata.append(prop_dict)
+        context.ids.add(prop_dict['ID'])
+    else:
+        context.dupe_count += 1
+
+
+def _estimate_sample_period(context: SearchContext, signal_id, signal_name):
+    sampling_formula = "$signal.estimateSamplePeriod(" \
+                       f"capsule('{context.pd_start.isoformat()}','{context.pd_end.isoformat()}'))"
+
+    formula_run_output = safely(
+        lambda: context.formulas_api.run_formula(formula=sampling_formula, parameters=[f"signal={signal_id}"]),
+        action_description='estimate sample period',
+        status=context.status,
+        additional_errors=[400])
+
+    if formula_run_output is not None and formula_run_output.scalar.value is not None:
+        context.sample_periods[signal_id] = pd.to_timedelta(
+            formula_run_output.scalar.value, unit=formula_run_output.scalar.uom)
+    else:
+        context.status.warn(
+            f'Could not determine the sample period for signal "{signal_name}" {signal_id} within the '
+            f'time period {context.pd_start.isoformat()} to {context.pd_end.isoformat()}. '
+            f'There might not be enough data in the specified time range. Modify the time period with the '
+            f'`estimate_start` and `estimate_end` arguments.'
+        )
+        context.sample_periods[signal_id] = pd.NaT
+
+
+def _add_all_properties(context: SearchContext, _id, prop_dict):
+    def _add_error_message_and_warn(msg):
+        _add_to_dict(context, prop_dict, 'Pull Result', msg)
+        context.status.warn(msg)
+
+    @request_safely(action_description=f'get all item properties for {_id}',
+                    status=context.status,
+                    on_error=_add_error_message_and_warn)
+    def _request_item_properties():
+        item = context.items_api.get_item_and_all_properties(id=_id)  # type: ItemOutputV1
+        # Name and Type don't appear in additional properties
+        _add_to_dict(context, prop_dict, 'Name', item.name)
+        _add_to_dict(context, prop_dict, 'Type', item.type)
+        _add_to_dict(context, prop_dict, 'Scoped To', _common.none_to_nan(item.scoped_to))
+        for prop in item.properties:  # type: PropertyOutputV1
+            if prop.name not in RESERVED_SEARCH_COLUMN_NAMES:
+                _add_to_dict(context, prop_dict, prop.name, prop.value)
+
+        if item.type in ['CalculatedSignal', 'CalculatedCondition', 'CalculatedScalar', 'LiteralScalar']:
+            formula_output = context.formulas_api.get_item(id=_id)  # type: FormulaItemOutputV1
+            _add_to_dict(context, prop_dict, 'Formula Parameters', [
+                '%s=%s' % (_p.name, _p.item.id if _p.item else _p.formula) for _p in formula_output.parameters
+            ])
+
+        elif item.type == 'ThresholdMetric':
+            formula_parameters = _metadata.formula_parameters_dict_from_threshold_metric(context.session, _id)
+            for key, value in formula_parameters.items():
+                _add_to_dict(context, prop_dict, key, value)
+
+        elif item.type == 'Display':
+            display_output = context.displays_api.get_display(id=_id)
+            _add_to_dict(context, prop_dict, 'Template ID', display_output.template.id)
+            if display_output.swap is not None:
+                _add_to_dict(context, prop_dict, 'Swap Out Asset ID', display_output.swap.swap_out)
+                _add_to_dict(context, prop_dict, 'Swap In Asset ID', display_output.swap.swap_in)
+            else:
+                _add_to_dict(context, prop_dict, 'Swap Out Asset ID', display_output.template.swap_source_asset_id)
+
+        elif item.type == 'DisplayTemplate':
+            display_template_output = context.display_templates_api.get_display_template(id=_id)
+            _add_to_dict(context, prop_dict, 'Source Workstep ID', display_template_output.source_workstep_id)
+
+    _request_item_properties()
+    return prop_dict
+
+
+def _add_tree(context: SearchContext, _id, prop_dict):
+    item_output = None
+    if context.include_swap_info:
+        item_dependency_output = safely(lambda: context.items_api.get_formula_dependencies(id=_id),
+                                        action_description=f'get dependencies for {_id}',
+                                        status=context.status)  # type: ItemDependencyOutputV1
+        if item_dependency_output is not None:
+            item_output = item_dependency_output
+
+        dependencies_with_relevant_assets = _swap.get_swappable_assets(item_dependency_output)
+
+        def _swappable_asset_dict(d):
+            leaf_asset = d.ancestors[-1]
+            return {
+                'ID': leaf_asset.id,
+                'Type': leaf_asset.type,
+                'Path': _common.path_list_to_string([a.name for a in d.ancestors[0:-1]]),
+                'Asset': leaf_asset.name
+            }
+
+        swappable_assets = pd.DataFrame([_swappable_asset_dict(d) for d in dependencies_with_relevant_assets],
+                                        columns=['ID', 'Type', 'Path', 'Asset'])
+
+        _add_to_dict(context, prop_dict, 'Swappable Assets', swappable_assets)
+    else:
+        asset_tree_output = safely(lambda: context.trees_api.get_tree(id=_id),
+                                   action_description=f'get asset tree ancestors for {_id}',
+                                   status=context.status)  # type: AssetTreeOutputV1
+        if asset_tree_output is not None:
+            item_output = asset_tree_output.item
+    if item_output is not None:
+        _add_ancestors_to_prop_dict_from_item_output(context, item_output, prop_dict)
+
+    return prop_dict
+
+
+def _process_query_path_string(context: SearchContext, current_query, kwargs, remaining_query_path_string,
+                               actual_path_list, clauses: dict, asset_id=None):
+    query_path_list = _common.path_string_to_list(remaining_query_path_string)
+
+    query_path_part = query_path_list[0]
+
+    tree_kwargs = dict()
+    tree_kwargs['limit'] = kwargs['limit']
+    tree_kwargs['offset'] = 0
+
+    if 'scope' in kwargs and isinstance(kwargs['scope'], str):
+        tree_kwargs['scope'] = [kwargs['scope']]
+
+    while True:
+        if not asset_id:
+            tree_output = context.trees_api.get_tree_root_nodes(**tree_kwargs)  # type: AssetTreeOutputV1
+        else:
+            tree_kwargs['id'] = asset_id
+            tree_output = context.trees_api.get_tree(**tree_kwargs)  # type: AssetTreeOutputV1
+
+        for child in tree_output.children:  # type: TreeItemOutputV1
+            if not asset_id:
+                @request_safely(action_description=f'check if "{child.name}" {child.id} has '
+                                                   f'datasource matching request',
+                                status=context.status,
+                                default_value=True)
+                def _is_item_in_filter_datasources():
+                    child_item_output = context.items_api.get_item_and_all_properties(
+                        id=child.id)  # type: ItemOutputV1
+                    for prop in ['Datasource Class', 'Datasource ID']:
+                        if prop in clauses:
+                            _, val = clauses[prop]
+                            p_list = [_p.value for _p in child_item_output.properties if
+                                      _p.name == prop]
+                            if len(p_list) == 0 or p_list[0] != val:
+                                return False
+                    return True
+
+                # We only filter out datasource at the top level, in case the tree is mixed
+                if not _is_item_in_filter_datasources():
+                    continue
+
+            if _common.does_query_fragment_match(query_path_part, child.name, contains=False):
+                actual_path_list_for_child = actual_path_list.copy()
+                actual_path_list_for_child.append(child.name)
+                if len(query_path_list) == 1:
+                    kwargs['asset'] = child.id
+                    _gather_results(context, current_query, kwargs, actual_path_list=actual_path_list_for_child)
+                else:
+                    _process_query_path_string(context,
+                                               current_query,
+                                               kwargs,
+                                               _common.path_list_to_string(query_path_list[1:]),
+                                               actual_path_list_for_child,
+                                               clauses,
+                                               child.id)
+
+        if len(tree_output.children) < tree_kwargs['limit']:
+            break
+
+        tree_kwargs['offset'] += tree_kwargs['limit']
+
+
+# noinspection PyUnusedLocal
+def _gather_results_via_item_search(context: SearchContext, current_query, _actual_path_list, _result):
+    item_search_preview = _result  # type: ItemSearchPreviewV1
+    prop_dict = dict()
+
+    _add_ancestors_to_prop_dict_from_item_output(context, item_search_preview, prop_dict)
+
+    uom = item_search_preview.value_unit_of_measure if item_search_preview.value_unit_of_measure \
+        else item_search_preview.source_value_unit_of_measure
+    _add_to_dict(context, prop_dict, 'Value Unit Of Measure', uom)
+    datasource_item_preview = item_search_preview.datasource  # type: ItemPreviewV1
+    _add_to_dict(context, prop_dict, 'Datasource Name',
+                 datasource_item_preview.name if datasource_item_preview else None)
+    _add_common_properties(context, prop_dict, item_search_preview)
+
+
+def _gather_results_via_get_tree(context: SearchContext, current_query, _actual_path_list, _result):
+    tree_item_output = _result  # type: TreeItemOutputV1
+    prop_dict = dict()
+
+    for prop, _attr in [('Name', 'name'), ('Description', 'description')]:
+        if prop not in current_query:
+            continue
+
+        if not _common.does_query_fragment_match(current_query[prop],
+                                                 getattr(tree_item_output, _attr),
+                                                 contains=(context.comparison == '~=')):
+            return
+
+    _add_ancestors_to_prop_dict(
+        context, tree_item_output.type, tree_item_output.name, _actual_path_list, prop_dict)
+
+    _add_to_dict(context, prop_dict, 'Value Unit Of Measure', tree_item_output.value_unit_of_measure)
+    _add_common_properties(context, prop_dict, tree_item_output)
+
+
+def _add_common_properties(context: SearchContext, prop_dict, output_object):
+    _add_to_dict(context, prop_dict, 'ID', output_object.id)
+    _add_to_dict(context, prop_dict, 'Name', output_object.name)
+    _add_to_dict(context, prop_dict, 'Description', output_object.description)
+    _add_to_dict(context, prop_dict, 'Type', output_object.type)
+    _add_to_dict(context, prop_dict, 'Archived', output_object.is_archived)
+    if context.all_properties:
+        _add_all_properties(context, output_object.id, prop_dict)
+    if context.include_swap_info:
+        _add_tree(context, output_object.id, prop_dict)
+    if context.estimate_sample_period is not None:
+        _add_to_dict(context, prop_dict, 'Estimated Sample Period',
+                     context.sample_periods[output_object.id])
+    _add_to_metadata(context, prop_dict)
+
+
+def _iterate_over_output(context: SearchContext, _output_func, _collection_name, _action_func, current_query,
+                         kwargs, _actual_path_list):
+    offset = 0
+    while True:
+        output = _output_func(context, kwargs, offset)
+
+        collection = getattr(output, _collection_name)
+        # Determine sample period for all signals and have NaT for non-signal items
+        if context.estimate_sample_period is not None:
+            for item in collection:
+                if 'Signal' in item.type:
+                    _estimate_sample_period(context, item.id, item.name)
+                else:
+                    context.sample_periods[item.id] = pd.NaT
+
+        context.status.df.at[context.status_index, 'Time'] = _common.timer_elapsed(context.timer)
+        context.status.df.at[context.status_index, 'Count'] = offset + len(collection)
+        context.status.df.at[context.status_index, 'Pages'] += 1
+        context.status.df.at[context.status_index, 'Result'] = 'Querying'
+        context.status.update('Querying Seeq Server for items', Status.RUNNING)
+
+        for item in collection:
+            _action_func(context, current_query, _actual_path_list, item)
+
+        if len(collection) != output.limit:
+            break
+
+        offset += output.limit
+
+
+def _do_search(context: SearchContext, kwargs: dict, offset):
+    kwargs['offset'] = offset
+    if 'scope' in kwargs and isinstance(kwargs['scope'], str):
+        kwargs['scope'] = [kwargs['scope']]
+    if context.use_search_items_api:
+        if context.order_by:
+            kwargs['order_by'] = context.order_by
+        return context.items_api.search_items(**kwargs)
+
+    kwargs2 = {
+        'offset': kwargs['offset'],
+        'limit': kwargs['limit'],
+        'scope': _common.get(kwargs, 'scope'),
+        'exclude_globally_scoped': ('@excludeGloballyScoped' in kwargs['filters'])
+    }
+    if 'asset' in kwargs:
+        kwargs2['id'] = kwargs['asset']
+        tree_output = context.trees_api.get_tree(**kwargs2)
+    else:
+        tree_output = context.trees_api.get_tree_root_nodes(**kwargs2)
+    if len(kwargs['types']) > 0:
+        tree_output.children = [x for x in tree_output.children if x.type in kwargs['types']]
+    return tree_output
+
+
+def _gather_results(context: SearchContext, current_query, kwargs, actual_path_list=None):
+    if context.use_search_items_api:
+        _iterate_over_output(context, _do_search, 'items', _gather_results_via_item_search, current_query, kwargs,
+                             actual_path_list)
+    else:
+        _iterate_over_output(context, _do_search, 'children', _gather_results_via_get_tree, current_query, kwargs,
+                             actual_path_list)
```

### Comparing `seeq-spy-188.0/seeq/spy/_session.py` & `seeq-spy-188.2/seeq/spy/_session.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/_status.py` & `seeq-spy-188.2/seeq/spy/_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import concurrent.futures
 import datetime
 import queue
 import re
 import threading
+from functools import wraps
 from typing import Tuple, Callable, Dict, Optional
 
 import pandas as pd
 from IPython.display import display, HTML
 
 from seeq.spy import _common, _datalab
 from seeq.spy._errors import *
@@ -105,16 +106,37 @@
 
     @property
     def catalogued_errors(self):
         return self._catalogued_errors
 
     @property
     def catalogued_errors_str(self):
-        return 'Errors encountered:\n' + \
-               '\n----------------------------------------\n'.join(self._catalogued_errors)
+        return 'Errors encountered:\n' + '\n----------------------------------------\n'.join(self._catalogued_errors)
+
+    @staticmethod
+    def handle_keyboard_interrupt(*, errors=None, quiet=None):
+        def decorator(func: Callable):
+            @wraps(func)
+            def out(*args, **kwargs):
+                kwargs['status'] = Status.validate(
+                    kwargs.get('status'), kwargs.get('quiet', quiet), kwargs.get('errors', errors))
+
+                for kwarg in ['quiet', 'errors']:
+                    if kwarg in kwargs:
+                        del kwargs[kwarg]
+
+                try:
+                    return func(*args, **kwargs)
+                except KeyboardInterrupt as e:
+                    kwargs['status'].update('Operation canceled', Status.CANCELED)
+                    raise SPyKeyboardInterrupt(e)
+
+            return out
+
+        return decorator
 
     def _drain_updates(self):
         while True:
             try:
                 _index, _updates = self.update_queue.get_nowait()
 
                 for _update_column, _update_value in _updates.items():
```

### Comparing `seeq-spy-188.0/seeq/spy/_swap.py` & `seeq-spy-188.2/seeq/spy/_swap.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     ItemParameterOfOutputV1, ItemPreviewWithAssetsV1
 from seeq.spy import _common, _login
 from seeq.spy._errors import *
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 
 
+@Status.handle_keyboard_interrupt()
 def swap(items: pd.DataFrame, assets: pd.DataFrame, *, partial_swaps_ok: bool = False,
          old_asset_format: Optional[bool] = None, errors: Optional[str] = None, quiet: Optional[bool] = False,
          status: Optional[Status] = None, session: Optional[Session] = None):
     """
     Operates on a DataFrame of items by swapping out the assets that those
     items are based on. The returned DataFrame can be supplied to
     spy.pull() to retrieve the resulting data.
```

### Comparing `seeq-spy-188.0/seeq/spy/_upgrade.py` & `seeq-spy-188.2/seeq/spy/_upgrade.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/_url.py` & `seeq-spy-188.2/seeq/spy/_url.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/acl/_pull.py` & `seeq-spy-188.2/seeq/spy/acl/_pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 from seeq.spy._errors import *
 from seeq.spy._redaction import safely
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 from seeq.spy.workbooks import Item
 
 
+@Status.handle_keyboard_interrupt()
 def pull(items: Union[pd.DataFrame, dict, list, str, Item], *, include_my_effective_permissions: bool = False,
-         errors: Optional[str] = None, quiet: bool = False, status: Optional[Status] = None,
+         errors: Optional[str] = None, quiet: Optional[bool] = None, status: Optional[Status] = None,
          session: Optional[Session] = None) -> pd.DataFrame:
     """
     Pulls access control entries for a set of items as specified
     by their IDs. The most common way to invoke this command is directly
     after having done a spy.search() and produced a DataFrame full of
     items to work with.
```

### Comparing `seeq-spy-188.0/seeq/spy/acl/_push.py` & `seeq-spy-188.2/seeq/spy/acl/_push.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from seeq.spy._errors import *
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 from seeq.spy.acl import _pull
 from seeq.spy.workbooks import Item
 
 
+@Status.handle_keyboard_interrupt()
 def push(items: Union[pd.DataFrame, dict, list, str, Item], acl: Union[pd.DataFrame, dict, list], *,
          replace: bool = False, disable_inheritance: bool = None, errors: Optional[str] = None,
          quiet: Optional[bool] = None, status: Optional[Status] = None, session: Optional[Session] = None
          ) -> pd.DataFrame:
     """
     Pushes new access control entries against a set of items as specified
     by their IDs. The most common way to invoke this command is directly
```

### Comparing `seeq-spy-188.0/seeq/spy/addons/_install.py` & `seeq-spy-188.2/seeq/spy/addons/_install.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from seeq.spy import addons
 from seeq.spy._errors import *
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 from seeq.spy.addons import _permissions
 
 
+@Status.handle_keyboard_interrupt()
 def install(tool: Union[pd.DataFrame, pd.Series, dict, list], *, include_workbook_parameters: bool = True,
             update_tool: bool = False, update_permissions: bool = False, errors: Optional[str] = None,
             quiet: Optional[bool] = None, status: Optional[Status] = None, session: Optional[Session] = None
             ) -> pd.DataFrame:
     """
     Installs or updates Add-on tool(s) in Seeq Workbench.
     Installing Add-on tools requires administrator access.
```

### Comparing `seeq-spy-188.0/seeq/spy/addons/_permissions.py` & `seeq-spy-188.2/seeq/spy/addons/_permissions.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/addons/_search.py` & `seeq-spy-188.2/seeq/spy/addons/_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from seeq.spy import _login
 from seeq.spy._redaction import safely
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 from seeq.spy.addons import _permissions
 
 
+@Status.handle_keyboard_interrupt()
 def search(query: Union[pd.DataFrame, pd.Series, dict, list, str], *, errors: Optional[str] = None,
            quiet: Optional[bool] = None, status: Status = None, session: Optional[Session] = None):
     """
     Issues a query to the Seeq Server to retrieve metadata for Add-on tools.
     This metadata can be used to update or uninstall Add-on tools.
 
     Parameters
```

### Comparing `seeq-spy-188.0/seeq/spy/addons/_uninstall.py` & `seeq-spy-188.2/seeq/spy/addons/_uninstall.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from seeq.spy import _login
 from seeq.spy._errors import *
 from seeq.spy._redaction import request_safely
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 
 
+@Status.handle_keyboard_interrupt()
 def uninstall(items: Union[pd.DataFrame, pd.Series], *, errors: Optional[str] = None, quiet: Optional[bool] = None,
               status: Status = None, session: Optional[Session] = None) -> pd.DataFrame:
     """
     Uninstalls Add-on Tool from the Seeq Workbench. It does not remove the
     target_url contents. Uninstalling Add-on tools requires administrator access.
 
     Parameters
```

### Comparing `seeq-spy-188.0/seeq/spy/assets/_brochure.py` & `seeq-spy-188.2/seeq/spy/assets/_brochure.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/assets/_build.py` & `seeq-spy-188.2/seeq/spy/assets/_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 import inspect
 import re
 import types
 from types import ModuleType
 from typing import List, Union, Type
 
 import pandas as pd
+
 from seeq.spy import _common
 from seeq.spy._errors import *
 from seeq.spy._status import Status
 from seeq.spy.assets._context import SPyInstanceAlreadyExists
 from seeq.spy.assets._model import _AssetBase, BuildContext, BuildPhase, SPyDependencyNotBuilt
 from seeq.spy.workbooks import Workbook
 
 
-def build(model, metadata, *, workbooks=None, errors='catalog', quiet=None, status: Status = None):
+@Status.handle_keyboard_interrupt(errors='catalog')
+def build(model, metadata, *, workbooks=None, errors=None, quiet=None, status: Status = None):
     """
     Utilizes a Python Class-based asset model specification to produce a set
     of item definitions as a metadata DataFrame.
 
     Parameters
     ----------
     model : {ModuleType, type, List[type]}
```

### Comparing `seeq-spy-188.0/seeq/spy/assets/_context.py` & `seeq-spy-188.2/seeq/spy/assets/_context.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/assets/_model.py` & `seeq-spy-188.2/seeq/spy/assets/_model.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/assets/_trees/_constants.py` & `seeq-spy-188.2/seeq/spy/assets/_trees/_constants.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/assets/_trees/_csv.py` & `seeq-spy-188.2/seeq/spy/assets/_trees/_csv.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/assets/_trees/_match.py` & `seeq-spy-188.2/seeq/spy/assets/_trees/_match.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/assets/_trees/_pandas.py` & `seeq-spy-188.2/seeq/spy/assets/_trees/_pandas.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/assets/_trees/_path.py` & `seeq-spy-188.2/seeq/spy/assets/_trees/_path.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/assets/_trees/_properties.py` & `seeq-spy-188.2/seeq/spy/assets/_trees/_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import copy
 import re
 import types
 from typing import Optional
 
 import numpy as np
 import pandas as pd
+
 from seeq.sdk import *
 from seeq.spy import _common, _login, _metadata, _redaction
 from seeq.spy._errors import *
 from seeq.spy._redaction import safely
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 from seeq.spy.assets._model import ItemGroup
@@ -144,15 +145,15 @@
     """
     df = df.reset_index(drop=True)
     df = KeyedDataFrame.of(df)
 
     _safely = _redaction.request_safely(
         action_description='get properties for requested item',
         status=status,
-        default_value=pd.Series(np.nan, index=_constants.dataframe_columns))
+        default_value=pd.Series(np.nan, index=_constants.dataframe_columns, dtype=object))
 
     df = df.apply(_safely(process_row_properties), axis=1,
                   session=session,
                   status=status,
                   pull_nodes=pull_nodes,
                   keep_parent_column=keep_parent_column)
 
@@ -211,15 +212,15 @@
 # Note that the session argument is second in this special case because we call this from pd.DataFrame.apply(),
 # which requires that row is the first argument.
 def process_row_properties(row, session: Session, status, pull_nodes, keep_parent_column) -> pd.Series:
     if _common.present(row, 'ID') and pull_nodes:
         new_row = pull_node(session, row['ID'])
         _utils.increment_status_df(status, pulled_items=[new_row])
     else:
-        new_row = pd.Series(index=_constants.dataframe_columns, dtype='object')
+        new_row = pd.Series(index=_constants.dataframe_columns, dtype=object)
 
     # In case that properties are specified, but IDs are given, the user-given properties
     # override those pulled from Seeq
     for prop, value in row.items():
         if prop == 'Type' and _common.present(new_row, 'Type'):
             continue
         if prop in ['Path', 'Asset']:
@@ -351,15 +352,15 @@
 def pull_node(session: Session, node_id) -> pd.Series:
     """
     Returns a dataframe row corresponding to the item given by node_id
     """
     items_api = _login.get_api(session, ItemsApi)
 
     item_output = items_api.get_item_and_all_properties(id=node_id)  # type: ItemOutputV1
-    node = pd.Series(index=_constants.dataframe_columns, dtype='object')
+    node = pd.Series(index=_constants.dataframe_columns, dtype=object)
 
     # Extract only the properties we use
     node['Name'] = item_output.name
     node['Type'] = item_output.type
     node['ID'] = item_output.id  # If this should be a copy, it'll be converted to 'Referenced ID' later
     for prop in item_output.properties:  # type: PropertyOutputV1
         add_tree_property(node, prop.name, prop.value)
@@ -403,16 +404,16 @@
                 raise SPyException(f'Formula Parameter: {param} needs to be in the format \'paramName=inputItem\'.')
             formula_dictionary[split_list[0].strip()] = split_list[1].strip()
     return formula_dictionary  # output == {'x': '2b17adfd-3308-4c03-bdfb-bf4419bf7b3a'}
 
 
 def format_references(df) -> pd.DataFrame:
     out_df = df.copy()
-    out_df['Formula Parameters'] = pd.Series(np.nan, index=df.index, dtype='object')
-    out_df['Thresholds'] = pd.Series(np.nan, index=df.index, dtype='object')
+    out_df['Formula Parameters'] = pd.Series(np.nan, index=df.index, dtype=object)
+    out_df['Thresholds'] = pd.Series(np.nan, index=df.index, dtype=object)
 
     for node in _match.TreeNode.of(df):  # type: _match.TreeNode
         if pd.api.types.is_dict_like(df.loc[node.index, 'Formula Parameters']):
             formula_parameters = copy.deepcopy(df.loc[node.index, 'Formula Parameters'])
             for name, reference in formula_parameters.items():
                 if not isinstance(reference, str) or _common.is_guid(reference):
                     continue
```

### Comparing `seeq-spy-188.0/seeq/spy/assets/_trees/_pull.py` & `seeq-spy-188.2/seeq/spy/assets/_trees/_pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     If any nodes already exist in the dataframe (by case-insensitive Path+Name), the existing row will be kept.
     """
     if df.empty:
         return df
 
     for col in ['ID', 'Referenced ID']:
         if col not in df.columns:
-            df[col] = pd.Series(np.nan, dtype='object')
+            df[col] = pd.Series(np.nan, dtype=object)
     # Gather all Paths+IDs into a list upfront
     items_to_pull_children = df[(~pd.isnull(df['ID'])) | (~pd.isnull(df['Referenced ID']))]
 
     for _, row in items_to_pull_children.iterrows():
         if _common.get(row, 'Type') != 'Asset':
             continue
 
@@ -230,16 +230,16 @@
                     and root.scoped_to.upper() == workbook_id
                     and item_output_has_sdl_datasource(root, datasource))
 
     existing_spy_trees = find_root_nodes(session, workbook_id, _spy_tree_root_filter)
 
     def _row_is_spy_tree_root(_row, root_id, root_name):
         return (_common.present(_row, 'ID') and _row['ID'].casefold() == root_id.casefold()) \
-               and (not _common.present(_row, 'Name') or _row['Name'].casefold() == root_name.casefold()) \
-               and (not _common.get(_row, 'Path'))
+            and (not _common.present(_row, 'Name') or _row['Name'].casefold() == root_name.casefold()) \
+            and (not _common.get(_row, 'Path'))
 
     df_root_id = None
     for spy_tree in existing_spy_trees:
         for _, row in df.iterrows():
             if _row_is_spy_tree_root(row, spy_tree.id, spy_tree.name):
                 if df_root_id is None:
                     df_root_id = row['ID']
```

### Comparing `seeq-spy-188.0/seeq/spy/assets/_trees/_tree.py` & `seeq-spy-188.2/seeq/spy/assets/_trees/_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,15 @@
     _workbook = _common.DEFAULT_WORKBOOK_PATH
     _workbook_id = _constants.UNKNOWN  # Placeholder for the ID of a workbook that hasn't been pushed yet
 
     session: Session
     status: Status
     is_dirty = False
 
+    @Status.handle_keyboard_interrupt()
     def __init__(self, data, *, friendly_name=None, description=None, workbook=_common.DEFAULT_WORKBOOK_PATH,
                  datasource=None, convert_displays_to_sdl=True, quiet=None, errors=None, status=None,
                  session: Optional[Session] = None):
         _common.validate_argument_types([
             (data, 'data', (pd.DataFrame, str)),
             (friendly_name, 'friendly_name', str),
             (description, 'description', str),
@@ -275,14 +276,15 @@
         df = _validate.validate_and_filter(self.session, df, self.status, stage='final',
                                            temporal_description='while creating tree',
                                            subtract_errors_from_status=True)
 
         self._dataframe = df
         self.status.update(f'{status_message} {self.summarize(ret=True)}', Status.SUCCESS)
 
+    # @Status.handle_keyboard_interrupt()
     def insert(self, children=None, parent=None, *, name=None, formula=None, formula_parameters=None,
                roll_up_statistic=None, roll_up_parameters=None, friendly_name=None, errors=None, quiet=None,
                status=None):
         """
         Insert the specified elements into the tree.
 
         Parameters
@@ -376,15 +378,15 @@
             (roll_up_statistic, 'roll_up_statistic', str),
             (roll_up_parameters, 'roll_up_parameters', str),
             (errors, 'errors', str),
             (quiet, 'quiet', bool),
             (status, 'status', Status)
         ])
 
-        status = self.validate_status(status, quiet, errors)
+        status = Status.validate(status, quiet, errors)
 
         if children is None:
             names = [arg for arg in (name, friendly_name) if arg is not None]
             if len(names) != 1:
                 raise SPyValueError('If no `children` argument is given, exactly one of the following arguments must '
                                     'be given: `name`, `friendly_name`')
             else:
@@ -544,15 +546,15 @@
         _common.validate_argument_types([
             (elements, 'elements', (pd.DataFrame, str, int)),
             (errors, 'errors', str),
             (quiet, 'quiet', bool),
             (status, 'status', Status)
         ])
 
-        status = self.validate_status(status, quiet, errors)
+        status = Status.validate(status, quiet, errors)
 
         _utils.initialize_status_df(status, 'Removed', 'Removing items from tree', Status.RUNNING)
 
         drop_rows_mask = _match.Query(self._dataframe).matches(elements).with_descendants().get_mask()
         working_df = self._dataframe.loc[~drop_rows_mask].reset_index(drop=True)
 
         _utils.increment_status_df(status, new_items=self._dataframe.loc[drop_rows_mask])
@@ -616,15 +618,15 @@
             (source, 'source', (pd.DataFrame, str)),
             (destination, 'destination', (pd.DataFrame, str)),
             (errors, 'errors', str),
             (quiet, 'quiet', bool),
             (status, 'status', Status)
         ])
 
-        status = self.validate_status(status, quiet, errors)
+        status = Status.validate(status, quiet, errors)
 
         _utils.initialize_status_df(status, 'Moved', 'Moving items in tree.', Status.RUNNING)
 
         # Find the destination. Fail if there is not exactly one match for the input
         destination_query = _match.Query(self._dataframe).matches(destination)
         destination_nodes = destination_query.get_node_list()
         if len(destination_nodes) == 0:
@@ -996,15 +998,15 @@
             (start, 'start', (str, pd.Timestamp, datetime.date)),
             (end, 'end', (str, pd.Timestamp, datetime.date)),
             (errors, 'errors', str),
             (quiet, 'quiet', bool),
             (status, 'status', Status)
         ])
 
-        status = self.validate_status(status, quiet, errors)
+        status = Status.validate(status, quiet, errors)
 
         if condition is None and within is None:
             raise SPyValueError("At least one of `condition` or `within` arguments must be provided")
 
         if condition is not None:
             if self.is_dirty:
                 raise SPyRuntimeError("Tree is dirty. Call the push function to commit the changes before calling "
@@ -1040,14 +1042,15 @@
         _utils.increment_status_df(status, new_items=result_df, error_items=error_conditions)
 
         tree_summary = re.sub(r'^The tree ".*"', 'The down-selected tree', result.summarize(ret=True))
         status.update(f'Successfully created down-selected tree. {tree_summary}', Status.SUCCESS)
 
         return result
 
+    @Status.handle_keyboard_interrupt()
     def push(self, *, metadata_state_file: Optional[str] = None, errors: Optional[str] = None,
              quiet: Optional[bool] = None, status: Optional[Status] = None) -> pd.DataFrame:
         """
         Imports the tree into Seeq Server.
 
         metadata_state_file : str, optional
             The file name (with full path, if desired) to a "metadata state file"
@@ -1085,15 +1088,15 @@
         """
         _common.validate_argument_types([
             (errors, 'errors', str),
             (quiet, 'quiet', bool),
             (status, 'status', Status)
         ])
 
-        status = self.validate_status(status, quiet, errors)
+        status = Status.validate(status, quiet, errors)
 
         if self._workbook is not None:
             self._push_workbook()
 
         _properties.push_and_replace_display_templates(self.session, self._dataframe, self._display_template_map,
                                                        self._datasource, self._workbook_id, status)
         self._display_template_map.clear()
@@ -1148,23 +1151,14 @@
         elif self.session.client:
             search_query, _ = _push.create_analysis_search_query(self._workbook)
             search_df = spy.workbooks.search(search_query, status=status, session=self.session)
             self._workbook_id = search_df.iloc[0]['ID'] if len(search_df) > 0 else _constants.UNKNOWN
         else:
             self._workbook_id = _constants.UNKNOWN
 
-    def validate_status(self, status: Status, quiet: Optional[bool], errors: Optional[str]):
-        if status is None:
-            status = Status()
-
-        status.errors = errors if errors is not None else self.status.errors
-        status.quiet = quiet if quiet is not None else self.status.quiet
-
-        return status
-
 
 class DownSelectedTree(Tree):
     # noinspection PyMissingConstructor
     def __init__(self, original: Tree):
         self._dataframe = pd.DataFrame()
         self._datasource = original._datasource
         self._workbook = original._workbook
```

### Comparing `seeq-spy-188.0/seeq/spy/assets/_trees/_utils.py` & `seeq-spy-188.2/seeq/spy/assets/_trees/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
 
 def visualize(df):
     if df.iloc[0].Depth != 1:
         df = df.copy()
         df['Depth'] = df['Depth'] - df.iloc[0].Depth + 1
 
-    show_vertical_columns = pd.Series([False] * (df['Depth'].max() - 2))
+    show_vertical_columns = pd.Series([False] * (df['Depth'].max() - 2), dtype=bool)
     lines = []
     for idx in reversed(df.index):
         depth = df.loc[idx, 'Depth']
         name = df.loc[idx, 'Name']
         if depth == 1:
             line = name
         else:
```

### Comparing `seeq-spy-188.0/seeq/spy/assets/_trees/_validate.py` & `seeq-spy-188.2/seeq/spy/assets/_trees/_validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from typing import Tuple, List
 
 import pandas as pd
+
 from seeq.spy import _common, _metadata, _status
 from seeq.spy._errors import *
 from seeq.spy._session import Session
 from seeq.spy.assets._trees import _constants, _match, _path, _utils
 from seeq.spy.assets._trees._pandas import KeyedDataFrame
 
 
@@ -137,15 +138,15 @@
     # - The dataframe is sorted by path
     # - There are no missing assets referenced in paths
     # - Paths reflect names of preceding items
     # - Depths reflects lengths of paths
 
     size = len(df)
     if size == 0:
-        return ['Tree must be non-empty.'], pd.Series(dtype='string')
+        return ['Tree must be non-empty.'], pd.Series(dtype=str)
 
     error_series = pd.Series('', index=df.index)
     error_summaries = []
     if ignore_rows is None:
         ignore_rows = pd.Series(False, index=df.index)
 
     prev_path = list()
```

### Comparing `seeq-spy-188.0/seeq/spy/assets/brochure.html` & `seeq-spy-188.2/seeq/spy/assets/brochure.html`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Administration/User Migration.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Administration/User Migration.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Command Reference.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Command Reference.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/Example Export.zip` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/Example Export.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Tutorial.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Version Considerations.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Version Considerations.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/Workbook Templates.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/Workbook Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.acl.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.acl.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.jobs.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.jobs.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.login.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.login.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.pull.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.pull.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.push.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.push.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.search.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.search.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.swap.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.swap.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.widgets.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.widgets.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/Documentation/spy.workbooks.ipynb` & `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.workbooks.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/docs/_copy.py` & `seeq-spy-188.2/seeq/spy/docs/_copy.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/jobs/_execute.py` & `seeq-spy-188.2/seeq/spy/jobs/_execute.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/jobs/_pull.py` & `seeq-spy-188.2/seeq/spy/jobs/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/jobs/_push.py` & `seeq-spy-188.2/seeq/spy/jobs/_push.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from seeq.spy import _common, _datalab
 from seeq.spy._errors import *
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 from seeq.spy.jobs import _schedule
 
 
+@Status.handle_keyboard_interrupt(errors='raise')
 def push(jobs_df: pd.DataFrame, spread: Optional[str] = None, datalab_notebook_url: Optional[str] = None,
          label: Optional[str] = None, user: Optional[str] = None,
          interactive_index: Union[Optional[int], Optional[str]] = None, suspend: bool = False,
          quiet: Optional[bool] = None, status: Optional[Status] = None, session: Optional[Session] = None):
     """
     Schedules the automatic execution of a notebook and returns the row
     corresponding for the currently running schedule.
@@ -127,15 +128,15 @@
         (interactive_index, 'interactive_index', (int, str)),
         (suspend, 'suspend', bool),
         (quiet, 'quiet', bool),
         (status, 'status', Status),
         (session, 'session', Session)
     ])
 
-    status = Status.validate(status, quiet, errors='raise')
+    status = Status.validate(status, quiet)
     session = Session.validate(session)
 
     try:
         _schedule.schedule_df(session, jobs_df=jobs_df, spread=spread, datalab_notebook_url=datalab_notebook_url,
                               label=label, user=user, suspend=suspend, status=status)
     except SchedulePostingError:
         # When the notebook is executed as a job, push will first re-schedule the notebook. If any errors will happen
```

### Comparing `seeq-spy-188.0/seeq/spy/jobs/_schedule.py` & `seeq-spy-188.2/seeq/spy/jobs/_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from seeq.sdk import *
 from seeq.spy import _common, _login, _datalab
 from seeq.spy._errors import *
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 
 
+@Status.handle_keyboard_interrupt(errors='raise')
 def schedule(schedule_spec: str, datalab_notebook_url: Optional[str] = None, label: Optional[str] = None,
              user: Optional[str] = None, suspend: bool = False, quiet: Optional[bool] = None,
              status: Optional[Status] = None, session: Optional[Session] = None):
     """
     Schedules the automatic execution of a Seeq Data Lab notebook.
 
     The current notebook is scheduled for execution unless datalab_notebook_url
```

### Comparing `seeq-spy-188.0/seeq/spy/notifications/_emails.py` & `seeq-spy-188.2/seeq/spy/notifications/_emails.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/utils/__init__.py` & `seeq-spy-188.2/seeq/spy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/widgets/_ipy_utils.py` & `seeq-spy-188.2/seeq/spy/widgets/_ipy_utils.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/widgets/_widgets.py` & `seeq-spy-188.2/seeq/spy/widgets/_widgets.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/__init__.py` & `seeq-spy-188.2/seeq/spy/workbooks/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_annotation.py` & `seeq-spy-188.2/seeq/spy/workbooks/_annotation.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_content.py` & `seeq-spy-188.2/seeq/spy/workbooks/_content.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_data.py` & `seeq-spy-188.2/seeq/spy/workbooks/_data.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_folder.py` & `seeq-spy-188.2/seeq/spy/workbooks/_folder.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_item.py` & `seeq-spy-188.2/seeq/spy/workbooks/_item.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_item_map.py` & `seeq-spy-188.2/seeq/spy/workbooks/_item_map.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_load.py` & `seeq-spy-188.2/seeq/spy/workbooks/_load.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_mustache.py` & `seeq-spy-188.2/seeq/spy/workbooks/_mustache.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_pull.py` & `seeq-spy-188.2/seeq/spy/workbooks/_pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from seeq.spy import _login
 from seeq.spy._errors import *
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 from seeq.spy.workbooks._workbook import Workbook, WorkbookList
 
 
+@Status.handle_keyboard_interrupt()
 def pull(workbooks_df: Union[pd.DataFrame, str], *, include_referenced_workbooks: bool = True,
          include_inventory: bool = True, include_annotations: bool = True, include_images: bool = True,
          include_rendered_content: bool = False, specific_worksheet_ids: Optional[List[str]] = None,
          errors: Optional[str] = None, quiet: Optional[bool] = None, status: Optional[Status] = None,
          session: Optional[Session] = None) -> Optional[WorkbookList]:
     """
     Pulls the definitions for each workbook specified by workbooks_df into
```

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_push.py` & `seeq-spy-188.2/seeq/spy/workbooks/_push.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from seeq.spy.workbooks import _user
 from seeq.spy.workbooks._annotation import Annotation
 from seeq.spy.workbooks._item import Item, ItemMap
 from seeq.spy.workbooks._template import ItemTemplate
 from seeq.spy.workbooks._workbook import Workbook, WorkbookList
 
 
+@Status.handle_keyboard_interrupt()
 def push(workbooks, *, path=None, owner=None, label=None, datasource=None, datasource_map_folder=None,
          use_full_path=False, access_control=None, override_max_interp=False,
          include_inventory=None, include_annotations: bool = True, scope_globals_to_workbook=False, refresh=True,
          lookup_df: pd.DataFrame = None, specific_worksheet_ids: Optional[List[str]] = None, errors=None, quiet=None,
          status: Optional[Status] = None, session: Optional[Session] = None):
     """
     Pushes workbooks into Seeq using a list of Workbook object definitions.
```

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_render.py` & `seeq-spy-188.2/seeq/spy/workbooks/_render.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_report_content_utilities.py` & `seeq-spy-188.2/seeq/spy/workbooks/_report_content_utilities.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_save.py` & `seeq-spy-188.2/seeq/spy/workbooks/_save.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_search.py` & `seeq-spy-188.2/seeq/spy/workbooks/_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from seeq.spy._errors import *
 from seeq.spy._redaction import safely, request_safely
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 from seeq.spy.workbooks._folder import SYNTHETIC_FOLDERS, synthetic_folder_to_content_filter
 
 
+@Status.handle_keyboard_interrupt()
 def search(query, *, content_filter='owner', all_properties=False, recursive=False, include_archived=False,
            errors=None, quiet=None, status=None, session: Optional[Session] = None):
     """
     Issues a query to the Seeq Server to retrieve metadata for workbooks.
     This metadata can be used to pull workbook definitions into memory.
 
     Parameters
```

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_template.py` & `seeq-spy-188.2/seeq/spy/workbooks/_template.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_user.py` & `seeq-spy-188.2/seeq/spy/workbooks/_user.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_workbook.py` & `seeq-spy-188.2/seeq/spy/workbooks/_workbook.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_worksheet.py` & `seeq-spy-188.2/seeq/spy/workbooks/_worksheet.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/_workstep.py` & `seeq-spy-188.2/seeq/spy/workbooks/_workstep.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq/spy/workbooks/app.css` & `seeq-spy-188.2/seeq/spy/workbooks/app.css`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/seeq_spy.egg-info/PKG-INFO` & `seeq-spy-188.2/seeq_spy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 188.0
+Version: 188.2
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -31,14 +31,16 @@
 - Import data in a programmatic way (when Seeq Workbench's *CSV Import* capability won't cut it)
 - Calculate new data in Python and push it into Seeq
 - Create an asset model
 - Programmatically create and manipulate Workbench Analyses or Organizer Topics
 
 **Use of the SPy module requires Python 3.7 or later.**
 
+**SPy version 187 and higher is compatible with Pandas 2.x.**
+
 To start exploring the SPy module, execute the following lines of code in Jupyter:
 
 ```
 from seeq import spy
 spy.docs.copy()
 ```
```

### Comparing `seeq-spy-188.0/seeq_spy.egg-info/SOURCES.txt` & `seeq-spy-188.2/seeq_spy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.0/setup.py` & `seeq-spy-188.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seeq-spy",
-    version="188.0",
+    version="188.2",
     author="Seeq Corporation",
     author_email="support@seeq.com",
     description="Easy-to-use Python interface for Seeq",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.seeq.com",
     project_urls={
```

