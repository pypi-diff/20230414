# Comparing `tmp/seeq-spy-186.9.tar.gz` & `tmp/seeq-spy-187.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\seeq-spy-186.9.tar", last modified: Wed Apr  5 20:38:30 2023, max compression
+gzip compressed data, was "dist\seeq-spy-187.0.tar", last modified: Thu Apr 13 22:01:16 2023, max compression
```

## Comparing `seeq-spy-186.9.tar` & `seeq-spy-187.0.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:30.000000 seeq-spy-186.9/
--rw-rw-rw-   0        0        0    33551 2023-01-30 20:12:10.000000 seeq-spy-186.9/LICENSE
--rw-rw-rw-   0        0        0      207 2023-01-30 20:12:10.000000 seeq-spy-186.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4541 2023-04-05 20:38:30.000000 seeq-spy-186.9/PKG-INFO
--rw-rw-rw-   0        0        0     4026 2023-01-30 20:12:10.000000 seeq-spy-186.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq/
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq/base/
--rw-rw-rw-   0        0        0       36 2023-04-05 20:38:26.000000 seeq-spy-186.9/seeq/base/__init__.py
--rw-rw-rw-   0        0        0      875 2023-04-05 20:38:26.000000 seeq-spy-186.9/seeq/base/proputil.py
--rw-rw-rw-   0        0        0    30471 2023-04-05 20:38:26.000000 seeq-spy-186.9/seeq/base/seeq_names.py
--rw-rw-rw-   0        0        0    39566 2023-04-05 20:38:26.000000 seeq-spy-186.9/seeq/base/system.py
--rw-rw-rw-   0        0        0     4788 2023-04-05 20:38:26.000000 seeq-spy-186.9/seeq/base/util.py
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq/scripts/
--rw-rw-rw-   0        0        0    44531 2023-04-05 20:38:26.000000 seeq-spy-186.9/seeq/scripts/create_monitoring_workbook.py
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq/spy/
--rw-rw-rw-   0        0        0     1912 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/__init__.py
--rw-rw-rw-   0        0        0    29824 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_common.py
--rw-rw-rw-   0        0        0     4687 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_config.py
--rw-rw-rw-   0        0        0     4424 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_datalab.py
--rw-rw-rw-   0        0        0     9686 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_errors.py
--rw-rw-rw-   0        0        0    45760 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_login.py
--rw-rw-rw-   0        0        0    91580 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_metadata.py
--rw-rw-rw-   0        0        0     5822 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_metadata_push_results.py
--rw-rw-rw-   0        0        0     2954 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_plot.py
--rw-rw-rw-   0        0        0    55353 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_pull.py
--rw-rw-rw-   0        0        0    68529 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_push.py
--rw-rw-rw-   0        0        0     5155 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_redaction.py
--rw-rw-rw-   0        0        0    41125 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_search.py
--rw-rw-rw-   0        0        0    18978 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_session.py
--rw-rw-rw-   0        0        0    15704 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_status.py
--rw-rw-rw-   0        0        0     7069 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_upgrade.py
--rw-rw-rw-   0        0        0    10707 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/_url.py
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq/spy/acl/
--rw-rw-rw-   0        0        0      104 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/acl/__init__.py
--rw-rw-rw-   0        0        0    12057 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/acl/_pull.py
--rw-rw-rw-   0        0        0    11313 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/acl/_push.py
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq/spy/addons/
--rw-rw-rw-   0        0        0      188 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/addons/__init__.py
--rw-rw-rw-   0        0        0    26338 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/addons/_install.py
--rw-rw-rw-   0        0        0     2408 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/addons/_permissions.py
--rw-rw-rw-   0        0        0    12099 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/addons/_search.py
--rw-rw-rw-   0        0        0     5303 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/addons/_uninstall.py
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq/spy/assets/
--rw-rw-rw-   0        0        0      336 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/__init__.py
--rw-rw-rw-   0        0        0     3638 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_brochure.py
--rw-rw-rw-   0        0        0    12106 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_build.py
--rw-rw-rw-   0        0        0     3133 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_context.py
--rw-rw-rw-   0        0        0    48166 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_model.py
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq/spy/assets/_trees/
--rw-rw-rw-   0        0        0       69 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_trees/__init__.py
--rw-rw-rw-   0        0        0     1358 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_trees/_constants.py
--rw-rw-rw-   0        0        0     7302 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_trees/_csv.py
--rw-rw-rw-   0        0        0    19962 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_trees/_match.py
--rw-rw-rw-   0        0        0     2629 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_trees/_pandas.py
--rw-rw-rw-   0        0        0     6458 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_trees/_path.py
--rw-rw-rw-   0        0        0    23200 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_trees/_properties.py
--rw-rw-rw-   0        0        0    13341 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_trees/_pull.py
--rw-rw-rw-   0        0        0    58684 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_trees/_tree.py
--rw-rw-rw-   0        0        0     5842 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_trees/_utils.py
--rw-rw-rw-   0        0        0    25528 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/_trees/_validate.py
--rw-rw-rw-   0        0        0     2538 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/assets/brochure.html
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq/spy/docs/
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Advanced Scheduling/
--rw-rw-rw-   0        0        0    17105 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
--rw-rw-rw-   0        0        0    33412 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
--rw-rw-rw-   0        0        0    16369 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
--rw-rw-rw-   0        0        0     8406 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
--rw-rw-rw-   0        0        0    38705 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
--rw-rw-rw-   0        0        0      870 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
--rw-rw-rw-   0        0        0   184846 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
--rw-rw-rw-   0        0        0   222283 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
--rw-rw-rw-   0        0        0   228808 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
--rw-rw-rw-   0        0        0    24125 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Attached Images/
--rw-rw-rw-   0        0        0   135771 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
--rw-rw-rw-   0        0        0   152116 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
--rw-rw-rw-   0        0        0   207271 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
--rw-rw-rw-   0        0        0      325 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Attached Images/Readme.txt
--rw-rw-rw-   0        0        0   141516 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
--rw-rw-rw-   0        0        0   439966 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
--rw-rw-rw-   0        0        0   189377 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
--rw-rw-rw-   0        0        0    15176 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Command Reference.ipynb
--rw-rw-rw-   0        0        0    94844 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Example Export.zip
--rw-rw-rw-   0        0        0   112234 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Report and Dashboard Templates.zip
--rw-rw-rw-   0        0        0   673871 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Tutorial.ipynb
--rw-rw-rw-   0        0        0    11411 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Version Considerations.ipynb
--rw-rw-rw-   0        0        0  1556897 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Workbook Templates.ipynb
--rw-rw-rw-   0        0        0   113431 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/Workbook Templates.zip
--rw-rw-rw-   0        0        0     1310 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/better_metadata.pickle
--rw-rw-rw-   0        0        0    62414 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/company_logo.png
--rw-rw-rw-   0        0        0  1083835 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/csv_import_example.csv
--rw-rw-rw-   0        0        0    53871 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/spy.acl.ipynb
--rw-rw-rw-   0        0        0    11009 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/spy.jobs.ipynb
--rw-rw-rw-   0        0        0    12828 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/spy.login.ipynb
--rw-rw-rw-   0        0        0   128038 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/spy.pull.ipynb
--rw-rw-rw-   0        0        0    99342 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/spy.push.ipynb
--rw-rw-rw-   0        0        0    54441 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/spy.search.ipynb
--rw-rw-rw-   0        0        0    10645 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/spy.widgets.ipynb
--rw-rw-rw-   0        0        0    69627 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/spy.workbooks.ipynb
--rw-rw-rw-   0        0        0      429 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/Documentation/spy_tree_example.csv
--rw-rw-rw-   0        0        0       60 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/docs/_copy.py
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:30.000000 seeq-spy-186.9/seeq/spy/jobs/
--rw-rw-rw-   0        0        0      491 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/jobs/__init__.py
--rw-rw-rw-   0        0        0     9869 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/jobs/_execute.py
--rw-rw-rw-   0        0        0     6111 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/jobs/_pull.py
--rw-rw-rw-   0        0        0     9362 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/jobs/_push.py
--rw-rw-rw-   0        0        0    25680 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/jobs/_schedule.py
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:30.000000 seeq-spy-186.9/seeq/spy/notifications/
--rw-rw-rw-   0        0        0      153 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/notifications/__init__.py
--rw-rw-rw-   0        0        0    11926 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/notifications/_emails.py
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:30.000000 seeq-spy-186.9/seeq/spy/utils/
--rw-rw-rw-   0        0        0     1516 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:30.000000 seeq-spy-186.9/seeq/spy/widgets/
--rw-rw-rw-   0        0        0      200 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/widgets/__init__.py
--rw-rw-rw-   0        0        0     4158 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/widgets/_ipy_utils.py
--rw-rw-rw-   0        0        0    30480 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/widgets/_widgets.py
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:30.000000 seeq-spy-186.9/seeq/spy/workbooks/
--rw-rw-rw-   0        0        0     3018 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/__init__.py
--rw-rw-rw-   0        0        0    41007 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_annotation.py
--rw-rw-rw-   0        0        0    25884 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_content.py
--rw-rw-rw-   0        0        0    40535 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_data.py
--rw-rw-rw-   0        0        0     6677 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_folder.py
--rw-rw-rw-   0        0        0    14959 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_item.py
--rw-rw-rw-   0        0        0     5448 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_item_map.py
--rw-rw-rw-   0        0        0     3033 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_load.py
--rw-rw-rw-   0        0        0     3456 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_mustache.py
--rw-rw-rw-   0        0        0    14137 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_pull.py
--rw-rw-rw-   0        0        0    23050 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_push.py
--rw-rw-rw-   0        0        0     6318 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_render.py
--rw-rw-rw-   0        0        0     4729 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_save.py
--rw-rw-rw-   0        0        0    15479 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_search.py
--rw-rw-rw-   0        0        0    37305 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_template.py
--rw-rw-rw-   0        0        0    11971 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_user.py
--rw-rw-rw-   0        0        0    52402 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_workbook.py
--rw-rw-rw-   0        0        0    48031 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_worksheet.py
--rw-rw-rw-   0        0        0    50398 2023-04-05 20:38:28.000000 seeq-spy-186.9/seeq/spy/workbooks/_workstep.py
--rw-rw-rw-   0        0        0   427362 2023-04-05 20:38:27.000000 seeq-spy-186.9/seeq/spy/workbooks/app.css
-drwxrwxrwx   0        0        0        0 2023-04-05 20:38:30.000000 seeq-spy-186.9/seeq_spy.egg-info/
--rw-rw-rw-   0        0        0     4541 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq_spy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4597 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq_spy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq_spy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-07 21:47:26.000000 seeq-spy-186.9/seeq_spy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      311 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq_spy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-05 20:38:29.000000 seeq-spy-186.9/seeq_spy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 20:38:30.000000 seeq-spy-186.9/setup.cfg
--rw-rw-rw-   0        0        0     1677 2023-04-05 20:37:10.000000 seeq-spy-186.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/
+-rw-rw-rw-   0        0        0    33551 2023-01-30 20:12:10.000000 seeq-spy-187.0/LICENSE
+-rw-rw-rw-   0        0        0      207 2023-01-30 20:12:10.000000 seeq-spy-187.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4541 2023-04-13 22:01:16.000000 seeq-spy-187.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4026 2023-01-30 20:12:10.000000 seeq-spy-187.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/base/
+-rw-rw-rw-   0        0        0       36 2023-04-13 22:01:11.000000 seeq-spy-187.0/seeq/base/__init__.py
+-rw-rw-rw-   0        0        0      875 2023-04-13 22:01:11.000000 seeq-spy-187.0/seeq/base/proputil.py
+-rw-rw-rw-   0        0        0    30471 2023-04-13 22:01:11.000000 seeq-spy-187.0/seeq/base/seeq_names.py
+-rw-rw-rw-   0        0        0    39566 2023-04-13 22:01:11.000000 seeq-spy-187.0/seeq/base/system.py
+-rw-rw-rw-   0        0        0     4788 2023-04-13 22:01:11.000000 seeq-spy-187.0/seeq/base/util.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/scripts/
+-rw-rw-rw-   0        0        0    44531 2023-04-13 22:01:11.000000 seeq-spy-187.0/seeq/scripts/create_monitoring_workbook.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/spy/
+-rw-rw-rw-   0        0        0     1912 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/__init__.py
+-rw-rw-rw-   0        0        0    29824 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_common.py
+-rw-rw-rw-   0        0        0     4687 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_config.py
+-rw-rw-rw-   0        0        0     4424 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_datalab.py
+-rw-rw-rw-   0        0        0     9686 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_errors.py
+-rw-rw-rw-   0        0        0    48626 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_login.py
+-rw-rw-rw-   0        0        0    91580 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_metadata.py
+-rw-rw-rw-   0        0        0     5822 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_metadata_push_results.py
+-rw-rw-rw-   0        0        0     2954 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_plot.py
+-rw-rw-rw-   0        0        0    55502 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_pull.py
+-rw-rw-rw-   0        0        0    68531 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_push.py
+-rw-rw-rw-   0        0        0     5155 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_redaction.py
+-rw-rw-rw-   0        0        0    41125 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_search.py
+-rw-rw-rw-   0        0        0    18978 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_session.py
+-rw-rw-rw-   0        0        0    15704 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_status.py
+-rw-rw-rw-   0        0        0     3471 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_upgrade.py
+-rw-rw-rw-   0        0        0    10707 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/_url.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/spy/acl/
+-rw-rw-rw-   0        0        0      104 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/acl/__init__.py
+-rw-rw-rw-   0        0        0    12125 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/acl/_pull.py
+-rw-rw-rw-   0        0        0    11313 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/acl/_push.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/spy/addons/
+-rw-rw-rw-   0        0        0      188 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/addons/__init__.py
+-rw-rw-rw-   0        0        0    26338 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/addons/_install.py
+-rw-rw-rw-   0        0        0     2408 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/addons/_permissions.py
+-rw-rw-rw-   0        0        0    12099 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/addons/_search.py
+-rw-rw-rw-   0        0        0     5296 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/addons/_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/spy/assets/
+-rw-rw-rw-   0        0        0      336 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/__init__.py
+-rw-rw-rw-   0        0        0     3638 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_brochure.py
+-rw-rw-rw-   0        0        0    12106 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_build.py
+-rw-rw-rw-   0        0        0     3133 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_context.py
+-rw-rw-rw-   0        0        0    48166 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_model.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/spy/assets/_trees/
+-rw-rw-rw-   0        0        0       69 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_trees/__init__.py
+-rw-rw-rw-   0        0        0     1358 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_trees/_constants.py
+-rw-rw-rw-   0        0        0     7302 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_trees/_csv.py
+-rw-rw-rw-   0        0        0    22068 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_trees/_match.py
+-rw-rw-rw-   0        0        0     2629 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_trees/_pandas.py
+-rw-rw-rw-   0        0        0     6458 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_trees/_path.py
+-rw-rw-rw-   0        0        0    23200 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_trees/_properties.py
+-rw-rw-rw-   0        0        0    13341 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_trees/_pull.py
+-rw-rw-rw-   0        0        0    58690 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_trees/_tree.py
+-rw-rw-rw-   0        0        0     5854 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_trees/_utils.py
+-rw-rw-rw-   0        0        0    25528 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/_trees/_validate.py
+-rw-rw-rw-   0        0        0     2538 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/assets/brochure.html
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/spy/docs/
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Advanced Scheduling/
+-rw-rw-rw-   0        0        0    17105 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
+-rw-rw-rw-   0        0        0    33412 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
+-rw-rw-rw-   0        0        0    16369 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
+-rw-rw-rw-   0        0        0     8406 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
+-rw-rw-rw-   0        0        0    38705 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
+-rw-rw-rw-   0        0        0      870 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
+-rw-rw-rw-   0        0        0   184846 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
+-rw-rw-rw-   0        0        0   222294 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
+-rw-rw-rw-   0        0        0   228808 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
+-rw-rw-rw-   0        0        0    24125 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Attached Images/
+-rw-rw-rw-   0        0        0   135771 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
+-rw-rw-rw-   0        0        0   152116 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
+-rw-rw-rw-   0        0        0   207271 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
+-rw-rw-rw-   0        0        0      325 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Attached Images/Readme.txt
+-rw-rw-rw-   0        0        0   141516 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
+-rw-rw-rw-   0        0        0   439966 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
+-rw-rw-rw-   0        0        0   189377 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
+-rw-rw-rw-   0        0        0    15176 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Command Reference.ipynb
+-rw-rw-rw-   0        0        0    94844 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Example Export.zip
+-rw-rw-rw-   0        0        0   112234 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Report and Dashboard Templates.zip
+-rw-rw-rw-   0        0        0   673871 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Tutorial.ipynb
+-rw-rw-rw-   0        0        0    11411 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Version Considerations.ipynb
+-rw-rw-rw-   0        0        0  1556897 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Workbook Templates.ipynb
+-rw-rw-rw-   0        0        0   113431 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/Workbook Templates.zip
+-rw-rw-rw-   0        0        0     1310 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/better_metadata.pickle
+-rw-rw-rw-   0        0        0    62414 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/company_logo.png
+-rw-rw-rw-   0        0        0  1083835 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/csv_import_example.csv
+-rw-rw-rw-   0        0        0    53871 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/spy.acl.ipynb
+-rw-rw-rw-   0        0        0    11009 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/spy.jobs.ipynb
+-rw-rw-rw-   0        0        0    12828 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/spy.login.ipynb
+-rw-rw-rw-   0        0        0   127929 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/spy.pull.ipynb
+-rw-rw-rw-   0        0        0    99342 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/spy.push.ipynb
+-rw-rw-rw-   0        0        0    54441 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/spy.search.ipynb
+-rw-rw-rw-   0        0        0    10645 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/spy.widgets.ipynb
+-rw-rw-rw-   0        0        0    69627 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/spy.workbooks.ipynb
+-rw-rw-rw-   0        0        0      429 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/Documentation/spy_tree_example.csv
+-rw-rw-rw-   0        0        0       60 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/docs/_copy.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/spy/jobs/
+-rw-rw-rw-   0        0        0      491 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/jobs/__init__.py
+-rw-rw-rw-   0        0        0     9869 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/jobs/_execute.py
+-rw-rw-rw-   0        0        0     6111 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/jobs/_pull.py
+-rw-rw-rw-   0        0        0     9362 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/jobs/_push.py
+-rw-rw-rw-   0        0        0    25680 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/jobs/_schedule.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/spy/notifications/
+-rw-rw-rw-   0        0        0      153 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/notifications/__init__.py
+-rw-rw-rw-   0        0        0    11926 2023-04-13 22:01:12.000000 seeq-spy-187.0/seeq/spy/notifications/_emails.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/spy/utils/
+-rw-rw-rw-   0        0        0     1516 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/spy/widgets/
+-rw-rw-rw-   0        0        0      200 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4158 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/widgets/_ipy_utils.py
+-rw-rw-rw-   0        0        0    30480 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/widgets/_widgets.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq/spy/workbooks/
+-rw-rw-rw-   0        0        0     3018 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/__init__.py
+-rw-rw-rw-   0        0        0    41007 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_annotation.py
+-rw-rw-rw-   0        0        0    25884 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_content.py
+-rw-rw-rw-   0        0        0    40535 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_data.py
+-rw-rw-rw-   0        0        0     6677 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_folder.py
+-rw-rw-rw-   0        0        0    14959 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_item.py
+-rw-rw-rw-   0        0        0     5448 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_item_map.py
+-rw-rw-rw-   0        0        0     3033 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_load.py
+-rw-rw-rw-   0        0        0     3456 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_mustache.py
+-rw-rw-rw-   0        0        0    14137 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_pull.py
+-rw-rw-rw-   0        0        0    23050 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_push.py
+-rw-rw-rw-   0        0        0     6318 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_render.py
+-rw-rw-rw-   0        0        0     4729 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_save.py
+-rw-rw-rw-   0        0        0    15507 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_search.py
+-rw-rw-rw-   0        0        0    37305 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_template.py
+-rw-rw-rw-   0        0        0    11995 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_user.py
+-rw-rw-rw-   0        0        0    52402 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_workbook.py
+-rw-rw-rw-   0        0        0    48031 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_worksheet.py
+-rw-rw-rw-   0        0        0    50418 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/_workstep.py
+-rw-rw-rw-   0        0        0   427362 2023-04-13 22:01:13.000000 seeq-spy-187.0/seeq/spy/workbooks/app.css
+drwxrwxrwx   0        0        0        0 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq_spy.egg-info/
+-rw-rw-rw-   0        0        0     4541 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq_spy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4597 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq_spy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq_spy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-07 21:47:26.000000 seeq-spy-187.0/seeq_spy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      311 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq_spy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-13 22:01:16.000000 seeq-spy-187.0/seeq_spy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 22:01:16.000000 seeq-spy-187.0/setup.cfg
+-rw-rw-rw-   0        0        0     1677 2023-04-13 21:57:48.000000 seeq-spy-187.0/setup.py
```

### Comparing `seeq-spy-186.9/LICENSE` & `seeq-spy-187.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/PKG-INFO` & `seeq-spy-187.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 186.9
+Version: 187.0
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seeq-spy-186.9/README.md` & `seeq-spy-187.0/README.md`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/base/proputil.py` & `seeq-spy-187.0/seeq/base/proputil.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/base/seeq_names.py` & `seeq-spy-187.0/seeq/base/seeq_names.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/base/system.py` & `seeq-spy-187.0/seeq/base/system.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/base/util.py` & `seeq-spy-187.0/seeq/base/util.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/scripts/create_monitoring_workbook.py` & `seeq-spy-187.0/seeq/scripts/create_monitoring_workbook.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/__init__.py` & `seeq-spy-187.0/seeq/spy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,8 +53,8 @@
 """
 
 __all__ = ['acl', 'addons', 'assets', 'docs', 'workbooks', 'widgets', 'login', 'logout', 'plot', 'pull', 'push',
            'search', 'PATH_ROOT', 'DEFAULT_WORKBOOK_PATH', 'GLOBALS_ONLY', 'GLOBALS_AND_ALL_WORKBOOKS',
            'INHERIT_FROM_WORKBOOK', 'Session', 'Status', 'options', 'session', 'client', 'user', 'server_version',
            'jobs', 'notifications', 'upgrade', 'utils', 'errors']
 
-__version__ = '%d.%d' % (int('186'), int('9'))
+__version__ = '%d.%d' % (int('187'), int('0'))
```

### Comparing `seeq-spy-186.9/seeq/spy/_common.py` & `seeq-spy-187.0/seeq/spy/_common.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/_config.py` & `seeq-spy-187.0/seeq/spy/_config.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/_datalab.py` & `seeq-spy-187.0/seeq/spy/_datalab.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/_errors.py` & `seeq-spy-187.0/seeq/spy/_errors.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/_login.py` & `seeq-spy-187.0/seeq/spy/_login.py`

 * *Files 2% similar despite different names*

```diff
@@ -787,40 +787,88 @@
     else:
         if sdk_module_major != seeq_server_major:
             message = (f'The major version of the seeq module ({sdk_module_major}) '
                        f'does not match the major version of the Seeq Server you are connected to '
                        f'({seeq_server_major}) and is incompatible.')
 
     if message is not None:
-        compatible_module_folder = find_compatible_module(session)
-        if not compatible_module_folder:
-            message += (f'\n\nIt is recommended that you run spy.upgrade() or issue the following PIP command to '
-                        f'install a compatible version of the seeq module:\n')
-            if using_old_server_versioning_scheme:
-                message += generate_seeq_module_pip_upgrade(
-                    f'{seeq_server_major}.{seeq_server_minor}.{seeq_server_patch}')
-            else:
-                message += generate_seeq_module_pip_upgrade(f'{seeq_server_major}.{seeq_server_minor}')
-        else:
-            message += (f'\n\nA compatible module was found here: {compatible_module_folder}\n'
-                        f'Consider uninstalling your project-specific seeq module by issuing the following PIP '
-                        f'command:\n'
-                        f'pip uninstall -y seeq')
+        message += (f'\n\nIt is recommended that you run spy.upgrade() or issue the following PIP command to '
+                    f'install a compatible version of the seeq module:\n')
+        message += generate_pip_upgrade_command(session)
 
         if allow_version_mismatch or session.options.allow_version_mismatch:
             status.warn(message)
         else:
             raise SPyRuntimeError(message)
 
     return seeq_server_major, seeq_server_minor, seeq_server_patch
 
 
-def generate_seeq_module_pip_upgrade(version, exact_match_version=False):
-    matcher = '==' if exact_match_version else '~='
-    return f'pip install -U seeq{matcher}{version}'
+def generate_pip_upgrade_command(session: Session, version: Optional[str] = None, use_testpypi: bool = False):
+    sdk_module_major, sdk_module_minor, _ = get_sdk_module_version_tuple()
+    seeq_server_major, seeq_server_minor, seeq_server_patch = get_server_version_tuple(session)
+    compatible_module_folder = find_compatible_module(session)
+    # The old versioning scheme is like 0.49.3 whereas the new scheme is like 50.1.8
+    # See https://seeq.atlassian.net/wiki/spaces/SQ/pages/947225963/Seeq+Versioning+Simplification
+    using_old_versioning_scheme = (seeq_server_major == 0)
+    first_command = None
+    if using_old_versioning_scheme:
+        install_compatible_sdk = (sdk_module_major != seeq_server_major or sdk_module_minor != seeq_server_minor)
+        compatible_sdk_version_specifier = f'{seeq_server_major}.{seeq_server_minor}.{seeq_server_patch}'
+    else:
+        install_compatible_sdk = (sdk_module_major != seeq_server_major)
+        compatible_sdk_version_specifier = f'{seeq_server_major}.{seeq_server_minor}'
+    repository_arg = ' --index-url https://test.pypi.org/simple/' if use_testpypi else ''
+
+    def _install_compatible_sdk():
+        if not install_compatible_sdk:
+            return None
+
+        if compatible_module_folder is not None:
+            return 'pip uninstall -y seeq'
+        else:
+            return f'pip install -U{repository_arg} seeq~={compatible_sdk_version_specifier}'
+
+    if version is not None:
+        if 'r' in version.lower():
+            version = re.sub(pattern='r', repl='', string=version, flags=re.IGNORECASE)
+
+        match = re.match(r'^(\d+)\..*', version)
+        if not match:
+            raise SPyValueError(f'version argument "{version}" is not a full version (e.g. 221.13 or 58.0.2.184.12)')
+
+        version_major = int(match.group(1))
+        if version_major < SEEQ_SERVER_VERSION_WHERE_SPY_IS_IN_ITS_OWN_PACKAGE:
+            # We're going to the old single-package scheme, where seeq and spy are in the same package and the
+            # versioning is something like 58.0.2.184.12. If the currently-installed sdk module is R60 or later, we must
+            # uninstall the seeq-spy package so that, when the older seeq package (which includes spy directly) is
+            # installed, pip doesn't think that seeq-spy is still installed as well.
+            if sdk_module_major >= SEEQ_SERVER_VERSION_WHERE_SPY_IS_IN_ITS_OWN_PACKAGE:
+                first_command = 'pip uninstall -y seeq-spy'
+
+            second_command = f'pip install -U{repository_arg} seeq=={version}'
+        else:
+            # We're going to the new seeq-spy package scheme.
+            if seeq_server_major < SEEQ_SERVER_VERSION_WHERE_SPY_IS_IN_ITS_OWN_PACKAGE:
+                raise SPyValueError(f'version argument "{version}" is incompatible with Seeq Server version '
+                                    f'{session.server_version}')
+
+            first_command = _install_compatible_sdk()
+            second_command = f'pip install -U{repository_arg} seeq-spy=={version}'
+    else:
+        if seeq_server_major >= SEEQ_SERVER_VERSION_WHERE_SPY_IS_IN_ITS_OWN_PACKAGE:
+            first_command = _install_compatible_sdk()
+            second_command = f'pip install -U{repository_arg} seeq-spy'
+        else:
+            if sdk_module_major >= SEEQ_SERVER_VERSION_WHERE_SPY_IS_IN_ITS_OWN_PACKAGE:
+                first_command = 'pip uninstall -y seeq-spy'
+            second_command = f'pip install -U{repository_arg} seeq~={compatible_sdk_version_specifier}'
+    pip_commands = [second_command] if first_command is None else [first_command, second_command]
+    pip_command = ' && '.join(pip_commands)
+    return pip_command
 
 
 def find_compatible_module(session: Session):
     """
     Uses pkg_resources tools to look for a seeq module that is compatible with the version of Seeq Server we're
     connected to. This function is useful in Seeq Data Lab scenarios where the user has installed a "private" version of
     the seeq module (presumably to get a bugfix for SPy) but Seeq Server and Seeq Data Lab have been upgraded in the
```

### Comparing `seeq-spy-186.9/seeq/spy/_metadata.py` & `seeq-spy-187.0/seeq/spy/_metadata.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/_metadata_push_results.py` & `seeq-spy-187.0/seeq/spy/_metadata_push_results.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/_plot.py` & `seeq-spy-187.0/seeq/spy/_plot.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/_pull.py` & `seeq-spy-187.0/seeq/spy/_pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,15 @@
                                 "DataFrame, or a Series. When applying a calculation to a signal/condition/scalar, "
                                 'calculation must be a string with a signal variable in it: $signal, $condition or '
                                 '$scalar.')
 
         calculation = calculation.iloc[0]
 
     if isinstance(items, pd.Series):
-        items = pd.DataFrame().append(items)
+        items = pd.DataFrame([items])
 
     if shape not in ['auto', 'capsules', 'samples']:
         raise SPyValueError("shape must be one of 'auto', 'capsules', 'samples'")
 
     if capsule_properties is not None and not isinstance(capsule_properties, list):
         raise SPyValueError("capsules_properties must be a list of strings (capsule property names)")
 
@@ -491,18 +491,20 @@
             for existing_column in existing_columns:
                 output.df[existing_column] = np.nan
 
         if shape == 'capsules':
             # When the shape of the output is capsules, it's effectively just a long
             # DataFrame with all of the results appended one after the other. The user can
             # then choose to sort by one of the columns if they would like.
-            output.df = output.df.append(result_list, ignore_index=True)
+            result_list.insert(0, output.df)
+            output.df = pd.concat(result_list, ignore_index=True)
         else:
             if group_by:
-                output.df = output.df.append(result_list)
+                result_list.insert(0, output.df)
+                output.df = pd.concat(result_list)
                 output.df = output.df.groupby(['Timestamp'] + group_by).first()
             else:
                 # noinspection PyTypeChecker
                 output.df = output.df.join(result_list, how='outer')
 
     status.update(f'Pull successful from <strong>{pd_start}</strong> to <strong>{pd_end}</strong>', Status.SUCCESS)
 
@@ -685,19 +687,19 @@
     _update_status_rows(f'Success', capsule_count, page_count)
 
     return RowResult(row_index, column_names, result_df)
 
 
 def _is_capsule_dupe(result_df, item_name, pd_capsule_start, pd_capsule_end):
     return 'Condition' in result_df and \
-           'Capsule Start' in result_df and \
-           'Capsule End' in result_df and \
-           len(result_df.loc[(result_df['Condition'] == item_name) &
-                             (result_df['Capsule Start'] == pd_capsule_start) &
-                             (result_df['Capsule End'] == pd_capsule_end)])
+        'Capsule Start' in result_df and \
+        'Capsule End' in result_df and \
+        len(result_df.loc[(result_df['Condition'] == item_name) &
+                          (result_df['Capsule Start'] == pd_capsule_start) &
+                          (result_df['Capsule End'] == pd_capsule_end)])
 
 
 def _pull_condition_via_formula_api(session: Session, calculation_to_use, shape, capsule_properties, current_start,
                                     index_to_use, item_id, item_name, offset, pd_end, tz, result_df,
                                     column_names):
     formulas_api = FormulasApi(session.client)
     parameters = ['condition=%s' % item_id]
@@ -757,15 +759,15 @@
         for col, series in columns.items():
             result_df[col] = series
             column_names[item_id].append(col)
     else:
         # In this case, we're creating a more straightforward table where each capsule is a row, complete with item
         # properties.
 
-        capsule_df_rows = list()
+        capsule_dict_list = list()
         if len(capsules_output['capsules']) > 0:
             column_names[item_id] = ['Condition', 'Capsule Start', 'Capsule End', 'Capsule Is Uncertain']
 
         for capsule in capsules_output['capsules']:  # type: dict
             capsule_start = capsule.get('start', None)
             capsule_end = capsule.get('end', None)
             pd_capsule_start = _common.convert_to_timestamp(capsule_start, tz)
@@ -787,20 +789,21 @@
                 if capsule_properties is not None and prop['name'] not in capsule_properties:
                     continue
 
                 capsule_dict[prop['name']] = prop.get('value', None)
                 if prop['name'] not in column_names[item_id]:
                     column_names[item_id].append(prop['name'])
 
-            capsule_df_rows.append(capsule_dict)
+            capsule_dict_list.append(capsule_dict)
 
             if not pd.isna(capsule_start) and capsule_start > next_start:
                 next_start = capsule_start
 
-        result_df = result_df.append(capsule_df_rows) if len(result_df) != 0 else pd.DataFrame(capsule_df_rows)
+        result_df = (pd.concat([result_df, pd.DataFrame(capsule_dict_list)])
+                     if len(result_df) != 0 else pd.DataFrame(capsule_dict_list))
 
     return len(capsules_output['capsules']), next_start, result_df
 
 
 def _build_limit_fragment(offset, limit):
     start_row = offset + 1  # Table object is 1-based, not 0
     end_row = start_row + limit
@@ -912,16 +915,16 @@
             column_names[item_id].append(column_name)
 
         capsule_df_rows.append(capsule_dict)
 
         if not pd.isna(capsule_start) and capsule_start > next_start:
             next_start = capsule_end
 
-    formula_result_df = result_df.copy().append(capsule_df_rows) if len(result_df) != 0 else pd.DataFrame(
-        capsule_df_rows)
+    formula_result_df = (pd.concat([result_df, pd.DataFrame(capsule_df_rows)])
+                         if len(result_df) != 0 else pd.DataFrame(capsule_df_rows))
 
     return len(formula_table), next_start, formula_result_df
 
 
 def _pull_signal(session: Session, formula, parameters, item_id, item_name, pd_start, pd_end, tz,
                  status: Status = None, row_index=None, bounding_values=False, invalid_values_as=np.nan,
                  enums_as='string'):
@@ -984,15 +987,15 @@
                             _keep_sample(sample_output)]
         timestamps = [sample['key'] for sample in filtered_samples]
         values = [_sanitize_pi_enums(sample.get('value', None), enums_as) for sample in filtered_samples]
 
         time_index = _convert_column_timezone(pd.DatetimeIndex(timestamps), tz)
 
         new_series = pd.Series(values, index=time_index, dtype=object)
-        series = new_series if series is None else series.append(new_series)
+        series = new_series if series is None else pd.concat([series, new_series])
 
         page_count += 1
 
         if len(series_samples_output['samples']) < session.options.pull_page_size:
             break
 
         if len(series) > 0:
```

### Comparing `seeq-spy-186.9/seeq/spy/_push.py` & `seeq-spy-187.0/seeq/spy/_push.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,15 +425,15 @@
                         }
 
                     else:
                         # Metadata has not been supplied and the column name is not an ID, so just create a
                         # "blank" row in the status DataFrame.
                         ad_hoc_status_df = pd.DataFrame({'Count': 0, 'Pages': 0, 'Time': 0, 'Result': 'Pushing'},
                                                         index=[status_index])
-                        status.df = status.df.append(ad_hoc_status_df, sort=True)
+                        status.df = pd.concat([status.df, ad_hoc_status_df], sort=True)
                         status.update()
                         signal_metadata = dict()
 
                     if not _common.present(signal_metadata, 'Name'):
                         if '>>' in column:
                             raise SPyRuntimeError(
                                 'Paths in column name not currently supported. Supply a metadata argument if you '
@@ -940,15 +940,15 @@
         interval_input.end = pd_end
         add_samples_input.interval = interval_input
 
     if data is not None:
         # Performance notes: It was found that pulling out the column as a pd.Series and then using series.iteritems()
         #                    instead of doing data.iterrows() was 5x-6x faster
         series: pd.Series = data[column]
-        for index, sample_value in series.iteritems():
+        for index, sample_value in series.items():
             if pd.isna(sample_value) and sample_value is not None:
                 continue
 
             if not isinstance(index, pd.Timestamp):
                 raise SPyRuntimeError('data index must only be pd.Timestamp objects, but %s found instead' %
                                       type(index))
```

### Comparing `seeq-spy-186.9/seeq/spy/_redaction.py` & `seeq-spy-187.0/seeq/spy/_redaction.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/_search.py` & `seeq-spy-187.0/seeq/spy/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/_session.py` & `seeq-spy-187.0/seeq/spy/_session.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/_status.py` & `seeq-spy-187.0/seeq/spy/_status.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/_url.py` & `seeq-spy-187.0/seeq/spy/_url.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/acl/_pull.py` & `seeq-spy-187.0/seeq/spy/acl/_pull.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import types
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
+
 from seeq import spy
 from seeq.sdk import *
 from seeq.spy import _common, _login, _metadata
 from seeq.spy._errors import *
 from seeq.spy._redaction import safely
 from seeq.spy._session import Session
 from seeq.spy._status import Status
@@ -237,22 +238,22 @@
 def items_to_data_frame(items):
     if isinstance(items, str):
         new_items = pd.DataFrame([{'ID': items}])
     elif isinstance(items, list):
         new_items = pd.DataFrame()
         for item in items:
             if isinstance(item, str):
-                new_items = new_items.append({'ID': item}, ignore_index=True)
+                new_items = pd.concat([new_items, pd.DataFrame([{'ID': item}])], ignore_index=True)
             elif isinstance(item, dict):
-                new_items = new_items.append(item, ignore_index=True)
+                new_items = pd.concat([new_items, pd.DataFrame([item])], ignore_index=True)
             elif isinstance(item, Item):
-                new_items = new_items.append({
+                new_items = pd.concat([new_items, pd.DataFrame([{
                     'ID': item.id,
                     'Name': item.name
-                }, ignore_index=True)
+                }])], ignore_index=True)
     elif isinstance(items, dict):
         new_items = pd.DataFrame([items])
     elif isinstance(items, pd.DataFrame):
         new_items = items
     elif isinstance(items, Item):
         new_items = pd.DataFrame([{
             'ID': items.id,
```

### Comparing `seeq-spy-186.9/seeq/spy/acl/_push.py` & `seeq-spy-187.0/seeq/spy/acl/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/addons/_install.py` & `seeq-spy-187.0/seeq/spy/addons/_install.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/addons/_permissions.py` & `seeq-spy-187.0/seeq/spy/addons/_permissions.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/addons/_search.py` & `seeq-spy-187.0/seeq/spy/addons/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/addons/_uninstall.py` & `seeq-spy-187.0/seeq/spy/addons/_uninstall.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     _login.validate_login(session, status)
     system_api = SystemApi(session.client)
 
     if 'ID' not in items:
         raise SPyValueError('items DataFrame must include "ID" column which is typically obtained from '
                             '"spy.addons.search"')
     if isinstance(items, pd.Series):
-        items = pd.DataFrame().append(items)
+        items = pd.DataFrame([items])
     if not isinstance(items, pd.DataFrame):
         raise SPyTypeError('item must be a pandas.Series or pandas.DataFrame')
 
     status_columns = [c for c in ['ID', 'Name', 'Target URL'] if c in items]
 
     status.df = items[status_columns].copy()
     status.df['Count'] = 0
```

### Comparing `seeq-spy-186.9/seeq/spy/assets/_brochure.py` & `seeq-spy-187.0/seeq/spy/assets/_brochure.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/assets/_build.py` & `seeq-spy-187.0/seeq/spy/assets/_build.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/assets/_context.py` & `seeq-spy-187.0/seeq/spy/assets/_context.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/assets/_model.py` & `seeq-spy-187.0/seeq/spy/assets/_model.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/assets/_trees/_constants.py` & `seeq-spy-187.0/seeq/spy/assets/_trees/_constants.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/assets/_trees/_csv.py` & `seeq-spy-187.0/seeq/spy/assets/_trees/_csv.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/assets/_trees/_match.py` & `seeq-spy-187.0/seeq/spy/assets/_trees/_match.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     path: str = dataclasses.field(init=False, repr=True, compare=False)
     index: int = dataclasses.field(init=True, repr=False, compare=True)
     size: int = dataclasses.field(init=True, repr=False, compare=False)
     parent: TreeNode = dataclasses.field(init=False, repr=False, compare=False)
     root: TreeNode = dataclasses.field(init=False, repr=False, compare=False)
 
     @staticmethod
-    @functools.lru_cache(maxsize=32)
     def of(df: KeyedDataFrame) -> TreeNode:
         return TreeNode._of(df.reset_index().to_dict(orient='records'))
 
     @staticmethod
     def _of(records: List[dict], set_as_root=True, offset=0) -> TreeNode:
         root = records[offset]
         root_depth = root['Depth']
@@ -124,15 +123,15 @@
         if isinstance(pattern, list):
             return any(self.matches(sub_pattern) for sub_pattern in pattern)
         if pd.api.types.is_dict_like(pattern):
             if _common.present(pattern, 'ID'):
                 return pattern['ID'] == self.id or pattern['ID'] == self.referenced_id
             if _common.present(pattern, 'Name'):
                 return (not _common.present(pattern, 'Path') or _path.determine_path(pattern) == self.path) \
-                       and pattern['Name'] == self.name
+                    and pattern['Name'] == self.name
             return False
         if isinstance(pattern, str):
             if _common.is_guid(pattern):
                 return pattern.upper() == self.id
             else:
                 return self.matches_path(_common.path_string_to_list(pattern))
         if isinstance(pattern, int):
@@ -442,19 +441,77 @@
 
     try:
         return re.sub(r'{({.*?}.*?)}', _fill_column_value, query)
     except SPyValueError:
         return np.nan
 
 
+def fnmatch_translate_from_py3_7_8(pat):
+    """
+    This code is copied from Python 3.7.8 source code. This function changed significantly in 3.10 and is
+    incompatible with the fixups that we do in glob_with_capture_groups_to_regex() to hack in a "capture group"
+    facility to the glob.
+    """
+
+    i, n = 0, len(pat)
+    res = ''
+    while i < n:
+        c = pat[i]
+        i = i + 1
+        if c == '*':
+            res = res + '.*'
+        elif c == '?':
+            res = res + '.'
+        elif c == '[':
+            j = i
+            if j < n and pat[j] == '!':
+                j = j + 1
+            if j < n and pat[j] == ']':
+                j = j + 1
+            while j < n and pat[j] != ']':
+                j = j + 1
+            if j >= n:
+                res = res + '\\['
+            else:
+                stuff = pat[i:j]
+                if '--' not in stuff:
+                    stuff = stuff.replace('\\', r'\\')
+                else:
+                    chunks = []
+                    k = i + 2 if pat[i] == '!' else i + 1
+                    while True:
+                        k = pat.find('-', k, j)
+                        if k < 0:
+                            break
+                        chunks.append(pat[i:k])
+                        i = k + 1
+                        k = k + 3
+                    chunks.append(pat[i:j])
+                    # Escape backslashes and hyphens for set difference (--).
+                    # Hyphens that create ranges shouldn't be escaped.
+                    stuff = '-'.join(s.replace('\\', r'\\').replace('-', r'\-')
+                                     for s in chunks)
+                # Escape set operations (&&, ~~ and ||).
+                stuff = re.sub(r'([&~|])', r'\\\1', stuff)
+                i = j + 1
+                if stuff[0] == '!':
+                    stuff = '^' + stuff[1:]
+                elif stuff[0] in ('^', '['):
+                    stuff = '\\' + stuff
+                res = '%s[%s]' % (res, stuff)
+        else:
+            res = res + re.escape(c)
+    return r'(?s:%s)\Z' % res
+
+
 def glob_with_capture_groups_to_regex(glob):
     """
     Converts a glob to a regex, but does not escape parentheses, so that the glob can be written with capture groups
     """
-    return re.sub(r'\\([()])', r'\1', fnmatch.translate(glob))
+    return re.sub(r'\\([()])', r'\1', fnmatch_translate_from_py3_7_8(glob))
 
 
 @functools.lru_cache(maxsize=2048)
 def exact_or_glob_or_regex(pat: str) -> re.Pattern:
     try:
         return re.compile('(?i)' + '(' + ')|('.join([re.escape(pat), fnmatch.translate(pat), pat]) + ')')
     except re.error:
```

### Comparing `seeq-spy-186.9/seeq/spy/assets/_trees/_pandas.py` & `seeq-spy-187.0/seeq/spy/assets/_trees/_pandas.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/assets/_trees/_path.py` & `seeq-spy-187.0/seeq/spy/assets/_trees/_path.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/assets/_trees/_properties.py` & `seeq-spy-187.0/seeq/spy/assets/_trees/_properties.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/assets/_trees/_pull.py` & `seeq-spy-187.0/seeq/spy/assets/_trees/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/assets/_trees/_tree.py` & `seeq-spy-187.0/seeq/spy/assets/_trees/_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,15 +463,15 @@
                                                         self._datasource, status)
 
         # We concatenate all children to be inserted into one dataframe before
         # inserting them using a single pd.merge call
         additions = list()
         if 'Parent' in children.columns:
             for node, matched_indices in _match.Query(self._dataframe).multimatch(children['Parent']):
-                children_to_add = _path.set_children_path(children.loc[matched_indices].copy(), node.full_path,
+                children_to_add = _path.set_children_path(children.loc[list(matched_indices)].copy(), node.full_path,
                                                           node.depth)
                 additions.append(children_to_add)
         else:
             for node in _match.Query(self._dataframe).matches(parent).get_node_set():
                 children_to_add = _path.set_children_path(children.copy(), node.full_path, node.depth)
                 additions.append(children_to_add)
```

### Comparing `seeq-spy-186.9/seeq/spy/assets/_trees/_utils.py` & `seeq-spy-187.0/seeq/spy/assets/_trees/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def set_name(df, new_name):
     df = df.copy()
     old_name = df.loc[0, 'Name']
 
     df.loc[0, 'Name'] = new_name
     pattern = re.compile(r'^' + re.escape(old_name) + r'(?=\s*>>|$)', flags=re.IGNORECASE)
-    df['Path'] = df['Path'].str.replace(pattern, new_name)
+    df['Path'] = df['Path'].str.replace(pattern, new_name, regex=True)
     df['ID'] = np.nan
 
     return df
 
 
 def upsert(df1, df2, prefer_right=True):
     """
```

### Comparing `seeq-spy-186.9/seeq/spy/assets/_trees/_validate.py` & `seeq-spy-187.0/seeq/spy/assets/_trees/_validate.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/assets/brochure.html` & `seeq-spy-187.0/seeq/spy/assets/brochure.html`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975626026272578%*

 * *Differences: {"'cells'": '{27: {\'source\': {insert: [(5, "metadata_df.loc[metadata_df[\'Name\'] == \'Area '*

 * *            'A_Temperature\', \'Build Asset\'] = \'Refrigerator 1\'\\n"), (6, '*

 * *            '"metadata_df.loc[metadata_df[\'Name\'] == \'Area A_Compressor Power\', \'Build '*

 * *            'Asset\'] = \'Refrigerator 1\'\\n"), (7, "metadata_df.loc[metadata_df[\'Name\'] == '*

 * *            '\'Area A_Compressor Power\', \'Compressor\'] = \'Compressor 1\'\\n"), (8, '*

 * *            '"metadata_df.loc[metadata_df[\'Name\'] == \ […]*

```diff
@@ -3138,24 +3138,24 @@
             ],
             "source": [
                 "metadata_df = spy.search({\n",
                 "    'Name': r'/Area [A-D]_(?:Temperature|Compressor Power)/',\n",
                 "    'Datasource Class': 'Time Series CSV Files'\n",
                 "})\n",
                 "\n",
-                "metadata_df.at[metadata_df['Name'] == 'Area A_Temperature', 'Build Asset'] = 'Refrigerator 1'\n",
-                "metadata_df.at[metadata_df['Name'] == 'Area A_Compressor Power', 'Build Asset'] = 'Refrigerator 1'\n",
-                "metadata_df.at[metadata_df['Name'] == 'Area A_Compressor Power', 'Compressor'] = 'Compressor 1'\n",
-                "metadata_df.at[metadata_df['Name'] == 'Area B_Compressor Power', 'Build Asset'] = 'Refrigerator 1'\n",
-                "metadata_df.at[metadata_df['Name'] == 'Area B_Compressor Power', 'Compressor'] = 'Compressor 2'\n",
-                "metadata_df.at[metadata_df['Name'] == 'Area C_Temperature', 'Build Asset'] = 'Refrigerator 2'\n",
-                "metadata_df.at[metadata_df['Name'] == 'Area C_Compressor Power', 'Build Asset'] = 'Refrigerator 2'\n",
-                "metadata_df.at[metadata_df['Name'] == 'Area C_Compressor Power', 'Compressor'] = 'Compressor 3'\n",
-                "metadata_df.at[metadata_df['Name'] == 'Area D_Compressor Power', 'Build Asset'] = 'Refrigerator 2'\n",
-                "metadata_df.at[metadata_df['Name'] == 'Area D_Compressor Power', 'Compressor'] = 'Compressor 4'\n",
+                "metadata_df.loc[metadata_df['Name'] == 'Area A_Temperature', 'Build Asset'] = 'Refrigerator 1'\n",
+                "metadata_df.loc[metadata_df['Name'] == 'Area A_Compressor Power', 'Build Asset'] = 'Refrigerator 1'\n",
+                "metadata_df.loc[metadata_df['Name'] == 'Area A_Compressor Power', 'Compressor'] = 'Compressor 1'\n",
+                "metadata_df.loc[metadata_df['Name'] == 'Area B_Compressor Power', 'Build Asset'] = 'Refrigerator 1'\n",
+                "metadata_df.loc[metadata_df['Name'] == 'Area B_Compressor Power', 'Compressor'] = 'Compressor 2'\n",
+                "metadata_df.loc[metadata_df['Name'] == 'Area C_Temperature', 'Build Asset'] = 'Refrigerator 2'\n",
+                "metadata_df.loc[metadata_df['Name'] == 'Area C_Compressor Power', 'Build Asset'] = 'Refrigerator 2'\n",
+                "metadata_df.loc[metadata_df['Name'] == 'Area C_Compressor Power', 'Compressor'] = 'Compressor 3'\n",
+                "metadata_df.loc[metadata_df['Name'] == 'Area D_Compressor Power', 'Build Asset'] = 'Refrigerator 2'\n",
+                "metadata_df.loc[metadata_df['Name'] == 'Area D_Compressor Power', 'Compressor'] = 'Compressor 4'\n",
                 "\n",
                 "metadata_df['Build Path'] = 'Refrigerator Units'\n",
                 "\n",
                 "metadata_df[['ID', 'Name', 'Build Path', 'Build Asset', 'Compressor']]"
             ]
         },
         {
@@ -4459,13 +4459,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.8"
+            "version": "3.8.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Command Reference.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Command Reference.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Example Export.zip` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Example Export.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Report and Dashboard Templates.zip` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Report and Dashboard Templates.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Tutorial.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Version Considerations.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Version Considerations.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Workbook Templates.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Workbook Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/Workbook Templates.zip` & `seeq-spy-187.0/seeq/spy/docs/Documentation/Workbook Templates.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/better_metadata.pickle` & `seeq-spy-187.0/seeq/spy/docs/Documentation/better_metadata.pickle`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/company_logo.png` & `seeq-spy-187.0/seeq/spy/docs/Documentation/company_logo.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/csv_import_example.csv` & `seeq-spy-187.0/seeq/spy/docs/Documentation/csv_import_example.csv`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/spy.acl.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/spy.acl.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/spy.jobs.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/spy.jobs.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/spy.login.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/spy.login.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/spy.pull.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/spy.pull.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998521292575001%*

 * *Differences: {"'cells'": "{0: {'source': ['import pandas as pd\\n', '\\n', 'from seeq import spy']}, 9: "*

 * *            '{\'metadata\': {replace: OrderedDict()}}, 21: {\'source\': {insert: [(2, "    '*

 * *            '\'Type\': \'Condition\',\\n"), (11, "    \'Formula\': '*

 * *            '\'$cp.valueSearch(isGreaterThan(25kW))\'\\n")], delete: [11, 2]}}, 30: {\'source\': '*

 * *            "{insert: [(0, 'compressor_signal_and_condition = pd.concat([spy.search({\\n'), (4, "*

 * *            '\'}), spy.search({\\n\'), (6, "}, workbook=\'SP […]*

```diff
@@ -2,16 +2,17 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from seeq import spy\n",
-                "import pandas as pd"
+                "import pandas as pd\n",
+                "\n",
+                "from seeq import spy"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
@@ -466,19 +467,15 @@
                 "         start=pd.Timestamp('2019-01-01', tz='US/Pacific'),\n",
                 "         end=pd.Timestamp('2019-01-07', tz='US/Pacific'),\n",
                 "         tz_convert='US/Eastern')"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
-            },
+            "metadata": {},
             "source": [
                 "If you are pulling items from an Analysis worksheet URL, `start` and `end` are selected  by default from the start \n",
                 "and end of the Display Range in the Trend view of the worksheet. \n",
                 "\n",
                 "`worksheet_url = 'http://localhost:34216/workbook/<workbookID>/worksheet/<worksheetID>'`\n",
                 "\n",
                 "`spy.pull(url)`\n",
@@ -1100,24 +1097,24 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "compressor_on_high = spy.push(metadata=pd.DataFrame([{\n",
                 "    'Name': 'Compressor on High',\n",
-                "    'Type': 'Condition',    \n",
+                "    'Type': 'Condition',\n",
                 "\n",
                 "    'Formula Parameters': {\n",
                 "        # Note here that we are just using a row from our search results. The SPy module will figure\n",
                 "        # out that it contains an identifier that we can use.\n",
                 "        '$cp': items[items['Name'] == 'Compressor Power']\n",
                 "    },\n",
                 "\n",
                 "    # This formula specifies capsules to be created when Compressor Power is above 25 kW\n",
-                "    'Formula': '$cp.valueSearch(isGreaterThan(25kW))'    \n",
+                "    'Formula': '$cp.valueSearch(isGreaterThan(25kW))'\n",
                 "}]), workbook='SPy Documentation Examples >> spy.pull')\n",
                 "\n",
                 "compressor_on_high"
             ]
         },
         {
             "cell_type": "markdown",
@@ -1716,21 +1713,21 @@
                     },
                     "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "compressor_signal_and_condition = spy.search({\n",
+                "compressor_signal_and_condition = pd.concat([spy.search({\n",
                 "    'Path': 'Example >> Cooling Tower 1 >> Area A',\n",
                 "    'Name': 'Compressor Power',\n",
                 "    'Datasource Name': 'Example Data'\n",
-                "}).append(spy.search({\n",
+                "}), spy.search({\n",
                 "    'Name': 'Compressor*High',\n",
-                "}, workbook='SPy Documentation Examples >> spy.pull'), sort=False, ignore_index=True)\n",
+                "}, workbook='SPy Documentation Examples >> spy.pull')], sort=False, ignore_index=True)\n",
                 "\n",
                 "spy.pull(compressor_signal_and_condition,\n",
                 "         start='2019-01-01T00:00:00Z', end='2019-01-01T12:00:00Z',\n",
                 "         header='Name', grid='1h')"
             ]
         },
         {
@@ -2116,16 +2113,16 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "compressor_power_limit = spy.push(metadata=pd.DataFrame([{\n",
                 "    'Name': 'Compressor Power Limit',\n",
-                "    'Type': 'Scalar',    \n",
-                "    'Formula': '50kW'    \n",
+                "    'Type': 'Scalar',\n",
+                "    'Formula': '50kW'\n",
                 "}]), workbook='SPy Documentation Examples >> spy.pull', errors='raise')\n",
                 "\n",
                 "compressor_power_limit"
             ]
         },
         {
             "cell_type": "code",
@@ -2322,19 +2319,15 @@
             ],
             "source": [
                 "unpickled_pull.spy.status.df"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
-            },
+            "metadata": {},
             "source": [
                 "## Detailed Help\n",
                 "\n",
                 "All SPy functions have detailed documentation to help you use them. Just execute `help(spy.<func>)` like\n",
                 "you see below.\n",
                 "\n",
                 "**Make sure you re-execute the cell below to see the latest documentation. It otherwise might be from an\n",
```

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/spy.push.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/spy.push.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/spy.search.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/spy.search.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/spy.widgets.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/spy.widgets.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/Documentation/spy.workbooks.ipynb` & `seeq-spy-187.0/seeq/spy/docs/Documentation/spy.workbooks.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/docs/_copy.py` & `seeq-spy-187.0/seeq/spy/docs/_copy.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/jobs/_execute.py` & `seeq-spy-187.0/seeq/spy/jobs/_execute.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/jobs/_pull.py` & `seeq-spy-187.0/seeq/spy/jobs/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/jobs/_push.py` & `seeq-spy-187.0/seeq/spy/jobs/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/jobs/_schedule.py` & `seeq-spy-187.0/seeq/spy/jobs/_schedule.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/notifications/_emails.py` & `seeq-spy-187.0/seeq/spy/notifications/_emails.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/utils/__init__.py` & `seeq-spy-187.0/seeq/spy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/widgets/_ipy_utils.py` & `seeq-spy-187.0/seeq/spy/widgets/_ipy_utils.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/widgets/_widgets.py` & `seeq-spy-187.0/seeq/spy/widgets/_widgets.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/__init__.py` & `seeq-spy-187.0/seeq/spy/workbooks/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_annotation.py` & `seeq-spy-187.0/seeq/spy/workbooks/_annotation.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_content.py` & `seeq-spy-187.0/seeq/spy/workbooks/_content.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_data.py` & `seeq-spy-187.0/seeq/spy/workbooks/_data.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_folder.py` & `seeq-spy-187.0/seeq/spy/workbooks/_folder.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_item.py` & `seeq-spy-187.0/seeq/spy/workbooks/_item.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_item_map.py` & `seeq-spy-187.0/seeq/spy/workbooks/_item_map.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_load.py` & `seeq-spy-187.0/seeq/spy/workbooks/_load.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_mustache.py` & `seeq-spy-187.0/seeq/spy/workbooks/_mustache.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_pull.py` & `seeq-spy-187.0/seeq/spy/workbooks/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_push.py` & `seeq-spy-187.0/seeq/spy/workbooks/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_render.py` & `seeq-spy-187.0/seeq/spy/workbooks/_render.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_save.py` & `seeq-spy-187.0/seeq/spy/workbooks/_save.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_search.py` & `seeq-spy-187.0/seeq/spy/workbooks/_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
                     _item: ItemOutputV1 = items_api.get_item_and_all_properties(id=content.id)
                     for prop in _item.properties:  # type: PropertyOutputV1
                         if prop.name not in excluded_properties:
                             content_dict[prop.name] = _common.none_to_nan(prop.value)
 
                 _request_workbook_properties()
 
-            results_df = results_df.append(content_dict, ignore_index=True, sort=True)
+            results_df = pd.concat([results_df, pd.DataFrame([content_dict])], ignore_index=True, sort=True)
 
         if content.type == 'Folder' and ((recursive and len(path_filter_parts) == 0) or path_matches):
             child_path_filter = None
             if path_filter_parts and len(path_filter_parts) > 1:
                 child_path_filter = _common.path_list_to_string(path_filter_parts[1:])
 
             if len(parent_path) == 0:
@@ -309,15 +309,15 @@
                 child_query['Path'] = child_path_filter
 
             child_results_df = _search(session, child_query, status, content_filter=content_filter,
                                        all_properties=all_properties, recursive=recursive,
                                        include_archived=include_archived, parent_id=content.id,
                                        parent_path=new_parent_path, search_folder_id=search_folder_id)
 
-            results_df = results_df.append(child_results_df, ignore_index=True, sort=True)
+            results_df = pd.concat([results_df, child_results_df], ignore_index=True, sort=True)
 
     return results_df
 
 
 def get_folders(session: Session, content_filter='ALL', folder_id=None, archived=False, sort_order='createdAt ASC',
                 only_pinned=False) -> WorkbenchItemOutputListV1:
     folders_api = FoldersApi(session.client)
```

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_template.py` & `seeq-spy-187.0/seeq/spy/workbooks/_template.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_user.py` & `seeq-spy-187.0/seeq/spy/workbooks/_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import List, Optional, Dict, Union
 
 import pandas as pd
+
 from seeq.sdk import *
 from seeq.spy import _common, _metadata
 from seeq.spy._errors import *
 from seeq.spy._redaction import request_safely, safely
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 from seeq.spy.workbooks._data import StoredItem
@@ -130,20 +131,20 @@
                 identity_id = Identity.find_identity(session, acl_to_push['Identity'], datasource_maps, item_map)
             except SPyDependencyNotFound:
                 if strict:
                     raise
 
                 continue
 
-            acl_df = acl_df.append({
+            acl_df = pd.concat([acl_df, pd.DataFrame([{
                 'ID': identity_id,
                 'Read': acl_to_push['Permissions']['Read'],
                 'Write': acl_to_push['Permissions']['Write'],
                 'Manage': acl_to_push['Permissions']['Manage']
-            }, ignore_index=True)
+            }])], ignore_index=True)
 
         _metadata.push_access_control(session, pushed_id, acl_df, replace)
 
     @staticmethod
     def _dict_to_permissions(d):
         return PermissionsV1(
             manage=_common.get(d, 'Manage', False),
```

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_workbook.py` & `seeq-spy-187.0/seeq/spy/workbooks/_workbook.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_worksheet.py` & `seeq-spy-187.0/seeq/spy/workbooks/_worksheet.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/_workstep.py` & `seeq-spy-187.0/seeq/spy/workbooks/_workstep.py`

 * *Files 0% similar despite different names*

```diff
@@ -812,15 +812,15 @@
                                 self._workstep_rightAxis_workstep_to_user[value]
                         else:
                             output_item[self._workstep_display_workstep_to_user[k]] = value
 
                 items.append(output_item)
 
         items_df = pd.DataFrame({'Name': pd.Series([], dtype=str), 'ID': pd.Series([], dtype=str)})
-        items_df = items_df.append(items, ignore_index=True).astype(object)
+        items_df = pd.concat([items_df, pd.DataFrame(items)], ignore_index=True).astype(object)
         return items_df
 
     def _get_scatter_plot_series(self):
         """
         Get the ID of the one of the items plotted on the x or y axis of a scatter plot
 
         :return: dict or none
```

### Comparing `seeq-spy-186.9/seeq/spy/workbooks/app.css` & `seeq-spy-187.0/seeq/spy/workbooks/app.css`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/seeq_spy.egg-info/PKG-INFO` & `seeq-spy-187.0/seeq_spy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 186.9
+Version: 187.0
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seeq-spy-186.9/seeq_spy.egg-info/SOURCES.txt` & `seeq-spy-187.0/seeq_spy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seeq-spy-186.9/setup.py` & `seeq-spy-187.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seeq-spy",
-    version="186.9",
+    version="187.0",
     author="Seeq Corporation",
     author_email="support@seeq.com",
     description="Easy-to-use Python interface for Seeq",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.seeq.com",
     project_urls={
```

