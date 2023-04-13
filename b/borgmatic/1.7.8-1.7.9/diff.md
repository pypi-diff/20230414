# Comparing `tmp/borgmatic-1.7.8.tar.gz` & `tmp/borgmatic-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "borgmatic-1.7.8.tar", last modified: Thu Mar  2 23:41:08 2023, max compression
+gzip compressed data, was "borgmatic-1.7.9.tar", last modified: Thu Mar 16 20:46:45 2023, max compression
```

## Comparing `borgmatic-1.7.8.tar` & `borgmatic-1.7.9.tar`

### file list

```diff
@@ -1,284 +1,288 @@
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.808290 borgmatic-1.7.8/
--rw-r--r--   0 witten    (1000) witten    (1000)       10 2021-06-08 17:56:15.000000 borgmatic-1.7.8/.dockerignore
--rw-r--r--   0 witten    (1000) witten    (1000)     1023 2022-08-02 04:17:26.000000 borgmatic-1.7.8/.drone.yml
--rw-r--r--   0 witten    (1000) witten    (1000)     1461 2023-01-27 00:18:02.000000 borgmatic-1.7.8/.eleventy.js
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.751621 borgmatic-1.7.8/.gitea/
--rw-r--r--   0 witten    (1000) witten    (1000)      808 2021-06-08 17:56:15.000000 borgmatic-1.7.8/.gitea/issue_template.md
--rw-r--r--   0 witten    (1000) witten    (1000)      105 2022-03-05 23:40:50.000000 borgmatic-1.7.8/.gitignore
--rw-r--r--   0 witten    (1000) witten    (1000)      631 2021-06-08 17:56:15.000000 borgmatic-1.7.8/AUTHORS
--rw-r--r--   0 witten    (1000) witten    (1000)    35122 2021-06-08 17:56:15.000000 borgmatic-1.7.8/LICENSE
--rw-r--r--   0 witten    (1000) witten    (1000)       58 2021-06-08 17:56:15.000000 borgmatic-1.7.8/MANIFEST.in
--rw-r--r--   0 witten    (1000) witten    (1000)    52845 2023-03-02 23:34:16.000000 borgmatic-1.7.8/NEWS
--rw-r--r--   0 witten    (1000) witten    (1000)      682 2023-03-02 23:41:08.811623 borgmatic-1.7.8/PKG-INFO
--rw-r--r--   0 witten    (1000) witten    (1000)     7044 2023-02-28 17:37:40.000000 borgmatic-1.7.8/README.md
--rw-r--r--   0 witten    (1000) witten    (1000)      665 2022-03-05 23:40:50.000000 borgmatic-1.7.8/SECURITY.md
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.751621 borgmatic-1.7.8/borgmatic/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:15.000000 borgmatic-1.7.8/borgmatic/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.754954 borgmatic-1.7.8/borgmatic/actions/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1058 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/borg.py
--rw-r--r--   0 witten    (1000) witten    (1000)      697 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/break_lock.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1287 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/check.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1613 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/compact.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2422 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/create.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1446 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/export_tar.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1883 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/extract.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1310 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/info.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1404 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/list.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1312 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/mount.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1240 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/prune.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1034 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/rcreate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    12293 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/restore.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1049 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/rinfo.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1013 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/rlist.py
--rw-r--r--   0 witten    (1000) witten    (1000)      626 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/actions/transfer.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.761621 borgmatic-1.7.8/borgmatic/borg/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2022-06-30 18:18:03.000000 borgmatic-1.7.8/borgmatic/borg/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2334 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/borg/borg.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1232 2022-12-12 19:25:31.000000 borgmatic-1.7.8/borgmatic/borg/break_lock.py
--rw-r--r--   0 witten    (1000) witten    (1000)    11327 2023-02-28 20:56:18.000000 borgmatic-1.7.8/borgmatic/borg/check.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1739 2022-08-19 06:07:33.000000 borgmatic-1.7.8/borgmatic/borg/compact.py
--rw-r--r--   0 witten    (1000) witten    (1000)    19042 2023-03-02 23:23:00.000000 borgmatic-1.7.8/borgmatic/borg/create.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1346 2022-06-30 18:00:59.000000 borgmatic-1.7.8/borgmatic/borg/environment.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2583 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/borg/export_tar.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4864 2022-12-02 18:12:38.000000 borgmatic-1.7.8/borgmatic/borg/extract.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1468 2023-03-02 18:53:58.000000 borgmatic-1.7.8/borgmatic/borg/feature.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1793 2022-08-19 06:07:33.000000 borgmatic-1.7.8/borgmatic/borg/flags.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2421 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/borg/info.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7963 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/borg/list.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2551 2022-12-12 19:25:31.000000 borgmatic-1.7.8/borgmatic/borg/mount.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2905 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/borg/prune.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2849 2022-08-19 06:07:33.000000 borgmatic-1.7.8/borgmatic/borg/rcreate.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1887 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/borg/rinfo.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4278 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/borg/rlist.py
--rw-r--r--   0 witten    (1000) witten    (1000)       52 2022-06-30 18:22:30.000000 borgmatic-1.7.8/borgmatic/borg/state.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1852 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/borg/transfer.py
--rw-r--r--   0 witten    (1000) witten    (1000)      576 2022-08-16 03:08:11.000000 borgmatic-1.7.8/borgmatic/borg/umount.py
--rw-r--r--   0 witten    (1000) witten    (1000)      971 2022-12-12 19:25:31.000000 borgmatic-1.7.8/borgmatic/borg/version.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.764955 borgmatic-1.7.8/borgmatic/commands/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:15.000000 borgmatic-1.7.8/borgmatic/commands/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)    33661 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/commands/arguments.py
--rw-r--r--   0 witten    (1000) witten    (1000)    25119 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/commands/borgmatic.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2082 2022-06-09 23:26:49.000000 borgmatic-1.7.8/borgmatic/commands/completion.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3421 2021-12-06 19:57:31.000000 borgmatic-1.7.8/borgmatic/commands/convert_config.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2388 2022-08-24 16:53:36.000000 borgmatic-1.7.8/borgmatic/commands/generate_config.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1705 2021-06-08 17:56:16.000000 borgmatic-1.7.8/borgmatic/commands/validate_config.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.768288 borgmatic-1.7.8/borgmatic/config/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.8/borgmatic/config/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)      349 2021-06-08 17:56:16.000000 borgmatic-1.7.8/borgmatic/config/checks.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2147 2021-12-06 19:54:03.000000 borgmatic-1.7.8/borgmatic/config/collect.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3805 2022-03-05 23:40:50.000000 borgmatic-1.7.8/borgmatic/config/convert.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1557 2022-10-03 18:27:04.000000 borgmatic-1.7.8/borgmatic/config/environment.py
--rw-r--r--   0 witten    (1000) witten    (1000)    11020 2022-08-19 06:07:33.000000 borgmatic-1.7.8/borgmatic/config/generate.py
--rw-r--r--   0 witten    (1000) witten    (1000)     5432 2021-06-08 17:56:16.000000 borgmatic-1.7.8/borgmatic/config/legacy.py
--rw-r--r--   0 witten    (1000) witten    (1000)     9063 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/config/load.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3707 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/config/normalize.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2401 2022-12-12 19:25:31.000000 borgmatic-1.7.8/borgmatic/config/override.py
--rw-r--r--   0 witten    (1000) witten    (1000)    60300 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/config/schema.yaml
--rw-r--r--   0 witten    (1000) witten    (1000)     6713 2022-10-03 18:36:05.000000 borgmatic-1.7.8/borgmatic/config/validate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    12717 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/execute.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.771622 borgmatic-1.7.8/borgmatic/hooks/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.8/borgmatic/hooks/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3412 2022-08-21 21:51:50.000000 borgmatic-1.7.8/borgmatic/hooks/command.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1752 2022-06-30 04:02:27.000000 borgmatic-1.7.8/borgmatic/hooks/cronhub.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1633 2022-06-30 03:51:46.000000 borgmatic-1.7.8/borgmatic/hooks/cronitor.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3182 2022-12-12 19:25:31.000000 borgmatic-1.7.8/borgmatic/hooks/dispatch.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2390 2023-01-26 07:02:04.000000 borgmatic-1.7.8/borgmatic/hooks/dump.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4877 2022-07-24 06:12:14.000000 borgmatic-1.7.8/borgmatic/hooks/healthchecks.py
--rw-r--r--   0 witten    (1000) witten    (1000)     6796 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/hooks/mongodb.py
--rw-r--r--   0 witten    (1000) witten    (1000)      168 2022-06-09 20:26:20.000000 borgmatic-1.7.8/borgmatic/hooks/monitor.py
--rw-r--r--   0 witten    (1000) witten    (1000)     9087 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/hooks/mysql.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2987 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/hooks/ntfy.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2649 2022-06-30 03:50:56.000000 borgmatic-1.7.8/borgmatic/hooks/pagerduty.py
--rw-r--r--   0 witten    (1000) witten    (1000)    10603 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/hooks/postgresql.py
--rw-r--r--   0 witten    (1000) witten    (1000)     6838 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/logger.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1048 2022-04-28 23:35:37.000000 borgmatic-1.7.8/borgmatic/signals.py
--rw-r--r--   0 witten    (1000) witten    (1000)      516 2023-02-28 17:37:40.000000 borgmatic-1.7.8/borgmatic/verbosity.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.751621 borgmatic-1.7.8/borgmatic.egg-info/
--rw-r--r--   0 witten    (1000) witten    (1000)      682 2023-03-02 23:41:08.000000 borgmatic-1.7.8/borgmatic.egg-info/PKG-INFO
--rw-r--r--   0 witten    (1000) witten    (1000)     7486 2023-03-02 23:41:08.000000 borgmatic-1.7.8/borgmatic.egg-info/SOURCES.txt
--rw-r--r--   0 witten    (1000) witten    (1000)        1 2023-03-02 23:41:08.000000 borgmatic-1.7.8/borgmatic.egg-info/dependency_links.txt
--rw-r--r--   0 witten    (1000) witten    (1000)      266 2023-03-02 23:41:08.000000 borgmatic-1.7.8/borgmatic.egg-info/entry_points.txt
--rw-r--r--   0 witten    (1000) witten    (1000)       79 2023-03-02 23:41:08.000000 borgmatic-1.7.8/borgmatic.egg-info/requires.txt
--rw-r--r--   0 witten    (1000) witten    (1000)       10 2023-03-02 23:41:08.000000 borgmatic-1.7.8/borgmatic.egg-info/top_level.txt
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.771622 borgmatic-1.7.8/docs/
--rw-r--r--   0 witten    (1000) witten    (1000)     1417 2023-02-28 17:37:40.000000 borgmatic-1.7.8/docs/Dockerfile
--rw-r--r--   0 witten    (1000) witten    (1000)     7044 2023-02-28 17:37:40.000000 borgmatic-1.7.8/docs/README.md
--rw-r--r--   0 witten    (1000) witten    (1000)      673 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/SECURITY.md
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.771622 borgmatic-1.7.8/docs/_data/
--rw-r--r--   0 witten    (1000) witten    (1000)       19 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/_data/layout.json
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.771622 borgmatic-1.7.8/docs/_includes/
--rw-r--r--   0 witten    (1000) witten    (1000)       52 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/_includes/asciinema.css
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.774955 borgmatic-1.7.8/docs/_includes/components/
--rw-r--r--   0 witten    (1000) witten    (1000)      492 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/_includes/components/external-links.css
--rw-r--r--   0 witten    (1000) witten    (1000)      636 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/_includes/components/info-blocks.css
--rw-r--r--   0 witten    (1000) witten    (1000)     5765 2021-12-06 19:54:03.000000 borgmatic-1.7.8/docs/_includes/components/lists.css
--rw-r--r--   0 witten    (1000) witten    (1000)     2242 2021-12-06 19:54:03.000000 borgmatic-1.7.8/docs/_includes/components/minilink.css
--rw-r--r--   0 witten    (1000) witten    (1000)      230 2022-03-05 23:40:50.000000 borgmatic-1.7.8/docs/_includes/components/suggestion-link.html
--rw-r--r--   0 witten    (1000) witten    (1000)     2088 2021-12-06 19:54:03.000000 borgmatic-1.7.8/docs/_includes/components/toc.css
--rw-r--r--   0 witten    (1000) witten    (1000)      265 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/_includes/header.njk
--rw-r--r--   0 witten    (1000) witten    (1000)    25868 2022-08-22 04:47:27.000000 borgmatic-1.7.8/docs/_includes/index.css
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.774955 borgmatic-1.7.8/docs/_includes/layouts/
--rw-r--r--   0 witten    (1000) witten    (1000)      813 2022-03-05 23:40:50.000000 borgmatic-1.7.8/docs/_includes/layouts/base.njk
--rw-r--r--   0 witten    (1000) witten    (1000)     1091 2022-03-05 23:40:50.000000 borgmatic-1.7.8/docs/_includes/layouts/main.njk
--rw-r--r--   0 witten    (1000) witten    (1000)     3039 2021-12-06 19:54:03.000000 borgmatic-1.7.8/docs/_includes/prism-theme.css
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.778289 borgmatic-1.7.8/docs/how-to/
--rw-r--r--   0 witten    (1000) witten    (1000)     4522 2022-08-22 03:42:17.000000 borgmatic-1.7.8/docs/how-to/add-preparation-and-cleanup-steps-to-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     5082 2023-02-28 17:37:40.000000 borgmatic-1.7.8/docs/how-to/backup-to-a-removable-drive-or-an-intermittent-server.md
--rw-r--r--   0 witten    (1000) witten    (1000)    11823 2023-02-28 17:37:40.000000 borgmatic-1.7.8/docs/how-to/backup-your-databases.md
--rw-r--r--   0 witten    (1000) witten    (1000)     6208 2023-02-28 17:37:40.000000 borgmatic-1.7.8/docs/how-to/deal-with-very-large-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     4667 2022-08-16 22:22:37.000000 borgmatic-1.7.8/docs/how-to/develop-on-borgmatic.md
--rw-r--r--   0 witten    (1000) witten    (1000)     4044 2022-08-19 06:07:33.000000 borgmatic-1.7.8/docs/how-to/extract-a-backup.md
--rw-r--r--   0 witten    (1000) witten    (1000)       66 2021-12-06 19:54:03.000000 borgmatic-1.7.8/docs/how-to/index.md
--rw-r--r--   0 witten    (1000) witten    (1000)     4425 2022-12-12 19:25:31.000000 borgmatic-1.7.8/docs/how-to/inspect-your-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     2057 2023-02-28 17:37:40.000000 borgmatic-1.7.8/docs/how-to/make-backups-redundant.md
--rw-r--r--   0 witten    (1000) witten    (1000)     8860 2023-02-28 17:37:40.000000 borgmatic-1.7.8/docs/how-to/make-per-application-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)    14065 2022-08-21 21:18:50.000000 borgmatic-1.7.8/docs/how-to/monitor-your-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     3110 2022-08-22 04:14:10.000000 borgmatic-1.7.8/docs/how-to/provide-your-passwords.md
--rw-r--r--   0 witten    (1000) witten    (1000)      124 2022-06-16 18:55:15.000000 borgmatic-1.7.8/docs/how-to/restore-a-backup.md
--rw-r--r--   0 witten    (1000) witten    (1000)     3924 2022-12-12 19:25:31.000000 borgmatic-1.7.8/docs/how-to/run-arbitrary-borg-commands.md
--rw-r--r--   0 witten    (1000) witten    (1000)      152 2022-06-16 18:55:21.000000 borgmatic-1.7.8/docs/how-to/run-preparation-steps-before-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)    14869 2023-02-28 17:37:40.000000 borgmatic-1.7.8/docs/how-to/set-up-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     7785 2023-02-28 17:37:40.000000 borgmatic-1.7.8/docs/how-to/upgrade.md
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.781622 borgmatic-1.7.8/docs/reference/
--rw-r--r--   0 witten    (1000) witten    (1000)      331 2023-02-28 17:37:40.000000 borgmatic-1.7.8/docs/reference/command-line.md
--rw-r--r--   0 witten    (1000) witten    (1000)      426 2023-02-28 17:37:40.000000 borgmatic-1.7.8/docs/reference/configuration.md
--rw-r--r--   0 witten    (1000) witten    (1000)       69 2021-12-06 19:54:03.000000 borgmatic-1.7.8/docs/reference/index.md
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.784956 borgmatic-1.7.8/docs/static/
--rw-r--r--   0 witten    (1000) witten    (1000)     5822 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/static/borgbase.png
--rw-r--r--   0 witten    (1000) witten    (1000)     3593 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/static/borgmatic.png
--rw-r--r--   0 witten    (1000) witten    (1000)     1674 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/static/borgmatic.svg
--rw-r--r--   0 witten    (1000) witten    (1000)    23536 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/static/cronhub.png
--rw-r--r--   0 witten    (1000) witten    (1000)    10364 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/static/cronitor.png
--rw-r--r--   0 witten    (1000) witten    (1000)     4556 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/static/healthchecks.png
--rw-r--r--   0 witten    (1000) witten    (1000)     9474 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/static/mariadb.png
--rw-r--r--   0 witten    (1000) witten    (1000)    12839 2022-03-05 23:40:50.000000 borgmatic-1.7.8/docs/static/mongodb.png
--rw-r--r--   0 witten    (1000) witten    (1000)     3761 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/static/mysql.png
--rw-r--r--   0 witten    (1000) witten    (1000)    10266 2022-06-09 20:35:18.000000 borgmatic-1.7.8/docs/static/ntfy.png
--rw-r--r--   0 witten    (1000) witten    (1000)    20107 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/static/pagerduty.png
--rw-r--r--   0 witten    (1000) witten    (1000)    31528 2021-06-08 17:56:16.000000 borgmatic-1.7.8/docs/static/postgresql.png
--rw-r--r--   0 witten    (1000) witten    (1000)       64 2021-06-08 17:56:16.000000 borgmatic-1.7.8/pyproject.toml
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.744954 borgmatic-1.7.8/sample/
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.784956 borgmatic-1.7.8/sample/cron/
--rw-r--r--   0 witten    (1000) witten    (1000)      183 2022-03-05 23:40:50.000000 borgmatic-1.7.8/sample/cron/borgmatic
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.784956 borgmatic-1.7.8/sample/systemd/
--rw-r--r--   0 witten    (1000) witten    (1000)     2612 2022-12-12 19:25:31.000000 borgmatic-1.7.8/sample/systemd/borgmatic.service
--rw-r--r--   0 witten    (1000) witten    (1000)      138 2022-05-08 06:08:53.000000 borgmatic-1.7.8/sample/systemd/borgmatic.timer
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.784956 borgmatic-1.7.8/scripts/
--rwxr-xr-x   0 witten    (1000) witten    (1000)      241 2023-01-27 02:00:56.000000 borgmatic-1.7.8/scripts/dev-docs
--rwxr-xr-x   0 witten    (1000) witten    (1000)     3108 2022-12-12 19:25:31.000000 borgmatic-1.7.8/scripts/find-unsupported-borg-options
--rwxr-xr-x   0 witten    (1000) witten    (1000)      137 2021-06-08 17:56:16.000000 borgmatic-1.7.8/scripts/push
--rwxr-xr-x   0 witten    (1000) witten    (1000)     1843 2023-03-02 23:41:00.000000 borgmatic-1.7.8/scripts/release
--rwxr-xr-x   0 witten    (1000) witten    (1000)      517 2021-06-08 17:56:16.000000 borgmatic-1.7.8/scripts/run-full-dev-tests
--rwxr-xr-x   0 witten    (1000) witten    (1000)      984 2022-08-19 06:07:33.000000 borgmatic-1.7.8/scripts/run-full-tests
--rw-r--r--   0 witten    (1000) witten    (1000)      467 2023-03-02 23:41:08.811623 borgmatic-1.7.8/setup.cfg
--rw-r--r--   0 witten    (1000) witten    (1000)     1372 2023-03-02 23:34:20.000000 borgmatic-1.7.8/setup.py
--rw-r--r--   0 witten    (1000) witten    (1000)      545 2023-02-28 17:37:40.000000 borgmatic-1.7.8/test_requirements.txt
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.784956 borgmatic-1.7.8/tests/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.788289 borgmatic-1.7.8/tests/end-to-end/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/end-to-end/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)      626 2022-03-05 23:40:50.000000 borgmatic-1.7.8/tests/end-to-end/docker-compose.yaml
--rw-r--r--   0 witten    (1000) witten    (1000)     3180 2022-08-22 05:57:33.000000 borgmatic-1.7.8/tests/end-to-end/test_borgmatic.py
--rw-r--r--   0 witten    (1000) witten    (1000)      143 2022-05-26 18:07:14.000000 borgmatic-1.7.8/tests/end-to-end/test_completion.py
--rw-r--r--   0 witten    (1000) witten    (1000)     6188 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/end-to-end/test_database.py
--rw-r--r--   0 witten    (1000) witten    (1000)      588 2022-08-19 06:07:33.000000 borgmatic-1.7.8/tests/end-to-end/test_generate_config.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2006 2022-08-22 06:22:23.000000 borgmatic-1.7.8/tests/end-to-end/test_override.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1227 2022-08-18 03:47:17.000000 borgmatic-1.7.8/tests/end-to-end/test_validate_config.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.788289 borgmatic-1.7.8/tests/integration/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/integration/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.788289 borgmatic-1.7.8/tests/integration/borg/
--rw-r--r--   0 witten    (1000) witten    (1000)      546 2022-03-05 23:40:50.000000 borgmatic-1.7.8/tests/integration/borg/test_feature.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.788289 borgmatic-1.7.8/tests/integration/commands/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/integration/commands/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)    18967 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/integration/commands/test_arguments.py
--rw-r--r--   0 witten    (1000) witten    (1000)      432 2022-08-21 21:13:43.000000 borgmatic-1.7.8/tests/integration/commands/test_borgmatic.py
--rw-r--r--   0 witten    (1000) witten    (1000)      133 2022-05-26 16:53:24.000000 borgmatic-1.7.8/tests/integration/commands/test_completion.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1671 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/integration/commands/test_convert_config.py
--rw-r--r--   0 witten    (1000) witten    (1000)      803 2022-05-29 23:00:10.000000 borgmatic-1.7.8/tests/integration/commands/test_generate_config.py
--rw-r--r--   0 witten    (1000) witten    (1000)      672 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/integration/commands/test_validate_config.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.791622 borgmatic-1.7.8/tests/integration/config/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/integration/config/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7927 2022-06-30 20:10:10.000000 borgmatic-1.7.8/tests/integration/config/test_generate.py
--rw-r--r--   0 witten    (1000) witten    (1000)      578 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/integration/config/test_legacy.py
--rw-r--r--   0 witten    (1000) witten    (1000)    15187 2022-05-20 22:15:07.000000 borgmatic-1.7.8/tests/integration/config/test_load.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1039 2021-11-29 20:38:51.000000 borgmatic-1.7.8/tests/integration/config/test_override.py
--rw-r--r--   0 witten    (1000) witten    (1000)      234 2021-12-06 19:54:03.000000 borgmatic-1.7.8/tests/integration/config/test_schema.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7699 2022-10-03 18:57:54.000000 borgmatic-1.7.8/tests/integration/config/test_validate.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.791622 borgmatic-1.7.8/tests/integration/hooks/
--rw-r--r--   0 witten    (1000) witten    (1000)      729 2021-12-06 19:54:03.000000 borgmatic-1.7.8/tests/integration/hooks/test_healthchecks.py
--rw-r--r--   0 witten    (1000) witten    (1000)    11263 2022-08-28 16:03:46.000000 borgmatic-1.7.8/tests/integration/test_execute.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.791622 borgmatic-1.7.8/tests/unit/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/unit/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.798289 borgmatic-1.7.8/tests/unit/actions/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)      760 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_borg.py
--rw-r--r--   0 witten    (1000) witten    (1000)      636 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_break_lock.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1039 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_check.py
--rw-r--r--   0 witten    (1000) witten    (1000)      999 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_compact.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1204 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_create.py
--rw-r--r--   0 witten    (1000) witten    (1000)      958 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_export_tar.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1104 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_extract.py
--rw-r--r--   0 witten    (1000) witten    (1000)      808 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_info.py
--rw-r--r--   0 witten    (1000) witten    (1000)      799 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_list.py
--rw-r--r--   0 witten    (1000) witten    (1000)      764 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_mount.py
--rw-r--r--   0 witten    (1000) witten    (1000)      849 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_prune.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1730 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_rcreate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    18426 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_restore.py
--rw-r--r--   0 witten    (1000) witten    (1000)      679 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_rinfo.py
--rw-r--r--   0 witten    (1000) witten    (1000)      671 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_rlist.py
--rw-r--r--   0 witten    (1000) witten    (1000)      621 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/actions/test_transfer.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.801623 borgmatic-1.7.8/tests/unit/borg/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/unit/borg/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)    12347 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/borg/test_borg.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2534 2022-12-12 19:25:31.000000 borgmatic-1.7.8/tests/unit/borg/test_break_lock.py
--rw-r--r--   0 witten    (1000) witten    (1000)    25781 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/borg/test_check.py
--rw-r--r--   0 witten    (1000) witten    (1000)     5527 2022-08-19 06:07:33.000000 borgmatic-1.7.8/tests/unit/borg/test_compact.py
--rw-r--r--   0 witten    (1000) witten    (1000)   116577 2023-03-02 23:31:53.000000 borgmatic-1.7.8/tests/unit/borg/test_create.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1174 2022-06-30 19:15:33.000000 borgmatic-1.7.8/tests/unit/borg/test_environment.py
--rw-r--r--   0 witten    (1000) witten    (1000)    10755 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/borg/test_export_tar.py
--rw-r--r--   0 witten    (1000) witten    (1000)    14383 2022-12-12 19:25:31.000000 borgmatic-1.7.8/tests/unit/borg/test_extract.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2846 2022-08-19 06:07:33.000000 borgmatic-1.7.8/tests/unit/borg/test_flags.py
--rw-r--r--   0 witten    (1000) witten    (1000)    13294 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/borg/test_info.py
--rw-r--r--   0 witten    (1000) witten    (1000)    23301 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/borg/test_list.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7359 2022-12-12 19:25:31.000000 borgmatic-1.7.8/tests/unit/borg/test_mount.py
--rw-r--r--   0 witten    (1000) witten    (1000)    10592 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/borg/test_prune.py
--rw-r--r--   0 witten    (1000) witten    (1000)     9791 2022-08-19 16:27:22.000000 borgmatic-1.7.8/tests/unit/borg/test_rcreate.py
--rw-r--r--   0 witten    (1000) witten    (1000)     9342 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/borg/test_rinfo.py
--rw-r--r--   0 witten    (1000) witten    (1000)    14072 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/borg/test_rlist.py
--rw-r--r--   0 witten    (1000) witten    (1000)    14768 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/borg/test_transfer.py
--rw-r--r--   0 witten    (1000) witten    (1000)      920 2022-06-30 19:06:41.000000 borgmatic-1.7.8/tests/unit/borg/test_umount.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2063 2022-12-12 19:25:31.000000 borgmatic-1.7.8/tests/unit/borg/test_version.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.804956 borgmatic-1.7.8/tests/unit/commands/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/unit/commands/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     5027 2022-08-19 00:01:19.000000 borgmatic-1.7.8/tests/unit/commands/test_arguments.py
--rw-r--r--   0 witten    (1000) witten    (1000)    42161 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/commands/test_borgmatic.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.808290 borgmatic-1.7.8/tests/unit/config/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/unit/config/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)      709 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/unit/config/test_checks.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7576 2021-12-06 19:54:03.000000 borgmatic-1.7.8/tests/unit/config/test_collect.py
--rw-r--r--   0 witten    (1000) witten    (1000)     5380 2022-03-05 23:40:50.000000 borgmatic-1.7.8/tests/unit/config/test_convert.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2880 2022-06-23 17:40:47.000000 borgmatic-1.7.8/tests/unit/config/test_environment.py
--rw-r--r--   0 witten    (1000) witten    (1000)     5549 2022-03-05 23:40:50.000000 borgmatic-1.7.8/tests/unit/config/test_generate.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7470 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/unit/config/test_legacy.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3381 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/config/test_normalize.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2827 2022-03-05 23:40:50.000000 borgmatic-1.7.8/tests/unit/config/test_override.py
--rw-r--r--   0 witten    (1000) witten    (1000)     6214 2022-08-17 16:56:29.000000 borgmatic-1.7.8/tests/unit/config/test_validate.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-02 23:41:08.808290 borgmatic-1.7.8/tests/unit/hooks/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.8/tests/unit/hooks/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4092 2022-05-23 22:26:48.000000 borgmatic-1.7.8/tests/unit/hooks/test_command.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3218 2022-06-30 04:04:43.000000 borgmatic-1.7.8/tests/unit/hooks/test_cronhub.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2666 2022-06-30 04:07:59.000000 borgmatic-1.7.8/tests/unit/hooks/test_cronitor.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4402 2022-12-12 19:25:31.000000 borgmatic-1.7.8/tests/unit/hooks/test_dispatch.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2938 2021-12-06 19:54:03.000000 borgmatic-1.7.8/tests/unit/hooks/test_dump.py
--rw-r--r--   0 witten    (1000) witten    (1000)    11007 2022-07-24 06:12:14.000000 borgmatic-1.7.8/tests/unit/hooks/test_healthchecks.py
--rw-r--r--   0 witten    (1000) witten    (1000)    11590 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/hooks/test_mongodb.py
--rw-r--r--   0 witten    (1000) witten    (1000)    15616 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/hooks/test_mysql.py
--rw-r--r--   0 witten    (1000) witten    (1000)     6825 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/hooks/test_ntfy.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2231 2022-06-30 04:15:15.000000 borgmatic-1.7.8/tests/unit/hooks/test_pagerduty.py
--rw-r--r--   0 witten    (1000) witten    (1000)    26214 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/hooks/test_postgresql.py
--rw-r--r--   0 witten    (1000) witten    (1000)    16090 2022-12-12 19:25:31.000000 borgmatic-1.7.8/tests/unit/test_execute.py
--rw-r--r--   0 witten    (1000) witten    (1000)    13531 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/test_logger.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1405 2022-04-28 23:35:37.000000 borgmatic-1.7.8/tests/unit/test_signals.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1265 2023-02-28 17:37:40.000000 borgmatic-1.7.8/tests/unit/test_verbosity.py
--rw-r--r--   0 witten    (1000) witten    (1000)      699 2022-08-28 16:03:30.000000 borgmatic-1.7.8/tox.ini
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.573053 borgmatic-1.7.9/
+-rw-r--r--   0 witten    (1000) witten    (1000)       10 2021-06-08 17:56:15.000000 borgmatic-1.7.9/.dockerignore
+-rw-r--r--   0 witten    (1000) witten    (1000)     1023 2023-03-16 20:28:40.000000 borgmatic-1.7.9/.drone.yml
+-rw-r--r--   0 witten    (1000) witten    (1000)     1461 2023-01-27 00:18:02.000000 borgmatic-1.7.9/.eleventy.js
+-rw-r--r--   0 witten    (1000) witten    (1000)       12 2023-03-07 22:01:46.000000 borgmatic-1.7.9/.flake8
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.543052 borgmatic-1.7.9/.gitea/
+-rw-r--r--   0 witten    (1000) witten    (1000)      808 2021-06-08 17:56:15.000000 borgmatic-1.7.9/.gitea/issue_template.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      105 2022-03-05 23:40:50.000000 borgmatic-1.7.9/.gitignore
+-rw-r--r--   0 witten    (1000) witten    (1000)      631 2021-06-08 17:56:15.000000 borgmatic-1.7.9/AUTHORS
+-rw-r--r--   0 witten    (1000) witten    (1000)    35122 2021-06-08 17:56:15.000000 borgmatic-1.7.9/LICENSE
+-rw-r--r--   0 witten    (1000) witten    (1000)       58 2021-06-08 17:56:15.000000 borgmatic-1.7.9/MANIFEST.in
+-rw-r--r--   0 witten    (1000) witten    (1000)    53738 2023-03-16 20:42:05.000000 borgmatic-1.7.9/NEWS
+-rw-r--r--   0 witten    (1000) witten    (1000)      682 2023-03-16 20:46:45.573053 borgmatic-1.7.9/PKG-INFO
+-rw-r--r--   0 witten    (1000) witten    (1000)     7227 2023-03-16 20:24:06.000000 borgmatic-1.7.9/README.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      665 2022-03-05 23:40:50.000000 borgmatic-1.7.9/SECURITY.md
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.543052 borgmatic-1.7.9/borgmatic/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:15.000000 borgmatic-1.7.9/borgmatic/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.546386 borgmatic-1.7.9/borgmatic/actions/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/actions/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1058 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/actions/borg.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      697 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/actions/break_lock.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1478 2023-03-16 20:24:06.000000 borgmatic-1.7.9/borgmatic/actions/check.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1808 2023-03-16 20:24:06.000000 borgmatic-1.7.9/borgmatic/actions/compact.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2615 2023-03-16 20:24:06.000000 borgmatic-1.7.9/borgmatic/actions/create.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1446 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/actions/export_tar.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1883 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/actions/extract.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1310 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/actions/info.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1404 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/actions/list.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1312 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/actions/mount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1431 2023-03-16 20:24:06.000000 borgmatic-1.7.9/borgmatic/actions/prune.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1034 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/actions/rcreate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    12293 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/actions/restore.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1049 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/actions/rinfo.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1013 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/actions/rlist.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      626 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/actions/transfer.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.546386 borgmatic-1.7.9/borgmatic/borg/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2022-06-30 18:18:03.000000 borgmatic-1.7.9/borgmatic/borg/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2334 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/borg/borg.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1232 2022-12-12 19:25:31.000000 borgmatic-1.7.9/borgmatic/borg/break_lock.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    11327 2023-03-07 22:07:02.000000 borgmatic-1.7.9/borgmatic/borg/check.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1739 2022-08-19 06:07:33.000000 borgmatic-1.7.9/borgmatic/borg/compact.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    19042 2023-03-02 23:23:00.000000 borgmatic-1.7.9/borgmatic/borg/create.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1346 2022-06-30 18:00:59.000000 borgmatic-1.7.9/borgmatic/borg/environment.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2583 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/borg/export_tar.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     5197 2023-03-09 18:07:20.000000 borgmatic-1.7.9/borgmatic/borg/extract.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1468 2023-03-02 18:53:58.000000 borgmatic-1.7.9/borgmatic/borg/feature.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1793 2022-08-19 06:07:33.000000 borgmatic-1.7.9/borgmatic/borg/flags.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2421 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/borg/info.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7963 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/borg/list.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2551 2022-12-12 19:25:31.000000 borgmatic-1.7.9/borgmatic/borg/mount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2905 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/borg/prune.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2849 2022-08-19 06:07:33.000000 borgmatic-1.7.9/borgmatic/borg/rcreate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1887 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/borg/rinfo.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4278 2023-03-07 22:07:16.000000 borgmatic-1.7.9/borgmatic/borg/rlist.py
+-rw-r--r--   0 witten    (1000) witten    (1000)       52 2022-06-30 18:22:30.000000 borgmatic-1.7.9/borgmatic/borg/state.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1852 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/borg/transfer.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      576 2022-08-16 03:08:11.000000 borgmatic-1.7.9/borgmatic/borg/umount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      971 2022-12-12 19:25:31.000000 borgmatic-1.7.9/borgmatic/borg/version.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.546386 borgmatic-1.7.9/borgmatic/commands/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:15.000000 borgmatic-1.7.9/borgmatic/commands/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    34430 2023-03-16 20:24:06.000000 borgmatic-1.7.9/borgmatic/commands/arguments.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    26598 2023-03-08 21:47:48.000000 borgmatic-1.7.9/borgmatic/commands/borgmatic.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2082 2022-06-09 23:26:49.000000 borgmatic-1.7.9/borgmatic/commands/completion.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3421 2021-12-06 19:57:31.000000 borgmatic-1.7.9/borgmatic/commands/convert_config.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2388 2022-08-24 16:53:36.000000 borgmatic-1.7.9/borgmatic/commands/generate_config.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1705 2021-06-08 17:56:16.000000 borgmatic-1.7.9/borgmatic/commands/validate_config.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.549719 borgmatic-1.7.9/borgmatic/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.9/borgmatic/config/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      349 2021-06-08 17:56:16.000000 borgmatic-1.7.9/borgmatic/config/checks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2147 2021-12-06 19:54:03.000000 borgmatic-1.7.9/borgmatic/config/collect.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3805 2022-03-05 23:40:50.000000 borgmatic-1.7.9/borgmatic/config/convert.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1557 2022-10-03 18:27:04.000000 borgmatic-1.7.9/borgmatic/config/environment.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    11020 2022-08-19 06:07:33.000000 borgmatic-1.7.9/borgmatic/config/generate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     5432 2021-06-08 17:56:16.000000 borgmatic-1.7.9/borgmatic/config/legacy.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     9063 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/config/load.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3707 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/config/normalize.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2401 2022-12-12 19:25:31.000000 borgmatic-1.7.9/borgmatic/config/override.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    61715 2023-03-08 21:49:46.000000 borgmatic-1.7.9/borgmatic/config/schema.yaml
+-rw-r--r--   0 witten    (1000) witten    (1000)     6712 2023-03-07 22:04:39.000000 borgmatic-1.7.9/borgmatic/config/validate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    12717 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/execute.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.549719 borgmatic-1.7.9/borgmatic/hooks/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.9/borgmatic/hooks/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3412 2022-08-21 21:51:50.000000 borgmatic-1.7.9/borgmatic/hooks/command.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1949 2023-03-07 22:22:17.000000 borgmatic-1.7.9/borgmatic/hooks/cronhub.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1832 2023-03-07 22:22:17.000000 borgmatic-1.7.9/borgmatic/hooks/cronitor.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3226 2023-03-04 17:47:51.000000 borgmatic-1.7.9/borgmatic/hooks/dispatch.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2429 2023-03-04 17:47:51.000000 borgmatic-1.7.9/borgmatic/hooks/dump.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4926 2023-03-07 22:22:17.000000 borgmatic-1.7.9/borgmatic/hooks/healthchecks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     6796 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/hooks/mongodb.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      180 2023-03-07 22:22:17.000000 borgmatic-1.7.9/borgmatic/hooks/monitor.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     9087 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/hooks/mysql.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2828 2023-03-07 23:34:13.000000 borgmatic-1.7.9/borgmatic/hooks/ntfy.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2649 2022-06-30 03:50:56.000000 borgmatic-1.7.9/borgmatic/hooks/pagerduty.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    10603 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/hooks/postgresql.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4780 2023-03-04 17:48:09.000000 borgmatic-1.7.9/borgmatic/hooks/sqlite.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     6838 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/logger.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1048 2022-04-28 23:35:37.000000 borgmatic-1.7.9/borgmatic/signals.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      516 2023-02-28 17:37:40.000000 borgmatic-1.7.9/borgmatic/verbosity.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.543052 borgmatic-1.7.9/borgmatic.egg-info/
+-rw-r--r--   0 witten    (1000) witten    (1000)      682 2023-03-16 20:46:45.000000 borgmatic-1.7.9/borgmatic.egg-info/PKG-INFO
+-rw-r--r--   0 witten    (1000) witten    (1000)     7575 2023-03-16 20:46:45.000000 borgmatic-1.7.9/borgmatic.egg-info/SOURCES.txt
+-rw-r--r--   0 witten    (1000) witten    (1000)        1 2023-03-16 20:46:45.000000 borgmatic-1.7.9/borgmatic.egg-info/dependency_links.txt
+-rw-r--r--   0 witten    (1000) witten    (1000)      266 2023-03-16 20:46:45.000000 borgmatic-1.7.9/borgmatic.egg-info/entry_points.txt
+-rw-r--r--   0 witten    (1000) witten    (1000)       79 2023-03-16 20:46:45.000000 borgmatic-1.7.9/borgmatic.egg-info/requires.txt
+-rw-r--r--   0 witten    (1000) witten    (1000)       10 2023-03-16 20:46:45.000000 borgmatic-1.7.9/borgmatic.egg-info/top_level.txt
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.553053 borgmatic-1.7.9/docs/
+-rw-r--r--   0 witten    (1000) witten    (1000)     1417 2023-03-08 22:11:32.000000 borgmatic-1.7.9/docs/Dockerfile
+-rw-r--r--   0 witten    (1000) witten    (1000)     7227 2023-03-16 20:24:06.000000 borgmatic-1.7.9/docs/README.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      673 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/SECURITY.md
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.553053 borgmatic-1.7.9/docs/_data/
+-rw-r--r--   0 witten    (1000) witten    (1000)       19 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/_data/layout.json
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.553053 borgmatic-1.7.9/docs/_includes/
+-rw-r--r--   0 witten    (1000) witten    (1000)       52 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/_includes/asciinema.css
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.553053 borgmatic-1.7.9/docs/_includes/components/
+-rw-r--r--   0 witten    (1000) witten    (1000)      492 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/_includes/components/external-links.css
+-rw-r--r--   0 witten    (1000) witten    (1000)      636 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/_includes/components/info-blocks.css
+-rw-r--r--   0 witten    (1000) witten    (1000)     5125 2023-03-05 00:18:28.000000 borgmatic-1.7.9/docs/_includes/components/lists.css
+-rw-r--r--   0 witten    (1000) witten    (1000)     1788 2023-03-05 00:18:28.000000 borgmatic-1.7.9/docs/_includes/components/minilink.css
+-rw-r--r--   0 witten    (1000) witten    (1000)      230 2022-03-05 23:40:50.000000 borgmatic-1.7.9/docs/_includes/components/suggestion-link.html
+-rw-r--r--   0 witten    (1000) witten    (1000)     1861 2023-03-05 00:18:28.000000 borgmatic-1.7.9/docs/_includes/components/toc.css
+-rw-r--r--   0 witten    (1000) witten    (1000)      265 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/_includes/header.njk
+-rw-r--r--   0 witten    (1000) witten    (1000)    25783 2023-03-05 00:18:28.000000 borgmatic-1.7.9/docs/_includes/index.css
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.553053 borgmatic-1.7.9/docs/_includes/layouts/
+-rw-r--r--   0 witten    (1000) witten    (1000)      813 2022-03-05 23:40:50.000000 borgmatic-1.7.9/docs/_includes/layouts/base.njk
+-rw-r--r--   0 witten    (1000) witten    (1000)     1091 2022-03-05 23:40:50.000000 borgmatic-1.7.9/docs/_includes/layouts/main.njk
+-rw-r--r--   0 witten    (1000) witten    (1000)     3039 2021-12-06 19:54:03.000000 borgmatic-1.7.9/docs/_includes/prism-theme.css
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.556386 borgmatic-1.7.9/docs/how-to/
+-rw-r--r--   0 witten    (1000) witten    (1000)     4522 2022-08-22 03:42:17.000000 borgmatic-1.7.9/docs/how-to/add-preparation-and-cleanup-steps-to-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     5082 2023-02-28 17:37:40.000000 borgmatic-1.7.9/docs/how-to/backup-to-a-removable-drive-or-an-intermittent-server.md
+-rw-r--r--   0 witten    (1000) witten    (1000)    12509 2023-03-09 00:09:27.000000 borgmatic-1.7.9/docs/how-to/backup-your-databases.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     6760 2023-03-08 22:04:20.000000 borgmatic-1.7.9/docs/how-to/deal-with-very-large-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     4667 2023-03-16 20:24:06.000000 borgmatic-1.7.9/docs/how-to/develop-on-borgmatic.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     4263 2023-03-07 06:45:31.000000 borgmatic-1.7.9/docs/how-to/extract-a-backup.md
+-rw-r--r--   0 witten    (1000) witten    (1000)       66 2021-12-06 19:54:03.000000 borgmatic-1.7.9/docs/how-to/index.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     4823 2023-03-09 00:09:35.000000 borgmatic-1.7.9/docs/how-to/inspect-your-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     2057 2023-02-28 17:37:40.000000 borgmatic-1.7.9/docs/how-to/make-backups-redundant.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     8860 2023-02-28 17:37:40.000000 borgmatic-1.7.9/docs/how-to/make-per-application-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)    14065 2023-03-08 21:56:29.000000 borgmatic-1.7.9/docs/how-to/monitor-your-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     3110 2022-08-22 04:14:10.000000 borgmatic-1.7.9/docs/how-to/provide-your-passwords.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      124 2022-06-16 18:55:15.000000 borgmatic-1.7.9/docs/how-to/restore-a-backup.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     3924 2022-12-12 19:25:31.000000 borgmatic-1.7.9/docs/how-to/run-arbitrary-borg-commands.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      152 2022-06-16 18:55:21.000000 borgmatic-1.7.9/docs/how-to/run-preparation-steps-before-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)    14869 2023-02-28 17:37:40.000000 borgmatic-1.7.9/docs/how-to/set-up-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     7785 2023-02-28 17:37:40.000000 borgmatic-1.7.9/docs/how-to/upgrade.md
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.556386 borgmatic-1.7.9/docs/reference/
+-rw-r--r--   0 witten    (1000) witten    (1000)      331 2023-02-28 17:37:40.000000 borgmatic-1.7.9/docs/reference/command-line.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      426 2023-02-28 17:37:40.000000 borgmatic-1.7.9/docs/reference/configuration.md
+-rw-r--r--   0 witten    (1000) witten    (1000)       69 2021-12-06 19:54:03.000000 borgmatic-1.7.9/docs/reference/index.md
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.559719 borgmatic-1.7.9/docs/static/
+-rw-r--r--   0 witten    (1000) witten    (1000)     5822 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/static/borgbase.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     3593 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/static/borgmatic.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     1674 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/static/borgmatic.svg
+-rw-r--r--   0 witten    (1000) witten    (1000)    23536 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/static/cronhub.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    10364 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/static/cronitor.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     4556 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/static/healthchecks.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     9474 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/static/mariadb.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    12839 2022-03-05 23:40:50.000000 borgmatic-1.7.9/docs/static/mongodb.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     3761 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/static/mysql.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    10266 2022-06-09 20:35:18.000000 borgmatic-1.7.9/docs/static/ntfy.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    20107 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/static/pagerduty.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    31528 2021-06-08 17:56:16.000000 borgmatic-1.7.9/docs/static/postgresql.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     4668 2023-03-04 17:53:36.000000 borgmatic-1.7.9/docs/static/sqlite.png
+-rw-r--r--   0 witten    (1000) witten    (1000)       64 2021-06-08 17:56:16.000000 borgmatic-1.7.9/pyproject.toml
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.539719 borgmatic-1.7.9/sample/
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.559719 borgmatic-1.7.9/sample/cron/
+-rw-r--r--   0 witten    (1000) witten    (1000)      183 2022-03-05 23:40:50.000000 borgmatic-1.7.9/sample/cron/borgmatic
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.559719 borgmatic-1.7.9/sample/systemd/
+-rw-r--r--   0 witten    (1000) witten    (1000)     2612 2022-12-12 19:25:31.000000 borgmatic-1.7.9/sample/systemd/borgmatic.service
+-rw-r--r--   0 witten    (1000) witten    (1000)      138 2022-05-08 06:08:53.000000 borgmatic-1.7.9/sample/systemd/borgmatic.timer
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.559719 borgmatic-1.7.9/scripts/
+-rwxr-xr-x   0 witten    (1000) witten    (1000)      241 2023-01-27 02:00:56.000000 borgmatic-1.7.9/scripts/dev-docs
+-rwxr-xr-x   0 witten    (1000) witten    (1000)     3108 2022-12-12 19:25:31.000000 borgmatic-1.7.9/scripts/find-unsupported-borg-options
+-rwxr-xr-x   0 witten    (1000) witten    (1000)      137 2021-06-08 17:56:16.000000 borgmatic-1.7.9/scripts/push
+-rwxr-xr-x   0 witten    (1000) witten    (1000)     1838 2023-03-04 17:49:38.000000 borgmatic-1.7.9/scripts/release
+-rwxr-xr-x   0 witten    (1000) witten    (1000)      517 2021-06-08 17:56:16.000000 borgmatic-1.7.9/scripts/run-full-dev-tests
+-rwxr-xr-x   0 witten    (1000) witten    (1000)      991 2023-03-04 17:47:51.000000 borgmatic-1.7.9/scripts/run-full-tests
+-rw-r--r--   0 witten    (1000) witten    (1000)      513 2023-03-16 20:46:45.573053 borgmatic-1.7.9/setup.cfg
+-rw-r--r--   0 witten    (1000) witten    (1000)     1372 2023-03-16 20:42:11.000000 borgmatic-1.7.9/setup.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      566 2023-03-07 22:02:22.000000 borgmatic-1.7.9/test_requirements.txt
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.559719 borgmatic-1.7.9/tests/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.563053 borgmatic-1.7.9/tests/end-to-end/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/end-to-end/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      626 2022-03-05 23:40:50.000000 borgmatic-1.7.9/tests/end-to-end/docker-compose.yaml
+-rw-r--r--   0 witten    (1000) witten    (1000)     3180 2022-08-22 05:57:33.000000 borgmatic-1.7.9/tests/end-to-end/test_borgmatic.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      143 2022-05-26 18:07:14.000000 borgmatic-1.7.9/tests/end-to-end/test_completion.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     6274 2023-03-04 17:47:51.000000 borgmatic-1.7.9/tests/end-to-end/test_database.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      588 2022-08-19 06:07:33.000000 borgmatic-1.7.9/tests/end-to-end/test_generate_config.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2006 2022-08-22 06:22:23.000000 borgmatic-1.7.9/tests/end-to-end/test_override.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1227 2022-08-18 03:47:17.000000 borgmatic-1.7.9/tests/end-to-end/test_validate_config.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.563053 borgmatic-1.7.9/tests/integration/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/integration/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.563053 borgmatic-1.7.9/tests/integration/borg/
+-rw-r--r--   0 witten    (1000) witten    (1000)      546 2022-03-05 23:40:50.000000 borgmatic-1.7.9/tests/integration/borg/test_feature.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.563053 borgmatic-1.7.9/tests/integration/commands/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/integration/commands/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    18673 2023-03-16 20:24:06.000000 borgmatic-1.7.9/tests/integration/commands/test_arguments.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      432 2022-08-21 21:13:43.000000 borgmatic-1.7.9/tests/integration/commands/test_borgmatic.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      133 2022-05-26 16:53:24.000000 borgmatic-1.7.9/tests/integration/commands/test_completion.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1671 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/integration/commands/test_convert_config.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      803 2022-05-29 23:00:10.000000 borgmatic-1.7.9/tests/integration/commands/test_generate_config.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      672 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/integration/commands/test_validate_config.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.563053 borgmatic-1.7.9/tests/integration/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/integration/config/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7927 2022-06-30 20:10:10.000000 borgmatic-1.7.9/tests/integration/config/test_generate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      578 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/integration/config/test_legacy.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    15187 2022-05-20 22:15:07.000000 borgmatic-1.7.9/tests/integration/config/test_load.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1039 2021-11-29 20:38:51.000000 borgmatic-1.7.9/tests/integration/config/test_override.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      234 2021-12-06 19:54:03.000000 borgmatic-1.7.9/tests/integration/config/test_schema.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7699 2023-03-07 22:03:24.000000 borgmatic-1.7.9/tests/integration/config/test_validate.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.563053 borgmatic-1.7.9/tests/integration/hooks/
+-rw-r--r--   0 witten    (1000) witten    (1000)      729 2021-12-06 19:54:03.000000 borgmatic-1.7.9/tests/integration/hooks/test_healthchecks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    11263 2022-08-28 16:03:46.000000 borgmatic-1.7.9/tests/integration/test_execute.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.563053 borgmatic-1.7.9/tests/unit/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/unit/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.566386 borgmatic-1.7.9/tests/unit/actions/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/actions/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      760 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/actions/test_borg.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      636 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/actions/test_break_lock.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3105 2023-03-16 20:24:53.000000 borgmatic-1.7.9/tests/unit/actions/test_check.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3142 2023-03-16 20:25:01.000000 borgmatic-1.7.9/tests/unit/actions/test_compact.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3418 2023-03-16 20:24:57.000000 borgmatic-1.7.9/tests/unit/actions/test_create.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      958 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/actions/test_export_tar.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1104 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/actions/test_extract.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      808 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/actions/test_info.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      799 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/actions/test_list.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      764 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/actions/test_mount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2712 2023-03-16 20:24:48.000000 borgmatic-1.7.9/tests/unit/actions/test_prune.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1730 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/actions/test_rcreate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    18426 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/actions/test_restore.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      679 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/actions/test_rinfo.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      671 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/actions/test_rlist.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      621 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/actions/test_transfer.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.569719 borgmatic-1.7.9/tests/unit/borg/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/unit/borg/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    12347 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/borg/test_borg.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2534 2022-12-12 19:25:31.000000 borgmatic-1.7.9/tests/unit/borg/test_break_lock.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    25781 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/borg/test_check.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     5527 2022-08-19 06:07:33.000000 borgmatic-1.7.9/tests/unit/borg/test_compact.py
+-rw-r--r--   0 witten    (1000) witten    (1000)   116577 2023-03-07 22:08:00.000000 borgmatic-1.7.9/tests/unit/borg/test_create.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1174 2022-06-30 19:15:33.000000 borgmatic-1.7.9/tests/unit/borg/test_environment.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    10755 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/borg/test_export_tar.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    15997 2023-03-09 18:07:00.000000 borgmatic-1.7.9/tests/unit/borg/test_extract.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2846 2022-08-19 06:07:33.000000 borgmatic-1.7.9/tests/unit/borg/test_flags.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    13294 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/borg/test_info.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    23301 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/borg/test_list.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7359 2022-12-12 19:25:31.000000 borgmatic-1.7.9/tests/unit/borg/test_mount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    10592 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/borg/test_prune.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     9791 2022-08-19 16:27:22.000000 borgmatic-1.7.9/tests/unit/borg/test_rcreate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     9342 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/borg/test_rinfo.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    14072 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/borg/test_rlist.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    14768 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/borg/test_transfer.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      920 2022-06-30 19:06:41.000000 borgmatic-1.7.9/tests/unit/borg/test_umount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2063 2022-12-12 19:25:31.000000 borgmatic-1.7.9/tests/unit/borg/test_version.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.569719 borgmatic-1.7.9/tests/unit/commands/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/unit/commands/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     5746 2023-03-08 20:11:06.000000 borgmatic-1.7.9/tests/unit/commands/test_arguments.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    44909 2023-03-08 21:50:23.000000 borgmatic-1.7.9/tests/unit/commands/test_borgmatic.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.569719 borgmatic-1.7.9/tests/unit/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/unit/config/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      709 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/unit/config/test_checks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7576 2021-12-06 19:54:03.000000 borgmatic-1.7.9/tests/unit/config/test_collect.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     5380 2022-03-05 23:40:50.000000 borgmatic-1.7.9/tests/unit/config/test_convert.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2880 2022-06-23 17:40:47.000000 borgmatic-1.7.9/tests/unit/config/test_environment.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     5549 2022-03-05 23:40:50.000000 borgmatic-1.7.9/tests/unit/config/test_generate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7470 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/unit/config/test_legacy.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3381 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/config/test_normalize.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2827 2022-03-05 23:40:50.000000 borgmatic-1.7.9/tests/unit/config/test_override.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     6214 2022-08-17 16:56:29.000000 borgmatic-1.7.9/tests/unit/config/test_validate.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-03-16 20:46:45.573053 borgmatic-1.7.9/tests/unit/hooks/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.7.9/tests/unit/hooks/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4092 2022-05-23 22:26:48.000000 borgmatic-1.7.9/tests/unit/hooks/test_command.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3525 2023-03-07 22:22:17.000000 borgmatic-1.7.9/tests/unit/hooks/test_cronhub.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2973 2023-03-07 22:22:17.000000 borgmatic-1.7.9/tests/unit/hooks/test_cronitor.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4402 2022-12-12 19:25:31.000000 borgmatic-1.7.9/tests/unit/hooks/test_dispatch.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2938 2021-12-06 19:54:03.000000 borgmatic-1.7.9/tests/unit/hooks/test_dump.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    11575 2023-03-07 22:22:17.000000 borgmatic-1.7.9/tests/unit/hooks/test_healthchecks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    11590 2023-03-07 22:08:11.000000 borgmatic-1.7.9/tests/unit/hooks/test_mongodb.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    15616 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/hooks/test_mysql.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7267 2023-03-07 23:37:04.000000 borgmatic-1.7.9/tests/unit/hooks/test_ntfy.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2231 2022-06-30 04:15:15.000000 borgmatic-1.7.9/tests/unit/hooks/test_pagerduty.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    26214 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/hooks/test_postgresql.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     5020 2023-03-04 17:47:51.000000 borgmatic-1.7.9/tests/unit/hooks/test_sqlite.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    16090 2022-12-12 19:25:31.000000 borgmatic-1.7.9/tests/unit/test_execute.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    13531 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/test_logger.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1405 2022-04-28 23:35:37.000000 borgmatic-1.7.9/tests/unit/test_signals.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1265 2023-02-28 17:37:40.000000 borgmatic-1.7.9/tests/unit/test_verbosity.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      711 2023-03-16 20:28:32.000000 borgmatic-1.7.9/tox.ini
```

### Comparing `borgmatic-1.7.8/.drone.yml` & `borgmatic-1.7.9/.drone.yml`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/.eleventy.js` & `borgmatic-1.7.9/.eleventy.js`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/.gitea/issue_template.md` & `borgmatic-1.7.9/.gitea/issue_template.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/AUTHORS` & `borgmatic-1.7.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/LICENSE` & `borgmatic-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/NEWS` & `borgmatic-1.7.9/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+1.7.9
+ * #295: Add a SQLite database dump/restore hook.
+ * #304: Change the default action order when no actions are specified on the command-line to:
+   "create", "prune", "compact", "check". If you'd like to retain the old ordering ("prune" and
+   "compact" first), then specify actions explicitly on the command-line.
+ * #304: Run any command-line actions in the order specified instead of using a fixed ordering.
+ * #564: Add "--repository" flag to all actions where it makes sense, so you can run borgmatic on
+   a single configured repository instead of all of them.
+ * #628: Add a Healthchecks "log" state to send borgmatic logs to Healthchecks without signalling
+   success or failure.
+ * #647: Add "--strip-components all" feature on the "extract" action to remove leading path
+   components of files you extract. Must be used with the "--path" flag.
+ * Add support for Python 3.11.
+
 1.7.8
  * #620: With the "create" action and the "--list" ("--files") flag, only show excluded files at
    verbosity 2.
  * #621: Add optional authentication to the ntfy monitoring hook.
  * With the "create" action, only one of "--list" ("--files") and "--progress" flags can be used.
    This lines up with the new behavior in Borg 2.0.0b5.
  * Internally support new Borg 2.0.0b5 "--filter" status characters / item flags for the "create"
```

### Comparing `borgmatic-1.7.8/PKG-INFO` & `borgmatic-1.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borgmatic
-Version: 1.7.8
+Version: 1.7.9
 Summary: Simple, configuration-driven backup software for servers and workstations
 Home-page: https://torsion.org/borgmatic
 Author: Dan Helfman
 Author-email: witten@torsion.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
```

### Comparing `borgmatic-1.7.8/README.md` & `borgmatic-1.7.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -63,29 +63,30 @@
 
 ## Integrations
 
 <a href="https://www.postgresql.org/"><img src="docs/static/postgresql.png" alt="PostgreSQL" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://www.mysql.com/"><img src="docs/static/mysql.png" alt="MySQL" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://mariadb.com/"><img src="docs/static/mariadb.png" alt="MariaDB" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://www.mongodb.com/"><img src="docs/static/mongodb.png" alt="MongoDB" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
+<a href="https://sqlite.org/"><img src="docs/static/sqlite.png" alt="SQLite" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://healthchecks.io/"><img src="docs/static/healthchecks.png" alt="Healthchecks" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://cronitor.io/"><img src="docs/static/cronitor.png" alt="Cronitor" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://cronhub.io/"><img src="docs/static/cronhub.png" alt="Cronhub" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://www.pagerduty.com/"><img src="docs/static/pagerduty.png" alt="PagerDuty" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://ntfy.sh/"><img src="docs/static/ntfy.png" alt="ntfy" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://www.borgbase.com/?utm_source=borgmatic"><img src="docs/static/borgbase.png" alt="BorgBase" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 
 
 ## Getting started
 
 Your first step is to [install and configure
 borgmatic](https://torsion.org/borgmatic/docs/how-to/set-up-backups/).
 
-For additional documentation, check out the links above for <a
-href="https://torsion.org/borgmatic/#documentation">borgmatic how-to and
+For additional documentation, check out the links above (left panel on wide screens)
+for <a href="https://torsion.org/borgmatic/#documentation">borgmatic how-to and
 reference guides</a>.
 
 
 ## Hosting providers
 
 Need somewhere to store your encrypted off-site backups? The following hosting
 providers include specific support for Borg/borgmatic—and fund borgmatic
```

#### html2text {}

```diff
@@ -13,23 +13,24 @@
 frequency: 2 weeks hooks: # Custom preparation scripts to run. before_backup: -
 prepare-for-backup.sh # Databases to dump and include in backups.
 postgresql_databases: - name: users # Third-party services to notify you if
 backups aren't happening. healthchecks: https://hc-ping.com/be067061-cf96-4412-
 8eae-62b0c50d6a8c ``` Want to see borgmatic in action? Check out the
 screencast. [https://asciinema.org/a/203761.png] borgmatic is powered by [Borg
 Backup](https://www.borgbackup.org/). ## Integrations [PostgreSQL]     
-[MySQL]      [MariaDB]      [MongoDB]      [Healthchecks]      [Cronitor]     
-[Cronhub]      [PagerDuty]      [ntfy]      [BorgBase]      ## Getting started
-Your first step is to [install and configure borgmatic](https://torsion.org/
-borgmatic/docs/how-to/set-up-backups/). For additional documentation, check out
-the links above for borgmatic_how-to_and_reference_guides. ## Hosting providers
-Need somewhere to store your encrypted off-site backups? The following hosting
-providers include specific support for Borg/borgmaticâand fund borgmatic
-development and hosting when you use these links to sign up. (These are
-referral links, but without any tracking scripts or cookies.)
+[MySQL]      [MariaDB]      [MongoDB]      [SQLite]      [Healthchecks]     
+[Cronitor]      [Cronhub]      [PagerDuty]      [ntfy]      [BorgBase]      ##
+Getting started Your first step is to [install and configure borgmatic](https:/
+/torsion.org/borgmatic/docs/how-to/set-up-backups/). For additional
+documentation, check out the links above (left panel on wide screens) for
+borgmatic_how-to_and_reference_guides. ## Hosting providers Need somewhere to
+store your encrypted off-site backups? The following hosting providers include
+specific support for Borg/borgmaticâand fund borgmatic development and
+hosting when you use these links to sign up. (These are referral links, but
+without any tracking scripts or cookies.)
     * BorgBase: Borg hosting service with support for monitoring, 2FA, and
       append-only repos
 Additionally, [rsync.net](https://www.rsync.net/products/borg.html) and
 [Hetzner](https://www.hetzner.com/storage/storage-box) have compatible storage
 offerings, but do not currently fund borgmatic development or hosting. ##
 Support and contributing ### Issues Are you experiencing an issue with
 borgmatic? Or do you have an idea for a feature enhancement? Head on over to
```

### Comparing `borgmatic-1.7.8/SECURITY.md` & `borgmatic-1.7.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/actions/borg.py` & `borgmatic-1.7.9/borgmatic/actions/borg.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/actions/break_lock.py` & `borgmatic-1.7.9/borgmatic/actions/break_lock.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/actions/check.py` & `borgmatic-1.7.9/borgmatic/actions/check.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 
 import borgmatic.borg.check
+import borgmatic.config.validate
 import borgmatic.hooks.command
 
 logger = logging.getLogger(__name__)
 
 
 def run_check(
     config_filename,
@@ -19,14 +20,19 @@
     global_arguments,
     local_path,
     remote_path,
 ):
     '''
     Run the "check" action for the given repository.
     '''
+    if check_arguments.repository and not borgmatic.config.validate.repositories_match(
+        repository, check_arguments.repository
+    ):
+        return
+
     borgmatic.hooks.command.execute_hook(
         hooks.get('before_check'),
         hooks.get('umask'),
         config_filename,
         'pre-check',
         global_arguments.dry_run,
         **hook_context,
```

### Comparing `borgmatic-1.7.8/borgmatic/actions/compact.py` & `borgmatic-1.7.9/borgmatic/actions/compact.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 
 import borgmatic.borg.compact
 import borgmatic.borg.feature
+import borgmatic.config.validate
 import borgmatic.hooks.command
 
 logger = logging.getLogger(__name__)
 
 
 def run_compact(
     config_filename,
@@ -20,14 +21,19 @@
     dry_run_label,
     local_path,
     remote_path,
 ):
     '''
     Run the "compact" action for the given repository.
     '''
+    if compact_arguments.repository and not borgmatic.config.validate.repositories_match(
+        repository, compact_arguments.repository
+    ):
+        return
+
     borgmatic.hooks.command.execute_hook(
         hooks.get('before_compact'),
         hooks.get('umask'),
         config_filename,
         'pre-compact',
         global_arguments.dry_run,
         **hook_context,
```

### Comparing `borgmatic-1.7.8/borgmatic/actions/create.py` & `borgmatic-1.7.9/borgmatic/actions/create.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 
 import borgmatic.borg.create
+import borgmatic.config.validate
 import borgmatic.hooks.command
 import borgmatic.hooks.dispatch
 import borgmatic.hooks.dump
 
 logger = logging.getLogger(__name__)
 
 
@@ -24,14 +25,19 @@
     remote_path,
 ):
     '''
     Run the "create" action for the given repository.
 
     If create_arguments.json is True, yield the JSON output from creating the archive.
     '''
+    if create_arguments.repository and not borgmatic.config.validate.repositories_match(
+        repository, create_arguments.repository
+    ):
+        return
+
     borgmatic.hooks.command.execute_hook(
         hooks.get('before_backup'),
         hooks.get('umask'),
         config_filename,
         'pre-backup',
         global_arguments.dry_run,
         **hook_context,
```

### Comparing `borgmatic-1.7.8/borgmatic/actions/export_tar.py` & `borgmatic-1.7.9/borgmatic/actions/export_tar.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/actions/extract.py` & `borgmatic-1.7.9/borgmatic/actions/extract.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/actions/info.py` & `borgmatic-1.7.9/borgmatic/actions/info.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/actions/list.py` & `borgmatic-1.7.9/borgmatic/actions/list.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/actions/mount.py` & `borgmatic-1.7.9/borgmatic/actions/mount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/actions/prune.py` & `borgmatic-1.7.9/borgmatic/actions/prune.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 
 import borgmatic.borg.prune
+import borgmatic.config.validate
 import borgmatic.hooks.command
 
 logger = logging.getLogger(__name__)
 
 
 def run_prune(
     config_filename,
@@ -19,14 +20,19 @@
     dry_run_label,
     local_path,
     remote_path,
 ):
     '''
     Run the "prune" action for the given repository.
     '''
+    if prune_arguments.repository and not borgmatic.config.validate.repositories_match(
+        repository, prune_arguments.repository
+    ):
+        return
+
     borgmatic.hooks.command.execute_hook(
         hooks.get('before_prune'),
         hooks.get('umask'),
         config_filename,
         'pre-prune',
         global_arguments.dry_run,
         **hook_context,
```

### Comparing `borgmatic-1.7.8/borgmatic/actions/rcreate.py` & `borgmatic-1.7.9/borgmatic/actions/rcreate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/actions/restore.py` & `borgmatic-1.7.9/borgmatic/actions/restore.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/actions/rinfo.py` & `borgmatic-1.7.9/borgmatic/actions/rinfo.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/actions/rlist.py` & `borgmatic-1.7.9/borgmatic/actions/rlist.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/actions/transfer.py` & `borgmatic-1.7.9/borgmatic/actions/transfer.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/borg.py` & `borgmatic-1.7.9/borgmatic/borg/borg.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/break_lock.py` & `borgmatic-1.7.9/borgmatic/borg/break_lock.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/check.py` & `borgmatic-1.7.9/borgmatic/borg/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             continue
 
         # If we've not yet reached the time when the frequency dictates we're ready for another
         # check, skip this check.
         if datetime.datetime.now() < check_time + frequency_delta:
             remaining = check_time + frequency_delta - datetime.datetime.now()
             logger.info(
-                f"Skipping {check} check due to configured frequency; {remaining} until next check"
+                f'Skipping {check} check due to configured frequency; {remaining} until next check'
             )
             filtered_checks.remove(check)
 
     return tuple(filtered_checks)
 
 
 def make_check_flags(local_borg_version, checks, check_last=None, prefix=None):
```

### Comparing `borgmatic-1.7.8/borgmatic/borg/compact.py` & `borgmatic-1.7.9/borgmatic/borg/compact.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/create.py` & `borgmatic-1.7.9/borgmatic/borg/create.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/environment.py` & `borgmatic-1.7.9/borgmatic/borg/environment.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/export_tar.py` & `borgmatic-1.7.9/borgmatic/borg/export_tar.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/extract.py` & `borgmatic-1.7.9/borgmatic/borg/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,14 +83,21 @@
         raise ValueError('progress and extract_to_stdout cannot both be set')
 
     if feature.available(feature.Feature.NUMERIC_IDS, local_borg_version):
         numeric_ids_flags = ('--numeric-ids',) if location_config.get('numeric_ids') else ()
     else:
         numeric_ids_flags = ('--numeric-owner',) if location_config.get('numeric_ids') else ()
 
+    if strip_components == 'all':
+        if not paths:
+            raise ValueError('The --strip-components flag with "all" requires at least one --path')
+
+        # Calculate the maximum number of leading path components of the given paths.
+        strip_components = max(0, *(len(path.split(os.path.sep)) - 1 for path in paths))
+
     full_command = (
         (local_path, 'extract')
         + (('--remote-path', remote_path) if remote_path else ())
         + numeric_ids_flags
         + (('--umask', str(umask)) if umask else ())
         + (('--lock-wait', str(lock_wait)) if lock_wait else ())
         + (('--info',) if logger.getEffectiveLevel() == logging.INFO else ())
```

### Comparing `borgmatic-1.7.8/borgmatic/borg/feature.py` & `borgmatic-1.7.9/borgmatic/borg/feature.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/flags.py` & `borgmatic-1.7.9/borgmatic/borg/flags.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/info.py` & `borgmatic-1.7.9/borgmatic/borg/info.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/list.py` & `borgmatic-1.7.9/borgmatic/borg/list.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/mount.py` & `borgmatic-1.7.9/borgmatic/borg/mount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/prune.py` & `borgmatic-1.7.9/borgmatic/borg/prune.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/rcreate.py` & `borgmatic-1.7.9/borgmatic/borg/rcreate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/rinfo.py` & `borgmatic-1.7.9/borgmatic/borg/rinfo.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/rlist.py` & `borgmatic-1.7.9/borgmatic/borg/rlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     '''
     Given a local or remote repository path, an archive name, a storage config dict, a local Borg
     path, and a remote Borg path, simply return the archive name. But if the archive name is
     "latest", then instead introspect the repository for the latest archive and return its name.
 
     Raise ValueError if "latest" is given but there are no archives in the repository.
     '''
-    if archive != "latest":
+    if archive != 'latest':
         return archive
 
     lock_wait = storage_config.get('lock_wait', None)
 
     full_command = (
         (
             local_path,
```

### Comparing `borgmatic-1.7.8/borgmatic/borg/transfer.py` & `borgmatic-1.7.9/borgmatic/borg/transfer.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/umount.py` & `borgmatic-1.7.9/borgmatic/borg/umount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/borg/version.py` & `borgmatic-1.7.9/borgmatic/borg/version.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/commands/arguments.py` & `borgmatic-1.7.9/borgmatic/commands/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,19 +42,20 @@
     }
 
     # If the "borg" action is used, skip all other subparsers. This avoids confusion like
     # "borg list" triggering borgmatic's own list action.
     if 'borg' in unparsed_arguments:
         subparsers = {'borg': subparsers['borg']}
 
-    for subparser_name, subparser in subparsers.items():
-        if subparser_name not in remaining_arguments:
-            continue
+    for argument in remaining_arguments:
+        canonical_name = alias_to_subparser_name.get(argument, argument)
+        subparser = subparsers.get(canonical_name)
 
-        canonical_name = alias_to_subparser_name.get(subparser_name, subparser_name)
+        if not subparser:
+            continue
 
         # If a parsed value happens to be the same as the name of a subparser, remove it from the
         # remaining arguments. This prevents, for instance, "check --only extract" from triggering
         # the "extract" subparser.
         parsed, unused_remaining = subparser.parse_known_args(unparsed_arguments)
         for value in vars(parsed).values():
             if isinstance(value, str):
@@ -63,17 +64,17 @@
             elif isinstance(value, list):
                 for item in value:
                     if item in subparsers:
                         remaining_arguments.remove(item)
 
         arguments[canonical_name] = parsed
 
-    # If no actions are explicitly requested, assume defaults: prune, compact, create, and check.
+    # If no actions are explicitly requested, assume defaults.
     if not arguments and '--help' not in unparsed_arguments and '-h' not in unparsed_arguments:
-        for subparser_name in ('prune', 'compact', 'create', 'check'):
+        for subparser_name in ('create', 'prune', 'compact', 'check'):
             subparser = subparsers[subparser_name]
             parsed, unused_remaining = subparser.parse_known_args(unparsed_arguments)
             arguments[subparser_name] = parsed
 
     remaining_arguments = list(unparsed_arguments)
 
     # Now ask each subparser, one by one, to greedily consume arguments.
@@ -211,24 +212,24 @@
         action='store_true',
         help='Display installed version number of borgmatic and exit',
     )
 
     top_level_parser = ArgumentParser(
         description='''
             Simple, configuration-driven backup software for servers and workstations. If none of
-            the action options are given, then borgmatic defaults to: prune, compact, create, and
+            the action options are given, then borgmatic defaults to: create, prune, compact, and
             check.
             ''',
         parents=[global_parser],
     )
 
     subparsers = top_level_parser.add_subparsers(
         title='actions',
         metavar='',
-        help='Specify zero or more actions. Defaults to prune, compact, create, and check. Use --help with action for details:',
+        help='Specify zero or more actions. Defaults to creat, prune, compact, and check. Use --help with action for details:',
     )
     rcreate_parser = subparsers.add_parser(
         'rcreate',
         aliases=SUBPARSER_ALIASES['rcreate'],
         help='Create a new, empty Borg repository',
         description='Create a new, empty Borg repository',
         add_help=False,
@@ -329,14 +330,18 @@
         aliases=SUBPARSER_ALIASES['prune'],
         help='Prune archives according to the retention policy (with Borg 1.2+, run compact afterwards to actually free space)',
         description='Prune archives according to the retention policy (with Borg 1.2+, run compact afterwards to actually free space)',
         add_help=False,
     )
     prune_group = prune_parser.add_argument_group('prune arguments')
     prune_group.add_argument(
+        '--repository',
+        help='Path of specific existing repository to prune (must be already specified in a borgmatic configuration file)',
+    )
+    prune_group.add_argument(
         '--stats',
         dest='stats',
         default=False,
         action='store_true',
         help='Display statistics of archive',
     )
     prune_group.add_argument(
@@ -349,14 +354,18 @@
         aliases=SUBPARSER_ALIASES['compact'],
         help='Compact segments to free space (Borg 1.2+, borgmatic 1.5.23+ only)',
         description='Compact segments to free space (Borg 1.2+, borgmatic 1.5.23+ only)',
         add_help=False,
     )
     compact_group = compact_parser.add_argument_group('compact arguments')
     compact_group.add_argument(
+        '--repository',
+        help='Path of specific existing repository to compact (must be already specified in a borgmatic configuration file)',
+    )
+    compact_group.add_argument(
         '--progress',
         dest='progress',
         default=False,
         action='store_true',
         help='Display progress as each segment is compacted',
     )
     compact_group.add_argument(
@@ -381,14 +390,18 @@
         aliases=SUBPARSER_ALIASES['create'],
         help='Create an archive (actually perform a backup)',
         description='Create an archive (actually perform a backup)',
         add_help=False,
     )
     create_group = create_parser.add_argument_group('create arguments')
     create_group.add_argument(
+        '--repository',
+        help='Path of specific existing repository to backup to (must be already specified in a borgmatic configuration file)',
+    )
+    create_group.add_argument(
         '--progress',
         dest='progress',
         default=False,
         action='store_true',
         help='Display progress for each file as it is backed up',
     )
     create_group.add_argument(
@@ -411,14 +424,18 @@
         aliases=SUBPARSER_ALIASES['check'],
         help='Check archives for consistency',
         description='Check archives for consistency',
         add_help=False,
     )
     check_group = check_parser.add_argument_group('check arguments')
     check_group.add_argument(
+        '--repository',
+        help='Path of specific existing repository to check (must be already specified in a borgmatic configuration file)',
+    )
+    check_group.add_argument(
         '--progress',
         dest='progress',
         default=False,
         action='store_true',
         help='Display progress for each file as it is checked',
     )
     check_group.add_argument(
@@ -471,18 +488,17 @@
         '--destination',
         metavar='PATH',
         dest='destination',
         help='Directory to extract files into, defaults to the current directory',
     )
     extract_group.add_argument(
         '--strip-components',
-        type=int,
+        type=lambda number: number if number == 'all' else int(number),
         metavar='NUMBER',
-        dest='strip_components',
-        help='Number of leading path components to remove from each extracted path. Skip paths with fewer elements',
+        help='Number of leading path components to remove from each extracted path or "all" to strip all leading path components. Skip paths with fewer elements',
     )
     extract_group.add_argument(
         '--progress',
         dest='progress',
         default=False,
         action='store_true',
         help='Display progress for each file as it is extracted',
@@ -607,15 +623,15 @@
         '--archive', help='Name of archive to restore from (or "latest")', required=True
     )
     restore_group.add_argument(
         '--database',
         metavar='NAME',
         nargs='+',
         dest='databases',
-        help='Names of databases to restore from archive, defaults to all databases. Note that any databases to restore must be defined in borgmatic\'s configuration',
+        help="Names of databases to restore from archive, defaults to all databases. Note that any databases to restore must be defined in borgmatic's configuration",
     )
     restore_group.add_argument(
         '-h', '--help', action='help', help='Show this help message and exit'
     )
 
     rlist_parser = subparsers.add_parser(
         'rlist',
@@ -801,15 +817,15 @@
         '-h', '--help', action='help', help='Show this help message and exit'
     )
 
     borg_parser = subparsers.add_parser(
         'borg',
         aliases=SUBPARSER_ALIASES['borg'],
         help='Run an arbitrary Borg command',
-        description='Run an arbitrary Borg command based on borgmatic\'s configuration',
+        description="Run an arbitrary Borg command based on borgmatic's configuration",
         add_help=False,
     )
     borg_group = borg_parser.add_argument_group('borg arguments')
     borg_group.add_argument(
         '--repository',
         help='Path of repository to pass to Borg, defaults to the configured repositories',
     )
```

### Comparing `borgmatic-1.7.8/borgmatic/commands/borgmatic.py` & `borgmatic-1.7.9/borgmatic/commands/borgmatic.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
 LEGACY_CONFIG_PATH = '/etc/borgmatic/config'
 
 
 def run_configuration(config_filename, config, arguments):
     '''
     Given a config filename, the corresponding parsed config dict, and command-line arguments as a
-    dict from subparser name to a namespace of parsed arguments, execute the defined prune, compact,
-    create, check, and/or other actions.
+    dict from subparser name to a namespace of parsed arguments, execute the defined create, prune,
+    compact, check, and/or other actions.
 
     Yield a combination of:
 
       * JSON output strings from successfully executing any actions that produce JSON
       * logging.LogRecord instances containing errors from any actions or backup hooks that fail
     '''
     (location, storage, retention, consistency, hooks) = (
@@ -60,15 +60,15 @@
 
     local_path = location.get('local_path', 'borg')
     remote_path = location.get('remote_path')
     retries = storage.get('retries', 0)
     retry_wait = storage.get('retry_wait', 0)
     encountered_error = None
     error_repository = ''
-    using_primary_action = {'prune', 'compact', 'create', 'check'}.intersection(arguments)
+    using_primary_action = {'create', 'prune', 'compact', 'check'}.intersection(arguments)
     monitoring_log_level = verbosity_to_log_level(global_arguments.monitoring_verbosity)
 
     try:
         local_borg_version = borg_version.local_borg_version(storage, local_path)
     except (OSError, CalledProcessError, ValueError) as error:
         yield from log_error_records(
             '{}: Error getting local Borg version'.format(config_filename), error
@@ -148,14 +148,33 @@
 
                 yield from log_error_records(
                     '{}: Error running actions for repository'.format(repository_path), error
                 )
                 encountered_error = error
                 error_repository = repository_path
 
+    try:
+        if using_primary_action:
+            # send logs irrespective of error
+            dispatch.call_hooks(
+                'ping_monitor',
+                hooks,
+                config_filename,
+                monitor.MONITOR_HOOK_NAMES,
+                monitor.State.LOG,
+                monitoring_log_level,
+                global_arguments.dry_run,
+            )
+    except (OSError, CalledProcessError) as error:
+        if command.considered_soft_failure(config_filename, error):
+            return
+
+        encountered_error = error
+        yield from log_error_records('{}: Error pinging monitor'.format(config_filename), error)
+
     if not encountered_error:
         try:
             if using_primary_action:
                 dispatch.call_hooks(
                     'ping_monitor',
                     hooks,
                     config_filename,
@@ -258,163 +277,170 @@
         hooks.get('umask'),
         config_filename,
         'pre-actions',
         global_arguments.dry_run,
         **hook_context,
     )
 
-    if 'rcreate' in arguments:
-        borgmatic.actions.rcreate.run_rcreate(
-            repository,
-            storage,
-            local_borg_version,
-            arguments['rcreate'],
-            global_arguments,
-            local_path,
-            remote_path,
-        )
-    if 'transfer' in arguments:
-        borgmatic.actions.transfer.run_transfer(
-            repository,
-            storage,
-            local_borg_version,
-            arguments['transfer'],
-            global_arguments,
-            local_path,
-            remote_path,
-        )
-    if 'prune' in arguments:
-        borgmatic.actions.prune.run_prune(
-            config_filename,
-            repository,
-            storage,
-            retention,
-            hooks,
-            hook_context,
-            local_borg_version,
-            arguments['prune'],
-            global_arguments,
-            dry_run_label,
-            local_path,
-            remote_path,
-        )
-    if 'compact' in arguments:
-        borgmatic.actions.compact.run_compact(
-            config_filename,
-            repository,
-            storage,
-            retention,
-            hooks,
-            hook_context,
-            local_borg_version,
-            arguments['compact'],
-            global_arguments,
-            dry_run_label,
-            local_path,
-            remote_path,
-        )
-    if 'create' in arguments:
-        yield from borgmatic.actions.create.run_create(
-            config_filename,
-            repository,
-            location,
-            storage,
-            hooks,
-            hook_context,
-            local_borg_version,
-            arguments['create'],
-            global_arguments,
-            dry_run_label,
-            local_path,
-            remote_path,
-        )
-    if 'check' in arguments and checks.repository_enabled_for_checks(repository, consistency):
-        borgmatic.actions.check.run_check(
-            config_filename,
-            repository,
-            location,
-            storage,
-            consistency,
-            hooks,
-            hook_context,
-            local_borg_version,
-            arguments['check'],
-            global_arguments,
-            local_path,
-            remote_path,
-        )
-    if 'extract' in arguments:
-        borgmatic.actions.extract.run_extract(
-            config_filename,
-            repository,
-            location,
-            storage,
-            hooks,
-            hook_context,
-            local_borg_version,
-            arguments['extract'],
-            global_arguments,
-            local_path,
-            remote_path,
-        )
-    if 'export-tar' in arguments:
-        borgmatic.actions.export_tar.run_export_tar(
-            repository,
-            storage,
-            local_borg_version,
-            arguments['export-tar'],
-            global_arguments,
-            local_path,
-            remote_path,
-        )
-    if 'mount' in arguments:
-        borgmatic.actions.mount.run_mount(
-            repository, storage, local_borg_version, arguments['mount'], local_path, remote_path,
-        )
-    if 'restore' in arguments:
-        borgmatic.actions.restore.run_restore(
-            repository,
-            location,
-            storage,
-            hooks,
-            local_borg_version,
-            arguments['restore'],
-            global_arguments,
-            local_path,
-            remote_path,
-        )
-    if 'rlist' in arguments:
-        yield from borgmatic.actions.rlist.run_rlist(
-            repository, storage, local_borg_version, arguments['rlist'], local_path, remote_path,
-        )
-    if 'list' in arguments:
-        yield from borgmatic.actions.list.run_list(
-            repository, storage, local_borg_version, arguments['list'], local_path, remote_path,
-        )
-    if 'rinfo' in arguments:
-        yield from borgmatic.actions.rinfo.run_rinfo(
-            repository, storage, local_borg_version, arguments['rinfo'], local_path, remote_path,
-        )
-    if 'info' in arguments:
-        yield from borgmatic.actions.info.run_info(
-            repository, storage, local_borg_version, arguments['info'], local_path, remote_path,
-        )
-    if 'break-lock' in arguments:
-        borgmatic.actions.break_lock.run_break_lock(
-            repository,
-            storage,
-            local_borg_version,
-            arguments['break-lock'],
-            local_path,
-            remote_path,
-        )
-    if 'borg' in arguments:
-        borgmatic.actions.borg.run_borg(
-            repository, storage, local_borg_version, arguments['borg'], local_path, remote_path,
-        )
+    for (action_name, action_arguments) in arguments.items():
+        if action_name == 'rcreate':
+            borgmatic.actions.rcreate.run_rcreate(
+                repository,
+                storage,
+                local_borg_version,
+                action_arguments,
+                global_arguments,
+                local_path,
+                remote_path,
+            )
+        elif action_name == 'transfer':
+            borgmatic.actions.transfer.run_transfer(
+                repository,
+                storage,
+                local_borg_version,
+                action_arguments,
+                global_arguments,
+                local_path,
+                remote_path,
+            )
+        elif action_name == 'create':
+            yield from borgmatic.actions.create.run_create(
+                config_filename,
+                repository,
+                location,
+                storage,
+                hooks,
+                hook_context,
+                local_borg_version,
+                action_arguments,
+                global_arguments,
+                dry_run_label,
+                local_path,
+                remote_path,
+            )
+        elif action_name == 'prune':
+            borgmatic.actions.prune.run_prune(
+                config_filename,
+                repository,
+                storage,
+                retention,
+                hooks,
+                hook_context,
+                local_borg_version,
+                action_arguments,
+                global_arguments,
+                dry_run_label,
+                local_path,
+                remote_path,
+            )
+        elif action_name == 'compact':
+            borgmatic.actions.compact.run_compact(
+                config_filename,
+                repository,
+                storage,
+                retention,
+                hooks,
+                hook_context,
+                local_borg_version,
+                action_arguments,
+                global_arguments,
+                dry_run_label,
+                local_path,
+                remote_path,
+            )
+        elif action_name == 'check':
+            if checks.repository_enabled_for_checks(repository, consistency):
+                borgmatic.actions.check.run_check(
+                    config_filename,
+                    repository,
+                    location,
+                    storage,
+                    consistency,
+                    hooks,
+                    hook_context,
+                    local_borg_version,
+                    action_arguments,
+                    global_arguments,
+                    local_path,
+                    remote_path,
+                )
+        elif action_name == 'extract':
+            borgmatic.actions.extract.run_extract(
+                config_filename,
+                repository,
+                location,
+                storage,
+                hooks,
+                hook_context,
+                local_borg_version,
+                action_arguments,
+                global_arguments,
+                local_path,
+                remote_path,
+            )
+        elif action_name == 'export-tar':
+            borgmatic.actions.export_tar.run_export_tar(
+                repository,
+                storage,
+                local_borg_version,
+                action_arguments,
+                global_arguments,
+                local_path,
+                remote_path,
+            )
+        elif action_name == 'mount':
+            borgmatic.actions.mount.run_mount(
+                repository,
+                storage,
+                local_borg_version,
+                arguments['mount'],
+                local_path,
+                remote_path,
+            )
+        elif action_name == 'restore':
+            borgmatic.actions.restore.run_restore(
+                repository,
+                location,
+                storage,
+                hooks,
+                local_borg_version,
+                action_arguments,
+                global_arguments,
+                local_path,
+                remote_path,
+            )
+        elif action_name == 'rlist':
+            yield from borgmatic.actions.rlist.run_rlist(
+                repository, storage, local_borg_version, action_arguments, local_path, remote_path,
+            )
+        elif action_name == 'list':
+            yield from borgmatic.actions.list.run_list(
+                repository, storage, local_borg_version, action_arguments, local_path, remote_path,
+            )
+        elif action_name == 'rinfo':
+            yield from borgmatic.actions.rinfo.run_rinfo(
+                repository, storage, local_borg_version, action_arguments, local_path, remote_path,
+            )
+        elif action_name == 'info':
+            yield from borgmatic.actions.info.run_info(
+                repository, storage, local_borg_version, action_arguments, local_path, remote_path,
+            )
+        elif action_name == 'break-lock':
+            borgmatic.actions.break_lock.run_break_lock(
+                repository,
+                storage,
+                local_borg_version,
+                arguments['break-lock'],
+                local_path,
+                remote_path,
+            )
+        elif action_name == 'borg':
+            borgmatic.actions.borg.run_borg(
+                repository, storage, local_borg_version, action_arguments, local_path, remote_path,
+            )
 
     command.execute_hook(
         hooks.get('after_actions'),
         hooks.get('umask'),
         config_filename,
         'post-actions',
         global_arguments.dry_run,
```

### Comparing `borgmatic-1.7.8/borgmatic/commands/completion.py` & `borgmatic-1.7.9/borgmatic/commands/completion.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/commands/convert_config.py` & `borgmatic-1.7.9/borgmatic/commands/convert_config.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/commands/generate_config.py` & `borgmatic-1.7.9/borgmatic/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/commands/validate_config.py` & `borgmatic-1.7.9/borgmatic/commands/validate_config.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/config/collect.py` & `borgmatic-1.7.9/borgmatic/config/collect.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/config/convert.py` & `borgmatic-1.7.9/borgmatic/config/convert.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/config/environment.py` & `borgmatic-1.7.9/borgmatic/config/environment.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/config/generate.py` & `borgmatic-1.7.9/borgmatic/config/generate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/config/legacy.py` & `borgmatic-1.7.9/borgmatic/config/legacy.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/config/load.py` & `borgmatic-1.7.9/borgmatic/config/load.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/config/normalize.py` & `borgmatic-1.7.9/borgmatic/config/normalize.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/config/override.py` & `borgmatic-1.7.9/borgmatic/config/override.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/config/schema.yaml` & `borgmatic-1.7.9/borgmatic/config/schema.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -365,29 +365,29 @@
                 additionalProperties: false
                 properties:
                     init:
                         type: string
                         description: |
                           Extra command-line options to pass to "borg init".
                         example: "--extra-option"
+                    create:
+                        type: string
+                        description: |
+                          Extra command-line options to pass to "borg create".
+                        example: "--extra-option"
                     prune:
                         type: string
                         description: |
                           Extra command-line options to pass to "borg prune".
                         example: "--extra-option"
                     compact:
                         type: string
                         description: |
                           Extra command-line options to pass to "borg compact".
                         example: "--extra-option"
-                    create:
-                        type: string
-                        description: |
-                          Extra command-line options to pass to "borg create".
-                        example: "--extra-option"
                     check:
                         type: string
                         description: |
                           Extra command-line options to pass to "borg check".
                         example: "--extra-option"
                 description: |
                     Additional options to pass directly to particular Borg
@@ -659,19 +659,19 @@
                     - echo "Finished actions."
             on_error:
                 type: array
                 items:
                     type: string
                 description: |
                     List of one or more shell commands or scripts to execute
-                    when an exception occurs during a "prune", "compact",
-                    "create", or "check" action or an associated before/after
+                    when an exception occurs during a "create", "prune",
+                    "compact", or "check" action or an associated before/after
                     hook.
                 example:
-                    - echo "Error during prune/compact/create/check."
+                    - echo "Error during create/prune/compact/check."
             before_everything:
                 type: array
                 items:
                     type: string
                 description: |
                     List of one or more shell commands or scripts to execute
                     before running all actions (if one of them is "create").
@@ -937,14 +937,39 @@
                     List of one or more MySQL/MariaDB databases to dump before
                     creating a backup, run once per configuration file. The
                     database dumps are added to your source directories at
                     runtime, backed up, and removed afterwards. Requires
                     mysqldump/mysql commands (from either MySQL or MariaDB). See
                     https://dev.mysql.com/doc/refman/8.0/en/mysqldump.html or
                     https://mariadb.com/kb/en/library/mysqldump/ for details.
+            sqlite_databases:
+                type: array
+                items:
+                    type: object
+                    required: ['path','name']
+                    additionalProperties: false
+                    properties:
+                        name:
+                            type: string
+                            description: |
+                                This is used to tag the database dump file
+                                with a name. It is not the path to the database
+                                file itself. The name "all" has no special
+                                meaning for SQLite databases.
+                            example: users
+                        path:
+                            type: string
+                            description: |
+                                Path to the SQLite database file to dump. If
+                                relative, it is relative to the current working
+                                directory. Note that using this
+                                database hook implicitly enables both
+                                read_special and one_file_system (see above) to
+                                support dump and restore streaming.
+                            example: /var/lib/sqlite/users.db
             mongodb_databases:
                 type: array
                 items:
                     type: object
                     required: ['name']
                     additionalProperties: false
                     properties:
@@ -1139,27 +1164,28 @@
                 required: ['ping_url']
                 additionalProperties: false
                 properties:
                     ping_url:
                         type: string
                         description: |
                             Healthchecks ping URL or UUID to notify when a
-                            backup begins, ends, or errors.
+                            backup begins, ends, errors or just to send logs.
                         example: https://hc-ping.com/your-uuid-here
                     verify_tls:
                         type: boolean
                         description: |
                             Verify the TLS certificate of the ping URL host.
                             Defaults to true.
                         example: false
                     send_logs:
                         type: boolean
                         description: |
                             Send borgmatic logs to Healthchecks as part the
-                            "finish" state. Defaults to true.
+                            "finish", "fail", and "log" states. Defaults to
+                            true.
                         example: false
                     ping_body_limit:
                         type: integer
                         description: |
                             Number of bytes of borgmatic logs to send to
                             Healthchecks, ideally the same as PING_BODY_LIMIT
                             configured on the Healthchecks server. Set to 0 to
@@ -1170,18 +1196,19 @@
                         type: array
                         items:
                             type: string
                             enum:
                                 - start
                                 - finish
                                 - fail
+                                - log
                             uniqueItems: true
                         description: |
                             List of one or more monitoring states to ping for:
-                            "start", "finish", and/or "fail". Defaults to
+                            "start", "finish", "fail", and/or "log". Defaults to
                             pinging for all states.
                         example:
                             - finish
                 description: |
                     Configuration for a monitoring integration with
                     Healthchecks. Create an account at https://healthchecks.io
                     (or self-host Healthchecks) if you'd like to use this
```

### Comparing `borgmatic-1.7.8/borgmatic/config/validate.py` & `borgmatic-1.7.9/borgmatic/config/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,9 +182,9 @@
             for config in configurations.values()
             for config_repository in config['location']['repositories']
         )
     )
 
     if count != 1:
         raise ValueError(
-            'Can\'t determine which repository to use. Use --repository to disambiguate'
+            "Can't determine which repository to use. Use --repository to disambiguate"
         )
```

### Comparing `borgmatic-1.7.8/borgmatic/execute.py` & `borgmatic-1.7.9/borgmatic/execute.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/hooks/command.py` & `borgmatic-1.7.9/borgmatic/hooks/command.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/hooks/cronhub.py` & `borgmatic-1.7.9/borgmatic/hooks/cronhub.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 
 
 def ping_monitor(hook_config, config_filename, state, monitoring_log_level, dry_run):
     '''
     Ping the configured Cronhub URL, modified with the monitor.State. Use the given configuration
     filename in any log entries. If this is a dry run, then don't actually ping anything.
     '''
+    if state not in MONITOR_STATE_TO_CRONHUB:
+        logger.debug(
+            f'{config_filename}: Ignoring unsupported monitoring {state.name.lower()} in Cronhub hook'
+        )
+        return
+
     dry_run_label = ' (dry run; not actually pinging)' if dry_run else ''
     formatted_state = '/{}/'.format(MONITOR_STATE_TO_CRONHUB[state])
     ping_url = (
         hook_config['ping_url']
         .replace('/start/', formatted_state)
         .replace('/ping/', formatted_state)
     )
```

### Comparing `borgmatic-1.7.8/borgmatic/hooks/cronitor.py` & `borgmatic-1.7.9/borgmatic/hooks/cronitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 
 
 def ping_monitor(hook_config, config_filename, state, monitoring_log_level, dry_run):
     '''
     Ping the configured Cronitor URL, modified with the monitor.State. Use the given configuration
     filename in any log entries. If this is a dry run, then don't actually ping anything.
     '''
+    if state not in MONITOR_STATE_TO_CRONITOR:
+        logger.debug(
+            f'{config_filename}: Ignoring unsupported monitoring {state.name.lower()} in Cronitor hook'
+        )
+        return
+
     dry_run_label = ' (dry run; not actually pinging)' if dry_run else ''
     ping_url = '{}/{}'.format(hook_config['ping_url'], MONITOR_STATE_TO_CRONITOR[state])
 
     logger.info(
         '{}: Pinging Cronitor {}{}'.format(config_filename, state.name.lower(), dry_run_label)
     )
     logger.debug('{}: Using Cronitor ping URL {}'.format(config_filename, ping_url))
```

### Comparing `borgmatic-1.7.8/borgmatic/hooks/dispatch.py` & `borgmatic-1.7.9/borgmatic/hooks/dispatch.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,29 @@
     cronitor,
     healthchecks,
     mongodb,
     mysql,
     ntfy,
     pagerduty,
     postgresql,
+    sqlite,
 )
 
 logger = logging.getLogger(__name__)
 
 HOOK_NAME_TO_MODULE = {
     'cronhub': cronhub,
     'cronitor': cronitor,
     'healthchecks': healthchecks,
     'mongodb_databases': mongodb,
     'mysql_databases': mysql,
     'ntfy': ntfy,
     'pagerduty': pagerduty,
     'postgresql_databases': postgresql,
+    'sqlite_databases': sqlite,
 }
 
 
 def call_hook(function_name, hooks, log_prefix, hook_name, *args, **kwargs):
     '''
     Given the hooks configuration dict and a prefix to use in log entries, call the requested
     function of the Python module corresponding to the given hook name. Supply that call with the
```

### Comparing `borgmatic-1.7.8/borgmatic/hooks/dump.py` & `borgmatic-1.7.9/borgmatic/hooks/dump.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 import os
 import shutil
 
 from borgmatic.borg.state import DEFAULT_BORGMATIC_SOURCE_DIRECTORY
 
 logger = logging.getLogger(__name__)
 
-DATABASE_HOOK_NAMES = ('postgresql_databases', 'mysql_databases', 'mongodb_databases')
+DATABASE_HOOK_NAMES = (
+    'postgresql_databases',
+    'mysql_databases',
+    'mongodb_databases',
+    'sqlite_databases',
+)
 
 
 def make_database_dump_path(borgmatic_source_directory, database_hook_name):
     '''
     Given a borgmatic source directory (or None) and a database hook name, construct a database dump
     path.
     '''
```

### Comparing `borgmatic-1.7.8/borgmatic/hooks/healthchecks.py` & `borgmatic-1.7.9/borgmatic/hooks/healthchecks.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 logger = logging.getLogger(__name__)
 
 MONITOR_STATE_TO_HEALTHCHECKS = {
     monitor.State.START: 'start',
     monitor.State.FINISH: None,  # Healthchecks doesn't append to the URL for the finished state.
     monitor.State.FAIL: 'fail',
+    monitor.State.LOG: 'log',
 }
 
 PAYLOAD_TRUNCATION_INDICATOR = '...\n'
 DEFAULT_PING_BODY_LIMIT_BYTES = 100000
 
 
 class Forgetful_buffering_handler(logging.Handler):
@@ -113,15 +114,15 @@
         ping_url = '{}/{}'.format(ping_url, healthchecks_state)
 
     logger.info(
         '{}: Pinging Healthchecks {}{}'.format(config_filename, state.name.lower(), dry_run_label)
     )
     logger.debug('{}: Using Healthchecks ping URL {}'.format(config_filename, ping_url))
 
-    if state in (monitor.State.FINISH, monitor.State.FAIL):
+    if state in (monitor.State.FINISH, monitor.State.FAIL, monitor.State.LOG):
         payload = format_buffered_logs_for_payload()
     else:
         payload = ''
 
     if not dry_run:
         logging.getLogger('urllib3').setLevel(logging.ERROR)
         try:
```

### Comparing `borgmatic-1.7.8/borgmatic/hooks/mongodb.py` & `borgmatic-1.7.9/borgmatic/hooks/mongodb.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/hooks/mysql.py` & `borgmatic-1.7.9/borgmatic/hooks/mysql.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/hooks/ntfy.py` & `borgmatic-1.7.9/borgmatic/hooks/ntfy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 import logging
 
 import requests
 
-from borgmatic.hooks import monitor
-
 logger = logging.getLogger(__name__)
 
-MONITOR_STATE_TO_NTFY = {
-    monitor.State.START: None,
-    monitor.State.FINISH: None,
-    monitor.State.FAIL: None,
-}
-
 
 def initialize_monitor(
     ping_url, config_filename, monitoring_log_level, dry_run
 ):  # pragma: no cover
     '''
     No initialization is necessary for this monitor.
     '''
```

### Comparing `borgmatic-1.7.8/borgmatic/hooks/pagerduty.py` & `borgmatic-1.7.9/borgmatic/hooks/pagerduty.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/hooks/postgresql.py` & `borgmatic-1.7.9/borgmatic/hooks/postgresql.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/logger.py` & `borgmatic-1.7.9/borgmatic/logger.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/signals.py` & `borgmatic-1.7.9/borgmatic/signals.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic/verbosity.py` & `borgmatic-1.7.9/borgmatic/verbosity.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/borgmatic.egg-info/PKG-INFO` & `borgmatic-1.7.9/borgmatic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borgmatic
-Version: 1.7.8
+Version: 1.7.9
 Summary: Simple, configuration-driven backup software for servers and workstations
 Home-page: https://torsion.org/borgmatic
 Author: Dan Helfman
 Author-email: witten@torsion.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
```

### Comparing `borgmatic-1.7.8/borgmatic.egg-info/SOURCES.txt` & `borgmatic-1.7.9/borgmatic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .dockerignore
 .drone.yml
 .eleventy.js
+.flake8
 .gitignore
 AUTHORS
 LICENSE
 MANIFEST.in
 NEWS
 README.md
 SECURITY.md
@@ -92,14 +93,15 @@
 borgmatic/hooks/healthchecks.py
 borgmatic/hooks/mongodb.py
 borgmatic/hooks/monitor.py
 borgmatic/hooks/mysql.py
 borgmatic/hooks/ntfy.py
 borgmatic/hooks/pagerduty.py
 borgmatic/hooks/postgresql.py
+borgmatic/hooks/sqlite.py
 docs/Dockerfile
 docs/README.md
 docs/SECURITY.md
 docs/_data/layout.json
 docs/_includes/asciinema.css
 docs/_includes/header.njk
 docs/_includes/index.css
@@ -140,14 +142,15 @@
 docs/static/healthchecks.png
 docs/static/mariadb.png
 docs/static/mongodb.png
 docs/static/mysql.png
 docs/static/ntfy.png
 docs/static/pagerduty.png
 docs/static/postgresql.png
+docs/static/sqlite.png
 sample/cron/borgmatic
 sample/systemd/borgmatic.service
 sample/systemd/borgmatic.timer
 scripts/dev-docs
 scripts/find-unsupported-borg-options
 scripts/push
 scripts/release
@@ -242,8 +245,9 @@
 tests/unit/hooks/test_dispatch.py
 tests/unit/hooks/test_dump.py
 tests/unit/hooks/test_healthchecks.py
 tests/unit/hooks/test_mongodb.py
 tests/unit/hooks/test_mysql.py
 tests/unit/hooks/test_ntfy.py
 tests/unit/hooks/test_pagerduty.py
-tests/unit/hooks/test_postgresql.py
+tests/unit/hooks/test_postgresql.py
+tests/unit/hooks/test_sqlite.py
```

### Comparing `borgmatic-1.7.8/docs/Dockerfile` & `borgmatic-1.7.9/docs/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 FROM alpine:3.17.1 as borgmatic
 
 COPY . /app
 RUN apk add --no-cache py3-pip py3-ruamel.yaml py3-ruamel.yaml.clib
 RUN pip install --no-cache /app && generate-borgmatic-config && chmod +r /etc/borgmatic/config.yaml
 RUN borgmatic --help > /command-line.txt \
-    && for action in rcreate transfer prune compact create check extract export-tar mount umount restore rlist list rinfo info break-lock borg; do \
+    && for action in rcreate transfer create prune compact check extract export-tar mount umount restore rlist list rinfo info break-lock borg; do \
            echo -e "\n--------------------------------------------------------------------------------\n" >> /command-line.txt \
            && borgmatic "$action" --help >> /command-line.txt; done
 
 FROM node:19.5.0-alpine as html
 
 ARG ENVIRONMENT=production
```

### Comparing `borgmatic-1.7.8/docs/README.md` & `borgmatic-1.7.9/docs/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -63,29 +63,30 @@
 
 ## Integrations
 
 <a href="https://www.postgresql.org/"><img src="docs/static/postgresql.png" alt="PostgreSQL" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://www.mysql.com/"><img src="docs/static/mysql.png" alt="MySQL" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://mariadb.com/"><img src="docs/static/mariadb.png" alt="MariaDB" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://www.mongodb.com/"><img src="docs/static/mongodb.png" alt="MongoDB" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
+<a href="https://sqlite.org/"><img src="docs/static/sqlite.png" alt="SQLite" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://healthchecks.io/"><img src="docs/static/healthchecks.png" alt="Healthchecks" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://cronitor.io/"><img src="docs/static/cronitor.png" alt="Cronitor" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://cronhub.io/"><img src="docs/static/cronhub.png" alt="Cronhub" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://www.pagerduty.com/"><img src="docs/static/pagerduty.png" alt="PagerDuty" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://ntfy.sh/"><img src="docs/static/ntfy.png" alt="ntfy" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href="https://www.borgbase.com/?utm_source=borgmatic"><img src="docs/static/borgbase.png" alt="BorgBase" height="60px" style="margin-bottom:20px;"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 
 
 ## Getting started
 
 Your first step is to [install and configure
 borgmatic](https://torsion.org/borgmatic/docs/how-to/set-up-backups/).
 
-For additional documentation, check out the links above for <a
-href="https://torsion.org/borgmatic/#documentation">borgmatic how-to and
+For additional documentation, check out the links above (left panel on wide screens)
+for <a href="https://torsion.org/borgmatic/#documentation">borgmatic how-to and
 reference guides</a>.
 
 
 ## Hosting providers
 
 Need somewhere to store your encrypted off-site backups? The following hosting
 providers include specific support for Borg/borgmatic—and fund borgmatic
```

#### html2text {}

```diff
@@ -13,23 +13,24 @@
 frequency: 2 weeks hooks: # Custom preparation scripts to run. before_backup: -
 prepare-for-backup.sh # Databases to dump and include in backups.
 postgresql_databases: - name: users # Third-party services to notify you if
 backups aren't happening. healthchecks: https://hc-ping.com/be067061-cf96-4412-
 8eae-62b0c50d6a8c ``` Want to see borgmatic in action? Check out the
 screencast. [https://asciinema.org/a/203761.png] borgmatic is powered by [Borg
 Backup](https://www.borgbackup.org/). ## Integrations [PostgreSQL]     
-[MySQL]      [MariaDB]      [MongoDB]      [Healthchecks]      [Cronitor]     
-[Cronhub]      [PagerDuty]      [ntfy]      [BorgBase]      ## Getting started
-Your first step is to [install and configure borgmatic](https://torsion.org/
-borgmatic/docs/how-to/set-up-backups/). For additional documentation, check out
-the links above for borgmatic_how-to_and_reference_guides. ## Hosting providers
-Need somewhere to store your encrypted off-site backups? The following hosting
-providers include specific support for Borg/borgmaticâand fund borgmatic
-development and hosting when you use these links to sign up. (These are
-referral links, but without any tracking scripts or cookies.)
+[MySQL]      [MariaDB]      [MongoDB]      [SQLite]      [Healthchecks]     
+[Cronitor]      [Cronhub]      [PagerDuty]      [ntfy]      [BorgBase]      ##
+Getting started Your first step is to [install and configure borgmatic](https:/
+/torsion.org/borgmatic/docs/how-to/set-up-backups/). For additional
+documentation, check out the links above (left panel on wide screens) for
+borgmatic_how-to_and_reference_guides. ## Hosting providers Need somewhere to
+store your encrypted off-site backups? The following hosting providers include
+specific support for Borg/borgmaticâand fund borgmatic development and
+hosting when you use these links to sign up. (These are referral links, but
+without any tracking scripts or cookies.)
     * BorgBase: Borg hosting service with support for monitoring, 2FA, and
       append-only repos
 Additionally, [rsync.net](https://www.rsync.net/products/borg.html) and
 [Hetzner](https://www.hetzner.com/storage/storage-box) have compatible storage
 offerings, but do not currently fund borgmatic development or hosting. ##
 Support and contributing ### Issues Are you experiencing an issue with
 borgmatic? Or do you have an idea for a feature enhancement? Head on over to
```

### Comparing `borgmatic-1.7.8/docs/SECURITY.md` & `borgmatic-1.7.9/docs/SECURITY.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/_includes/components/info-blocks.css` & `borgmatic-1.7.9/docs/_includes/components/info-blocks.css`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/_includes/components/lists.css` & `borgmatic-1.7.9/docs/_includes/components/lists.css`

 * *Files 11% similar despite different names*

```diff
@@ -59,19 +59,14 @@
 		content: " ";
 		border-left: 1px solid rgba(255,255,255,.8);
 		position: absolute;
 		left: -2px;
 		top: -2px;
 		bottom: 2px;
 	}
-	@media (prefers-color-scheme: dark) {
-		.inlinelist .inlinelist-item code:before {
-			border-left-color: rgba(0,0,0,.8);
-		}
-	}
 }
 a.buzzword {
 	text-decoration: underline;
 }
 .buzzword-list a,
 .inlinelist a {
 	text-decoration: none;
@@ -87,34 +82,17 @@
 		display: inline-block;
 	}
 }
 .buzzword-list li,
 .buzzword {
 	background-color: #f7f7f7;
 }
-@media (prefers-color-scheme: dark) {
-	.buzzword-list li,
-	.buzzword {
-		background-color: #080808;
-	}
-}
 .inlinelist .inlinelist-item {
 	background-color: #e9e9e9;
 }
-@media (prefers-color-scheme: dark) {
-	.inlinelist .inlinelist-item {
-		background-color: #000;
-	}
-	.inlinelist .inlinelist-item a {
-		color: #fff;
-	}
-	.inlinelist .inlinelist-item code {
-		color: inherit;
-	}
-}
 .inlinelist .inlinelist-item:hover,
 .inlinelist .inlinelist-item:focus,
 .buzzword-list li:hover,
 .buzzword-list li:focus,
 .buzzword:hover,
 .buzzword:focus,
 .rainbow-active:hover,
@@ -213,20 +191,14 @@
 	justify-content: center;
 	background-color: #dff7ff;
 	border-radius: 50%;
 	width: 1.75em;
 	height: 1.75em;
 	font-weight: 600;
 }
-@media (prefers-color-scheme: dark) {
-	.numberflag {
-		background-color: #00bcd4;
-		color: #222;
-	}
-}
 h1 .numberflag,
 h2 .numberflag,
 h3 .numberflag,
 h4 .numberflag,
 h5 .numberflag {
 	width: 1.25em;
 	height: 1.25em;
@@ -240,19 +212,14 @@
 	position: absolute;
 	bottom: -1px;
 	left: 0;
 	height: 1px;
 	background-color: #fff;
 	width: calc(100% + 0.4em); /* 16px /40 */
 }
-@media (prefers-color-scheme: dark) {
-	h2 .numberflag:after {
-		background-color: #222;
-	}
-}
 
 /* Super featured list on home page */
 .list-superfeatured .avatar {
 	width: calc(30px + 5vw);
 	height: calc(30px + 5vw);
 	max-width: 60px;
 	max-height: 60px;
```

### Comparing `borgmatic-1.7.8/docs/_includes/components/minilink.css` & `borgmatic-1.7.9/docs/_includes/components/minilink.css`

 * *Files 17% similar despite different names*

```diff
@@ -8,40 +8,24 @@
 	background-color: #ddd;
 	border-radius: 0.1875em; /* 3px /16 */
 	font-weight: 500;
 	margin: 0 0.4285714285714em 0.07142857142857em 0; /* 0 6px 1px 0 /14 */
 	line-height: 1.285714285714; /* 18px /14 */
 	font-family: system-ui, -apple-system, sans-serif;
 }
-@media (prefers-color-scheme: dark) {
-  .minilink {
-    background-color: #222;
-    /*
-      !important to override .elv-callout a
-      see _includes/components/callout.css
-     */
-    color: #fff !important;
-  }
-}
 table .minilink {
 	margin-top: 6px;
 }
 .minilink[href] {
 	box-shadow: 0 1px 1px 0 rgba(0,0,0,.5);
 }
 .minilink[href]:hover,
 .minilink[href]:focus {
 	background-color: #bbb;
 }
-@media (prefers-color-scheme: dark) {
-  .minilink[href]:hover,
-  .minilink[href]:focus {
-    background-color: #444;
-  }
-}
 pre + .minilink {
 	color: #fff;
 	border-radius: 0 0 0.2857142857143em 0.2857142857143em; /* 4px /14 */
 	float: right;
 	background-color: #444;
 	color: #fff;
 }
@@ -70,19 +54,14 @@
 	clear: both;
 }
 
 .minilink-addedin {
 	text-transform: none;
 	box-shadow: 0 0 0 1px rgba(0,0,0,0.3);
 }
-@media (prefers-color-scheme: dark) {
-  .minilink-addedin {
-    box-shadow: 0 0 0 1px rgba(255,255,255,0.3);
-  }
-}
 .minilink-addedin:not(:first-child) {
 	margin-left: .5em;
 }
 .minilink-addedin.minilink-inline {
 	margin: 0 4px;
 	background-color: #fff;
 }
```

### Comparing `borgmatic-1.7.8/docs/_includes/components/toc.css` & `borgmatic-1.7.9/docs/_includes/components/toc.css`

 * *Files 9% similar despite different names*

```diff
@@ -75,30 +75,19 @@
 /* Top level links */
 .elv-toc-list > li > a {
 	color: #222;
 	font-weight: 600;
 	border-bottom: 1px solid #ddd;
 	margin-bottom: 0.25em; /* 4px /16 */
 }
-@media (prefers-color-scheme: dark) {
-  .elv-toc-list > li > a {
-    color: #fff;
-    border-color: #444;
-  }
-}
 
 /* Active links */
 .elv-toc-list li.elv-toc-active > a {
 	background-color: #dff7ff;
 }
-@media (prefers-color-scheme: dark) {
-  .elv-toc-list li.elv-toc-active > a {
-    background-color: #353535;
-  }
-}
 .elv-toc-list ul .elv-toc-active > a:after {
 	content: "";
 }
 
 /* Show only active nested lists */
 .elv-toc-list ul.elv-toc-active,
 .elv-toc-list li.elv-toc-active > ul {
```

### Comparing `borgmatic-1.7.8/docs/_includes/index.css` & `borgmatic-1.7.9/docs/_includes/index.css`

 * *Files 1% similar despite different names*

```diff
@@ -281,19 +281,14 @@
 .elv-header-docs:after {
 	clear: both;
 }
 /* Header Hero */
 .elv-hero {
 	background-color: #222;
 }
-@media (prefers-color-scheme: dark) {
-	.elv-hero {
-		background-color: #292929;
-	}
-}
 .elv-hero img,
 .elv-hero svg {
 	width: 42.95774646vh;
 	height: 60vh;
 }
 .elv-hero:hover img,
 .elv-hero:hover svg {
```

### Comparing `borgmatic-1.7.8/docs/_includes/layouts/base.njk` & `borgmatic-1.7.9/docs/_includes/layouts/base.njk`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/_includes/layouts/main.njk` & `borgmatic-1.7.9/docs/_includes/layouts/main.njk`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/_includes/prism-theme.css` & `borgmatic-1.7.9/docs/_includes/prism-theme.css`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/how-to/add-preparation-and-cleanup-steps-to-backups.md` & `borgmatic-1.7.9/docs/how-to/add-preparation-and-cleanup-steps-to-backups.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/how-to/backup-to-a-removable-drive-or-an-intermittent-server.md` & `borgmatic-1.7.9/docs/how-to/backup-to-a-removable-drive-or-an-intermittent-server.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/how-to/backup-your-databases.md` & `borgmatic-1.7.9/docs/how-to/backup-your-databases.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,44 @@
 systems to backup an exported database dump, rather than backing up your
 database's internal file storage. That's because the internal storage can
 change while you're reading from it. In contrast, a database dump creates a
 consistent snapshot that is more suited for backups.
 
 Fortunately, borgmatic includes built-in support for creating database dumps
 prior to running backups. For example, here is everything you need to dump and
-backup a couple of local PostgreSQL databases, a MySQL/MariaDB database, and a
-MongoDB database:
+backup a couple of local PostgreSQL databases and a MySQL/MariaDB database.
 
 ```yaml
 hooks:
     postgresql_databases:
         - name: users
         - name: orders
     mysql_databases:
         - name: posts
+```
+
+<span class="minilink minilink-addedin">New in version 1.5.22</span> You can
+also dump MongoDB databases. For example:
+
+```yaml
+hooks:
     mongodb_databases:
         - name: messages
 ```
 
+<span class="minilink minilink-addedin">New in version 1.7.9</span>
+Additionally, you can dump SQLite databases. For example:
+
+```yaml
+hooks:
+    sqlite_databases:
+        - name: mydb
+          path: /var/lib/sqlite3/mydb.sqlite
+```
+
 As part of each backup, borgmatic streams a database dump for each configured
 database directly to Borg, so it's included in the backup without consuming
 additional disk space. (The exceptions are the PostgreSQL/MongoDB "directory"
 dump formats, which can't stream and therefore do consume temporary disk
 space. Additionally, prior to borgmatic 1.5.3, all database dumps consumed
 temporary disk space.)
 
@@ -70,14 +86,17 @@
         - name: messages
           hostname: database4.example.org
           port: 27018
           username: dbuser
           password: trustsome1
           authentication_database: mongousers
           options: "--ssl"
+    sqlite_databases:
+        - name: mydb
+          path: /var/lib/sqlite3/mydb.sqlite
 ```
 
 See your [borgmatic configuration
 file](https://torsion.org/borgmatic/docs/reference/configuration/) for
 additional customization of the options passed to database commands (when
 listing databases, restoring databases, etc.).
 
@@ -95,14 +114,16 @@
     mongodb_databases:
         - name: all
 ```
 
 Note that you may need to use a `username` of the `postgres` superuser for
 this to work with PostgreSQL.
 
+The SQLite hook in particular does not consider "all" a special database name.
+
 <span class="minilink minilink-addedin">New in version 1.7.6</span> With
 PostgreSQL and MySQL, you can optionally dump "all" databases to separate
 files instead of one combined dump file, allowing more convenient restores of
 individual databases. Enable this by specifying your desired database dump
 `format`:
 
 ```yaml
@@ -150,19 +171,19 @@
 to prepare for this situation, it's a good idea to include borgmatic's own
 configuration files as part of your regular backups. That way, you can always
 bring back any missing configuration files in order to restore a database.
 
 
 ## Supported databases
 
-As of now, borgmatic supports PostgreSQL, MySQL/MariaDB, and MongoDB databases
-directly. But see below about general-purpose preparation and cleanup hooks as
-a work-around with other database systems. Also, please [file a
-ticket](https://torsion.org/borgmatic/#issues) for additional database systems
-that you'd like supported.
+As of now, borgmatic supports PostgreSQL, MySQL/MariaDB, MongoDB, and SQLite
+databases directly. But see below about general-purpose preparation and
+cleanup hooks as a work-around with other database systems. Also, please [file
+a ticket](https://torsion.org/borgmatic/#issues) for additional database
+systems that you'd like supported.
 
 
 ## Database restoration
 
 To restore a database dump from an archive, use the `borgmatic restore`
 action. But the first step is to figure out which archive to restore from. A
 good way to do that is to use the `rlist` action:
@@ -291,15 +312,18 @@
 borgmatic extracts the dump file into the *`username`*`/.borgmatic/` directory
 within the extraction destination path, where *`username`* is the user that
 created the backup. For example, if you created the backup with the `root`
 user and you're extracting to `/tmp`, then the dump will be in
 `/tmp/root/.borgmatic`.
 
 After extraction, you can manually restore the dump file using native database
-commands like `pg_restore`, `mysql`, `mongorestore` or similar.
+commands like `pg_restore`, `mysql`, `mongorestore`, `sqlite`, or similar.
+
+Also see the documentation on [listing database
+dumps](https://torsion.org/borgmatic/docs/how-to/inspect-your-backups/#listing-database-dumps).
 
 
 ## Preparation and cleanup hooks
 
 If this database integration is too limited for needs, borgmatic also supports
 general-purpose [preparation and cleanup
 hooks](https://torsion.org/borgmatic/docs/how-to/add-preparation-and-cleanup-steps-to-backups/).
```

### Comparing `borgmatic-1.7.8/docs/how-to/deal-with-very-large-backups.md` & `borgmatic-1.7.9/docs/how-to/deal-with-very-large-backups.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,45 +5,55 @@
   parent: How-to guides
   order: 4
 ---
 ## Biggish data
 
 Borg itself is great for efficiently de-duplicating data across successive
 backup archives, even when dealing with very large repositories. But you may
-find that while borgmatic's default mode of `prune`, `compact`, `create`, and
-`check` works well on small repositories, it's not so great on larger ones.
-That's because running the default pruning, compact, and consistency checks
-take a long time on large repositories.
+find that while borgmatic's default actions of `create`, `prune`, `compact`,
+and `check` works well on small repositories, it's not so great on larger
+ones. That's because running the default pruning, compact, and consistency
+checks take a long time on large repositories.
+
+<span class="minilink minilink-addedin">Prior to version 1.7.9</span> The
+default action ordering was `prune`, `compact`, `create`, and `check`.
 
 ### A la carte actions
 
-If you find yourself in this situation, you have some options. First, you can
-run borgmatic's `prune`, `compact`, `create`, or `check` actions separately.
-For instance, the following optional actions are available:
+If you find yourself wanting to customize the actions, you have some options.
+First, you can run borgmatic's `prune`, `compact`, `create`, or `check`
+actions separately. For instance, the following optional actions are
+available (among others):
 
 ```bash
+borgmatic create
 borgmatic prune
 borgmatic compact
-borgmatic create
 borgmatic check
 ```
 
-You can run with only one of these actions provided, or you can mix and match
-any number of them in a single borgmatic run. This supports approaches like
-skipping certain actions while running others. For instance, this skips
-`prune` and `compact` and only runs `create` and `check`:
+You can run borgmatic with only one of these actions provided, or you can mix
+and match any number of them in a single borgmatic run. This supports
+approaches like skipping certain actions while running others. For instance,
+this skips `prune` and `compact` and only runs `create` and `check`:
 
 ```bash
 borgmatic create check
 ```
 
-Or, you can make backups with `create` on a frequent schedule (e.g. with
-`borgmatic create` called from one cron job), while only running expensive
-consistency checks with `check` on a much less frequent basis (e.g. with
-`borgmatic check` called from a separate cron job).
+<span class="minilink minilink-addedin">New in version 1.7.9</span> borgmatic
+now respects your specified command-line action order, running actions in the
+order you specify. In previous versions, borgmatic ran your specified actions
+in a fixed ordering regardless of the order they appeared on the command-line.
+
+But instead of running actions together, another option is to run backups with
+`create` on a frequent schedule (e.g. with `borgmatic create` called from one
+cron job), while only running expensive consistency checks with `check` on a
+much less frequent basis (e.g. with `borgmatic check` called from a separate
+cron job).
 
 
 ### Consistency check configuration
 
 Another option is to customize your consistency checks. By default, if you
 omit consistency checks from configuration, borgmatic runs full-repository
 checks (`repository`) and per-archive checks (`archives`) within each
```

### Comparing `borgmatic-1.7.8/docs/how-to/develop-on-borgmatic.md` & `borgmatic-1.7.9/docs/how-to/develop-on-borgmatic.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 Then, install borgmatic
 "[editable](https://pip.pypa.io/en/stable/cli/pip_install/#editable-installs)"
 so that you can run borgmatic commands while you're hacking on them to
 make sure your changes work.
 
 ```bash
 cd borgmatic/
-pip3 install --editable --user .
+pip3 install --user --editable .
 ```
 
 Note that this will typically install the borgmatic commands into
 `~/.local/bin`, which may or may not be on your PATH. There are other ways to
 install borgmatic editable as well, for instance into the system Python
 install (so without `--user`, as root), or even into a
 [virtualenv](https://virtualenv.pypa.io/en/stable/). How or where you install
```

### Comparing `borgmatic-1.7.8/docs/how-to/extract-a-backup.md` & `borgmatic-1.7.9/docs/how-to/extract-a-backup.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 ```
 
 (No borgmatic `rlist` action? Try `list` instead or upgrade borgmatic!)
 
 That should yield output looking something like:
 
 ```text
-host-2019-01-01T04:05:06.070809      Tue, 2019-01-01 04:05:06 [...]
-host-2019-01-02T04:06:07.080910      Wed, 2019-01-02 04:06:07 [...]
+host-2023-01-01T04:05:06.070809      Tue, 2023-01-01 04:05:06 [...]
+host-2023-01-02T04:06:07.080910      Wed, 2023-01-02 04:06:07 [...]
 ```
 
 Assuming that you want to extract the archive with the most up-to-date files
 and therefore the latest timestamp, run a command like:
 
 ```bash
-borgmatic extract --archive host-2019-01-02T04:06:07.080910
+borgmatic extract --archive host-2023-01-02T04:06:07.080910
 ```
 
 (No borgmatic `extract` action? Upgrade borgmatic!)
 
 Or simplify this to:
 
 ```bash
@@ -50,15 +50,15 @@
 If you have a single repository in your borgmatic configuration file(s), no
 problem: the `extract` action figures out which repository to use.
 
 But if you have multiple repositories configured, then you'll need to specify
 the repository path containing the archive to extract. Here's an example:
 
 ```bash
-borgmatic extract --repository repo.borg --archive host-2019-...
+borgmatic extract --repository repo.borg --archive host-2023-...
 ```
 
 ## Extract particular files
 
 Sometimes, you want to extract a single deleted file, rather than extracting
 everything from an archive. To do that, tack on one or more `--path` values.
 For instance:
@@ -70,14 +70,21 @@
 Note that the specified restore paths should not have a leading slash. Like a
 whole-archive extract, this also extracts into the current directory by
 default. So for example, if you happen to be in the directory `/var` and you
 run the `extract` command above, borgmatic will extract `/var/path/1` and
 `/var/path/2`.
 
 
+### Searching for files
+
+If you're not sure which archive contains the files you're looking for, you
+can [search across
+archives](https://torsion.org/borgmatic/docs/how-to/inspect-your-backups/#searching-for-a-file).
+
+
 ## Extract to a particular destination
 
 By default, borgmatic extracts files into the current directory. To instead
 extract files to a particular destination directory, use the `--destination`
 flag:
 
 ```bash
```

### Comparing `borgmatic-1.7.8/docs/how-to/inspect-your-backups.md` & `borgmatic-1.7.9/docs/how-to/inspect-your-backups.md`

 * *Files 8% similar despite different names*

```diff
@@ -87,14 +87,27 @@
 filtering archives such as `--last`, `--archive`, `--match-archives`, etc. For
 example, to search only the last five archives:
 
 ```bash
 borgmatic list --find foo.txt --last 5
 ```
 
+## Listing database dumps
+
+If you have enabled borgmatic's [database
+hooks](https://torsion.org/borgmatic/docs/how-to/backup-your-databases/), you
+can list backed up database dumps via borgmatic. For example:
+
+```bash 
+borgmatic list --archive latest --find .borgmatic/*_databases
+```
+
+This gives you a listing of all database dump files contained in the latest
+archive, complete with file sizes.
+
 
 ## Logging
 
 By default, borgmatic logs to a local syslog-compatible daemon if one is
 present and borgmatic is running in a non-interactive console. Where those
 logs show up depends on your particular system. If you're using systemd, try
 running `journalctl -xe`. Otherwise, try viewing `/var/log/syslog` or
```

### Comparing `borgmatic-1.7.8/docs/how-to/make-backups-redundant.md` & `borgmatic-1.7.9/docs/how-to/make-backups-redundant.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/how-to/make-per-application-backups.md` & `borgmatic-1.7.9/docs/how-to/make-per-application-backups.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/how-to/monitor-your-backups.md` & `borgmatic-1.7.9/docs/how-to/monitor-your-backups.md`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 checks](https://torsion.org/borgmatic/docs/how-to/deal-with-very-large-backups/#consistency-check-configuration)
 or even script full [extract
 tests](https://torsion.org/borgmatic/docs/how-to/extract-a-backup/).
 
 
 ## Error hooks
 
-When an error occurs during a `prune`, `compact`, `create`, or `check` action,
+When an error occurs during a `create`, `prune`, `compact`, or `check` action,
 borgmatic can run configurable shell commands to fire off custom error
 notifications or take other actions, so you can get alerted as soon as
 something goes wrong. Here's a not-so-useful example:
 
 ```yaml
 hooks:
     on_error:
@@ -112,16 +112,16 @@
    error occurred
  * `repository`: path of the repository in which the error occurred (may be
    blank if the error occurs in a hook)
  * `error`: the error message itself
  * `output`: output of the command that failed (may be blank if an error
    occurred without running a command)
 
-Note that borgmatic runs the `on_error` hooks only for `prune`, `compact`,
-`create`, or `check` actions or hooks in which an error occurs, and not other
+Note that borgmatic runs the `on_error` hooks only for `create`, `prune`,
+`compact`, or `check` actions or hooks in which an error occurs, and not other
 actions. borgmatic does not run `on_error` hooks if an error occurs within a
 `before_everything` or `after_everything` hook. For more about hooks, see the
 [borgmatic hooks
 documentation](https://torsion.org/borgmatic/docs/how-to/add-preparation-and-cleanup-steps-to-backups/),
 especially the security information.
 
 
@@ -140,26 +140,26 @@
         ping_url: https://hc-ping.com/addffa72-da17-40ae-be9c-ff591afb942a
 ```
 
 With this hook in place, borgmatic pings your Healthchecks project when a
 backup begins, ends, or errors. Specifically, after the <a
 href="https://torsion.org/borgmatic/docs/how-to/add-preparation-and-cleanup-steps-to-backups/">`before_backup`
 hooks</a> run, borgmatic lets Healthchecks know that it has started if any of
-the `prune`, `compact`, `create`, or `check` actions are run.
+the `create`, `prune`, `compact`, or `check` actions are run.
 
 Then, if the actions complete successfully, borgmatic notifies Healthchecks of
 the success after the `after_backup` hooks run, and includes borgmatic logs in
 the payload data sent to Healthchecks. This means that borgmatic logs show up
 in the Healthchecks UI, although be aware that Healthchecks currently has a
 10-kilobyte limit for the logs in each ping.
 
 If an error occurs during any action or hook, borgmatic notifies Healthchecks
 after the `on_error` hooks run, also tacking on logs including the error
-itself. But the logs are only included for errors that occur when a `prune`,
-`compact`, `create`, or `check` action is run.
+itself. But the logs are only included for errors that occur when a `create`,
+`prune`, `compact`, or `check` action is run.
 
 You can customize the verbosity of the logs that are sent to Healthchecks with
 borgmatic's `--monitoring-verbosity` flag. The `--list` and `--stats` flags
 may also be of use. See `borgmatic create --help` for more information.
 Additionally, see the [borgmatic configuration
 file](https://torsion.org/borgmatic/docs/reference/configuration/) for
 additional Healthchecks options.
```

### Comparing `borgmatic-1.7.8/docs/how-to/provide-your-passwords.md` & `borgmatic-1.7.9/docs/how-to/provide-your-passwords.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/how-to/run-arbitrary-borg-commands.md` & `borgmatic-1.7.9/docs/how-to/run-arbitrary-borg-commands.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/how-to/set-up-backups.md` & `borgmatic-1.7.9/docs/how-to/set-up-backups.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/how-to/upgrade.md` & `borgmatic-1.7.9/docs/how-to/upgrade.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/static/borgbase.png` & `borgmatic-1.7.9/docs/static/borgbase.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/static/borgmatic.png` & `borgmatic-1.7.9/docs/static/borgmatic.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/static/borgmatic.svg` & `borgmatic-1.7.9/docs/static/borgmatic.svg`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/static/cronhub.png` & `borgmatic-1.7.9/docs/static/cronhub.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/static/cronitor.png` & `borgmatic-1.7.9/docs/static/cronitor.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/static/healthchecks.png` & `borgmatic-1.7.9/docs/static/healthchecks.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/static/mariadb.png` & `borgmatic-1.7.9/docs/static/mariadb.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/static/mongodb.png` & `borgmatic-1.7.9/docs/static/mongodb.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/static/mysql.png` & `borgmatic-1.7.9/docs/static/mysql.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/static/ntfy.png` & `borgmatic-1.7.9/docs/static/ntfy.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/static/pagerduty.png` & `borgmatic-1.7.9/docs/static/pagerduty.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/docs/static/postgresql.png` & `borgmatic-1.7.9/docs/static/postgresql.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/sample/systemd/borgmatic.service` & `borgmatic-1.7.9/sample/systemd/borgmatic.service`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/scripts/find-unsupported-borg-options` & `borgmatic-1.7.9/scripts/find-unsupported-borg-options`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/scripts/release` & `borgmatic-1.7.9/scripts/release`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 version=$(head --lines=1 NEWS)
 
 if [[ $version =~ .*dev* ]]; then
     echo "Refusing to release a dev version: $version"
     exit 1
 fi
 
-#if ! git diff-index --quiet HEAD -- ; then
-#    echo "Refusing to release with local changes:"
-#    git status --porcelain
-#    exit 1
-#fi
+if ! git diff-index --quiet HEAD -- ; then
+    echo "Refusing to release with local changes:"
+    git status --porcelain
+    exit 1
+fi
 
 git tag $version
 git push origin $version
 git push github $version
 
 # Build borgmatic and publish to pypi.
 rm -fr dist
```

### Comparing `borgmatic-1.7.8/scripts/run-full-dev-tests` & `borgmatic-1.7.9/scripts/run-full-dev-tests`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/scripts/run-full-tests` & `borgmatic-1.7.9/scripts/run-full-tests`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # For more information, see:
 # https://torsion.org/borgmatic/docs/how-to/develop-on-borgmatic/
 
 set -e
 
 apk add --no-cache python3 py3-pip borgbackup postgresql-client mariadb-client mongodb-tools \
-    py3-ruamel.yaml py3-ruamel.yaml.clib bash
+    py3-ruamel.yaml py3-ruamel.yaml.clib bash sqlite
 # If certain dependencies of black are available in this version of Alpine, install them.
 apk add --no-cache py3-typed-ast py3-regex || true
 python3 -m pip install --no-cache --upgrade pip==22.2.2 setuptools==64.0.1
 pip3 install --ignore-installed tox==3.25.1
 export COVERAGE_FILE=/tmp/.coverage
 tox --workdir /tmp/.tox --sitepackages
 tox --workdir /tmp/.tox --sitepackages -e end-to-end
```

### Comparing `borgmatic-1.7.8/setup.py` & `borgmatic-1.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = '1.7.8'
+VERSION = '1.7.9'
 
 
 setup(
     name='borgmatic',
     version=VERSION,
     description='Simple, configuration-driven backup software for servers and workstations',
     author='Dan Helfman',
```

### Comparing `borgmatic-1.7.8/test_requirements.txt` & `borgmatic-1.7.9/test_requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 appdirs==1.4.4; python_version >= '3.8'
 attrs==20.3.0; python_version >= '3.8'
 black==19.10b0; python_version >= '3.8'
 click==7.1.2; python_version >= '3.8'
 colorama==0.4.4
 coverage==5.3
 flake8==4.0.1
+flake8-quotes==3.3.2
 flexmock==0.10.4
 isort==5.9.1
 mccabe==0.6.1
 pluggy==0.13.1
 pathspec==0.8.1; python_version >= '3.8'
 py==1.10.0
 pycodestyle==2.8.0
```

### Comparing `borgmatic-1.7.8/tests/end-to-end/docker-compose.yaml` & `borgmatic-1.7.9/tests/end-to-end/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/end-to-end/test_borgmatic.py` & `borgmatic-1.7.9/tests/end-to-end/test_borgmatic.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/end-to-end/test_database.py` & `borgmatic-1.7.9/tests/end-to-end/test_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,17 @@
           password: test
           authentication_database: admin
           format: {mongodb_dump_format}
         - name: all
           hostname: mongodb
           username: root
           password: test
+    sqlite_databases:
+        - name: sqlite_test
+          path: /tmp/sqlite_test.db
 '''
 
     with open(config_path, 'w') as config_file:
         config_file.write(config)
 
 
 def test_database_dump_and_restore():
```

### Comparing `borgmatic-1.7.8/tests/end-to-end/test_generate_config.py` & `borgmatic-1.7.9/tests/end-to-end/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/end-to-end/test_override.py` & `borgmatic-1.7.9/tests/end-to-end/test_override.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/end-to-end/test_validate_config.py` & `borgmatic-1.7.9/tests/end-to-end/test_validate_config.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/integration/borg/test_feature.py` & `borgmatic-1.7.9/tests/integration/borg/test_feature.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/integration/commands/test_arguments.py` & `borgmatic-1.7.9/tests/integration/commands/test_arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,21 +250,14 @@
 
 def test_parse_arguments_allows_init_and_create():
     flexmock(module.collect).should_receive('get_default_config_paths').and_return(['default'])
 
     module.parse_arguments('--config', 'myconfig', 'init', '--encryption', 'repokey', 'create')
 
 
-def test_parse_arguments_disallows_repository_unless_action_consumes_it():
-    flexmock(module.collect).should_receive('get_default_config_paths').and_return(['default'])
-
-    with pytest.raises(SystemExit):
-        module.parse_arguments('--config', 'myconfig', '--repository', 'test.borg')
-
-
 def test_parse_arguments_allows_repository_with_extract():
     flexmock(module.collect).should_receive('get_default_config_paths').and_return(['default'])
 
     module.parse_arguments(
         '--config', 'myconfig', 'extract', '--repository', 'test.borg', '--archive', 'test'
     )
```

### Comparing `borgmatic-1.7.8/tests/integration/commands/test_convert_config.py` & `borgmatic-1.7.9/tests/integration/commands/test_convert_config.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/integration/commands/test_generate_config.py` & `borgmatic-1.7.9/tests/integration/commands/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/integration/commands/test_validate_config.py` & `borgmatic-1.7.9/tests/integration/commands/test_validate_config.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/integration/config/test_generate.py` & `borgmatic-1.7.9/tests/integration/config/test_generate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/integration/config/test_legacy.py` & `borgmatic-1.7.9/tests/integration/config/test_legacy.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/integration/config/test_load.py` & `borgmatic-1.7.9/tests/integration/config/test_load.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/integration/config/test_override.py` & `borgmatic-1.7.9/tests/integration/config/test_override.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/integration/config/test_validate.py` & `borgmatic-1.7.9/tests/integration/config/test_validate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/integration/hooks/test_healthchecks.py` & `borgmatic-1.7.9/tests/integration/hooks/test_healthchecks.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/integration/test_execute.py` & `borgmatic-1.7.9/tests/integration/test_execute.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/actions/test_borg.py` & `borgmatic-1.7.9/tests/unit/actions/test_borg.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/actions/test_break_lock.py` & `borgmatic-1.7.9/tests/unit/actions/test_break_lock.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/actions/test_compact.py` & `borgmatic-1.7.9/tests/unit/actions/test_compact.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,76 @@
 from flexmock import flexmock
 
 from borgmatic.actions import compact as module
 
 
-def test_compact_actions_calls_hooks():
+def test_compact_actions_calls_hooks_for_configured_repository():
     flexmock(module.logger).answer = lambda message: None
     flexmock(module.borgmatic.borg.feature).should_receive('available').and_return(True)
-    flexmock(module.borgmatic.borg.compact).should_receive('compact_segments')
+    flexmock(module.borgmatic.config.validate).should_receive('repositories_match').never()
+    flexmock(module.borgmatic.borg.compact).should_receive('compact_segments').once()
     flexmock(module.borgmatic.hooks.command).should_receive('execute_hook').times(2)
     compact_arguments = flexmock(
-        progress=flexmock(), cleanup_commits=flexmock(), threshold=flexmock()
+        repository=None, progress=flexmock(), cleanup_commits=flexmock(), threshold=flexmock()
+    )
+    global_arguments = flexmock(monitoring_verbosity=1, dry_run=False)
+
+    module.run_compact(
+        config_filename='test.yaml',
+        repository='repo',
+        storage={},
+        retention={},
+        hooks={},
+        hook_context={},
+        local_borg_version=None,
+        compact_arguments=compact_arguments,
+        global_arguments=global_arguments,
+        dry_run_label='',
+        local_path=None,
+        remote_path=None,
+    )
+
+
+def test_compact_runs_with_selected_repository():
+    flexmock(module.logger).answer = lambda message: None
+    flexmock(module.borgmatic.config.validate).should_receive(
+        'repositories_match'
+    ).once().and_return(True)
+    flexmock(module.borgmatic.borg.feature).should_receive('available').and_return(True)
+    flexmock(module.borgmatic.borg.compact).should_receive('compact_segments').once()
+    compact_arguments = flexmock(
+        repository=flexmock(), progress=flexmock(), cleanup_commits=flexmock(), threshold=flexmock()
+    )
+    global_arguments = flexmock(monitoring_verbosity=1, dry_run=False)
+
+    module.run_compact(
+        config_filename='test.yaml',
+        repository='repo',
+        storage={},
+        retention={},
+        hooks={},
+        hook_context={},
+        local_borg_version=None,
+        compact_arguments=compact_arguments,
+        global_arguments=global_arguments,
+        dry_run_label='',
+        local_path=None,
+        remote_path=None,
+    )
+
+
+def test_compact_bails_if_repository_does_not_match():
+    flexmock(module.logger).answer = lambda message: None
+    flexmock(module.borgmatic.borg.feature).should_receive('available').and_return(True)
+    flexmock(module.borgmatic.config.validate).should_receive(
+        'repositories_match'
+    ).once().and_return(False)
+    flexmock(module.borgmatic.borg.compact).should_receive('compact_segments').never()
+    compact_arguments = flexmock(
+        repository=flexmock(), progress=flexmock(), cleanup_commits=flexmock(), threshold=flexmock()
     )
     global_arguments = flexmock(monitoring_verbosity=1, dry_run=False)
 
     module.run_compact(
         config_filename='test.yaml',
         repository='repo',
         storage={},
```

### Comparing `borgmatic-1.7.8/tests/unit/actions/test_export_tar.py` & `borgmatic-1.7.9/tests/unit/actions/test_export_tar.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/actions/test_extract.py` & `borgmatic-1.7.9/tests/unit/actions/test_extract.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/actions/test_info.py` & `borgmatic-1.7.9/tests/unit/actions/test_info.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/actions/test_list.py` & `borgmatic-1.7.9/tests/unit/actions/test_list.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/actions/test_mount.py` & `borgmatic-1.7.9/tests/unit/actions/test_mount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/actions/test_rcreate.py` & `borgmatic-1.7.9/tests/unit/actions/test_rcreate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/actions/test_restore.py` & `borgmatic-1.7.9/tests/unit/actions/test_restore.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/actions/test_rinfo.py` & `borgmatic-1.7.9/tests/unit/actions/test_rinfo.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/actions/test_rlist.py` & `borgmatic-1.7.9/tests/unit/actions/test_rlist.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/actions/test_transfer.py` & `borgmatic-1.7.9/tests/unit/actions/test_transfer.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_borg.py` & `borgmatic-1.7.9/tests/unit/borg/test_borg.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_break_lock.py` & `borgmatic-1.7.9/tests/unit/borg/test_break_lock.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_check.py` & `borgmatic-1.7.9/tests/unit/borg/test_check.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_compact.py` & `borgmatic-1.7.9/tests/unit/borg/test_compact.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_create.py` & `borgmatic-1.7.9/tests/unit/borg/test_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1912,15 +1912,15 @@
     flexmock(module.logger).should_receive('warning').twice()
     flexmock(module).should_receive('make_pattern_flags').and_return(())
     flexmock(module).should_receive('make_exclude_flags').and_return(())
     flexmock(module.flags).should_receive('make_repository_archive_flags').and_return(
         (f'repo::{DEFAULT_ARCHIVE_NAME}',)
     )
     flexmock(module.environment).should_receive('make_environment')
-    flexmock(module).should_receive('collect_special_file_paths').and_return(("/dev/null",))
+    flexmock(module).should_receive('collect_special_file_paths').and_return(('/dev/null',))
     create_command = (
         'borg',
         'create',
         '--one-file-system',
         '--read-special',
     ) + REPO_ARCHIVE_WITH_PATHS
     flexmock(module).should_receive('execute_command_with_processes').with_args(
```

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_environment.py` & `borgmatic-1.7.9/tests/unit/borg/test_environment.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_export_tar.py` & `borgmatic-1.7.9/tests/unit/borg/test_export_tar.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_extract.py` & `borgmatic-1.7.9/tests/unit/borg/test_extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -308,14 +308,65 @@
         location_config={},
         storage_config={},
         local_borg_version='1.2.3',
         strip_components=5,
     )
 
 
+def test_extract_archive_calls_borg_with_strip_components_calculated_from_all():
+    flexmock(module.os.path).should_receive('abspath').and_return('repo')
+    insert_execute_command_mock(
+        (
+            'borg',
+            'extract',
+            '--strip-components',
+            '2',
+            'repo::archive',
+            'foo/bar/baz.txt',
+            'foo/bar.txt',
+        )
+    )
+    flexmock(module.feature).should_receive('available').and_return(True)
+    flexmock(module.flags).should_receive('make_repository_archive_flags').and_return(
+        ('repo::archive',)
+    )
+
+    module.extract_archive(
+        dry_run=False,
+        repository='repo',
+        archive='archive',
+        paths=['foo/bar/baz.txt', 'foo/bar.txt'],
+        location_config={},
+        storage_config={},
+        local_borg_version='1.2.3',
+        strip_components='all',
+    )
+
+
+def test_extract_archive_with_strip_components_all_and_no_paths_raises():
+    flexmock(module.os.path).should_receive('abspath').and_return('repo')
+    flexmock(module.feature).should_receive('available').and_return(True)
+    flexmock(module.flags).should_receive('make_repository_archive_flags').and_return(
+        ('repo::archive',)
+    )
+    flexmock(module).should_receive('execute_command').never()
+
+    with pytest.raises(ValueError):
+        module.extract_archive(
+            dry_run=False,
+            repository='repo',
+            archive='archive',
+            paths=None,
+            location_config={},
+            storage_config={},
+            local_borg_version='1.2.3',
+            strip_components='all',
+        )
+
+
 def test_extract_archive_calls_borg_with_progress_parameter():
     flexmock(module.os.path).should_receive('abspath').and_return('repo')
     flexmock(module.environment).should_receive('make_environment')
     flexmock(module).should_receive('execute_command').with_args(
         ('borg', 'extract', '--progress', 'repo::archive'),
         output_file=module.DO_NOT_CAPTURE,
         working_directory=None,
```

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_flags.py` & `borgmatic-1.7.9/tests/unit/borg/test_flags.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_info.py` & `borgmatic-1.7.9/tests/unit/borg/test_info.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_list.py` & `borgmatic-1.7.9/tests/unit/borg/test_list.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_mount.py` & `borgmatic-1.7.9/tests/unit/borg/test_mount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_prune.py` & `borgmatic-1.7.9/tests/unit/borg/test_prune.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_rcreate.py` & `borgmatic-1.7.9/tests/unit/borg/test_rcreate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_rinfo.py` & `borgmatic-1.7.9/tests/unit/borg/test_rinfo.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_rlist.py` & `borgmatic-1.7.9/tests/unit/borg/test_rlist.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_transfer.py` & `borgmatic-1.7.9/tests/unit/borg/test_transfer.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_umount.py` & `borgmatic-1.7.9/tests/unit/borg/test_umount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/borg/test_version.py` & `borgmatic-1.7.9/tests/unit/borg/test_version.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/commands/test_arguments.py` & `borgmatic-1.7.9/tests/unit/commands/test_arguments.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import collections
+
 from flexmock import flexmock
 
 from borgmatic.commands import arguments as module
 
 
 def test_parse_subparser_arguments_consumes_subparser_arguments_before_subparser_name():
     action_namespace = flexmock(foo=True)
@@ -66,14 +68,34 @@
         ('action', '--foo', 'true', 'other', '--bar', '3'), subparsers
     )
 
     assert arguments == {'action': action_namespace, 'other': other_namespace}
     assert remaining_arguments == []
 
 
+def test_parse_subparser_arguments_respects_command_line_action_ordering():
+    other_namespace = flexmock()
+    action_namespace = flexmock(foo=True)
+    subparsers = {
+        'action': flexmock(
+            parse_known_args=lambda arguments: (action_namespace, ['action', '--foo', 'true'])
+        ),
+        'other': flexmock(parse_known_args=lambda arguments: (other_namespace, ['other'])),
+    }
+
+    arguments, remaining_arguments = module.parse_subparser_arguments(
+        ('other', '--foo', 'true', 'action'), subparsers
+    )
+
+    assert arguments == collections.OrderedDict(
+        [('other', other_namespace), ('action', action_namespace)]
+    )
+    assert remaining_arguments == []
+
+
 def test_parse_subparser_arguments_applies_default_subparsers():
     prune_namespace = flexmock()
     compact_namespace = flexmock()
     create_namespace = flexmock(progress=True)
     check_namespace = flexmock()
     subparsers = {
         'prune': flexmock(
```

### Comparing `borgmatic-1.7.8/tests/unit/commands/test_borgmatic.py` & `borgmatic-1.7.9/tests/unit/commands/test_borgmatic.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 def test_run_configuration_logs_monitor_start_error():
     flexmock(module).should_receive('verbosity_to_log_level').and_return(logging.INFO)
     flexmock(module.borg_version).should_receive('local_borg_version').and_return(flexmock())
     flexmock(module.dispatch).should_receive('call_hooks').and_raise(OSError).and_return(
         None
-    ).and_return(None)
+    ).and_return(None).and_return(None)
     expected_results = [flexmock()]
     flexmock(module).should_receive('log_error_records').and_return(expected_results)
     flexmock(module).should_receive('run_actions').never()
     config = {'location': {'repositories': ['foo']}}
     arguments = {'global': flexmock(monitoring_verbosity=1, dry_run=False), 'create': flexmock()}
 
     results = list(module.run_configuration('test.yaml', config, arguments))
@@ -95,15 +95,15 @@
     arguments = {'global': flexmock(monitoring_verbosity=1, dry_run=False), 'create': flexmock()}
 
     results = list(module.run_configuration('test.yaml', config, arguments))
 
     assert results == []
 
 
-def test_run_configuration_logs_monitor_finish_error():
+def test_run_configuration_logs_monitor_log_error():
     flexmock(module).should_receive('verbosity_to_log_level').and_return(logging.INFO)
     flexmock(module.borg_version).should_receive('local_borg_version').and_return(flexmock())
     flexmock(module.dispatch).should_receive('call_hooks').and_return(None).and_return(
         None
     ).and_raise(OSError)
     expected_results = [flexmock()]
     flexmock(module).should_receive('log_error_records').and_return(expected_results)
@@ -112,15 +112,15 @@
     arguments = {'global': flexmock(monitoring_verbosity=1, dry_run=False), 'create': flexmock()}
 
     results = list(module.run_configuration('test.yaml', config, arguments))
 
     assert results == expected_results
 
 
-def test_run_configuration_bails_for_monitor_finish_soft_failure():
+def test_run_configuration_bails_for_monitor_log_soft_failure():
     flexmock(module).should_receive('verbosity_to_log_level').and_return(logging.INFO)
     flexmock(module.borg_version).should_receive('local_borg_version').and_return(flexmock())
     error = subprocess.CalledProcessError(borgmatic.hooks.command.SOFT_FAIL_EXIT_CODE, 'try again')
     flexmock(module.dispatch).should_receive('call_hooks').and_return(None).and_return(
         None
     ).and_raise(error)
     flexmock(module).should_receive('log_error_records').never()
@@ -130,14 +130,49 @@
     arguments = {'global': flexmock(monitoring_verbosity=1, dry_run=False), 'create': flexmock()}
 
     results = list(module.run_configuration('test.yaml', config, arguments))
 
     assert results == []
 
 
+def test_run_configuration_logs_monitor_finish_error():
+    flexmock(module).should_receive('verbosity_to_log_level').and_return(logging.INFO)
+    flexmock(module.borg_version).should_receive('local_borg_version').and_return(flexmock())
+    flexmock(module.dispatch).should_receive('call_hooks').and_return(None).and_return(
+        None
+    ).and_return(None).and_raise(OSError)
+    expected_results = [flexmock()]
+    flexmock(module).should_receive('log_error_records').and_return(expected_results)
+    flexmock(module).should_receive('run_actions').and_return([])
+    config = {'location': {'repositories': ['foo']}}
+    arguments = {'global': flexmock(monitoring_verbosity=1, dry_run=False), 'create': flexmock()}
+
+    results = list(module.run_configuration('test.yaml', config, arguments))
+
+    assert results == expected_results
+
+
+def test_run_configuration_bails_for_monitor_finish_soft_failure():
+    flexmock(module).should_receive('verbosity_to_log_level').and_return(logging.INFO)
+    flexmock(module.borg_version).should_receive('local_borg_version').and_return(flexmock())
+    error = subprocess.CalledProcessError(borgmatic.hooks.command.SOFT_FAIL_EXIT_CODE, 'try again')
+    flexmock(module.dispatch).should_receive('call_hooks').and_return(None).and_return(
+        None
+    ).and_raise(None).and_raise(error)
+    flexmock(module).should_receive('log_error_records').never()
+    flexmock(module).should_receive('run_actions').and_return([])
+    flexmock(module.command).should_receive('considered_soft_failure').and_return(True)
+    config = {'location': {'repositories': ['foo']}}
+    arguments = {'global': flexmock(monitoring_verbosity=1, dry_run=False), 'create': flexmock()}
+
+    results = list(module.run_configuration('test.yaml', config, arguments))
+
+    assert results == []
+
+
 def test_run_configuration_logs_on_error_hook_error():
     flexmock(module).should_receive('verbosity_to_log_level').and_return(logging.INFO)
     flexmock(module.borg_version).should_receive('local_borg_version').and_return(flexmock())
     flexmock(module.command).should_receive('execute_hook').and_raise(OSError)
     expected_results = [flexmock(), flexmock()]
     flexmock(module).should_receive('log_error_records').and_return(
         expected_results[:1]
@@ -397,80 +432,80 @@
             remote_path=flexmock(),
             local_borg_version=flexmock(),
             repository_path='repo',
         )
     )
 
 
-def test_run_actions_runs_prune():
+def test_run_actions_runs_create():
     flexmock(module).should_receive('add_custom_log_levels')
     flexmock(module.command).should_receive('execute_hook')
-    flexmock(borgmatic.actions.prune).should_receive('run_prune').once()
+    expected = flexmock()
+    flexmock(borgmatic.actions.create).should_receive('run_create').and_yield(expected).once()
 
-    tuple(
+    result = tuple(
         module.run_actions(
-            arguments={'global': flexmock(dry_run=False), 'prune': flexmock()},
+            arguments={'global': flexmock(dry_run=False), 'create': flexmock()},
             config_filename=flexmock(),
             location={'repositories': []},
             storage=flexmock(),
             retention=flexmock(),
             consistency=flexmock(),
             hooks={},
             local_path=flexmock(),
             remote_path=flexmock(),
             local_borg_version=flexmock(),
             repository_path='repo',
         )
     )
+    assert result == (expected,)
 
 
-def test_run_actions_runs_compact():
+def test_run_actions_runs_prune():
     flexmock(module).should_receive('add_custom_log_levels')
     flexmock(module.command).should_receive('execute_hook')
-    flexmock(borgmatic.actions.compact).should_receive('run_compact').once()
+    flexmock(borgmatic.actions.prune).should_receive('run_prune').once()
 
     tuple(
         module.run_actions(
-            arguments={'global': flexmock(dry_run=False), 'compact': flexmock()},
+            arguments={'global': flexmock(dry_run=False), 'prune': flexmock()},
             config_filename=flexmock(),
             location={'repositories': []},
             storage=flexmock(),
             retention=flexmock(),
             consistency=flexmock(),
             hooks={},
             local_path=flexmock(),
             remote_path=flexmock(),
             local_borg_version=flexmock(),
             repository_path='repo',
         )
     )
 
 
-def test_run_actions_runs_create():
+def test_run_actions_runs_compact():
     flexmock(module).should_receive('add_custom_log_levels')
     flexmock(module.command).should_receive('execute_hook')
-    expected = flexmock()
-    flexmock(borgmatic.actions.create).should_receive('run_create').and_yield(expected).once()
+    flexmock(borgmatic.actions.compact).should_receive('run_compact').once()
 
-    result = tuple(
+    tuple(
         module.run_actions(
-            arguments={'global': flexmock(dry_run=False), 'create': flexmock()},
+            arguments={'global': flexmock(dry_run=False), 'compact': flexmock()},
             config_filename=flexmock(),
             location={'repositories': []},
             storage=flexmock(),
             retention=flexmock(),
             consistency=flexmock(),
             hooks={},
             local_path=flexmock(),
             remote_path=flexmock(),
             local_borg_version=flexmock(),
             repository_path='repo',
         )
     )
-    assert result == (expected,)
 
 
 def test_run_actions_runs_check_when_repository_enabled_for_checks():
     flexmock(module).should_receive('add_custom_log_levels')
     flexmock(module.command).should_receive('execute_hook')
     flexmock(module.checks).should_receive('repository_enabled_for_checks').and_return(True)
     flexmock(borgmatic.actions.check).should_receive('run_check').once()
@@ -732,14 +767,41 @@
             config_filename=flexmock(),
             location={'repositories': []},
             storage=flexmock(),
             retention=flexmock(),
             consistency=flexmock(),
             hooks={},
             local_path=flexmock(),
+            remote_path=flexmock(),
+            local_borg_version=flexmock(),
+            repository_path='repo',
+        )
+    )
+
+
+def test_run_actions_runs_multiple_actions_in_argument_order():
+    flexmock(module).should_receive('add_custom_log_levels')
+    flexmock(module.command).should_receive('execute_hook')
+    flexmock(borgmatic.actions.borg).should_receive('run_borg').once().ordered()
+    flexmock(borgmatic.actions.restore).should_receive('run_restore').once().ordered()
+
+    tuple(
+        module.run_actions(
+            arguments={
+                'global': flexmock(dry_run=False),
+                'borg': flexmock(),
+                'restore': flexmock(),
+            },
+            config_filename=flexmock(),
+            location={'repositories': []},
+            storage=flexmock(),
+            retention=flexmock(),
+            consistency=flexmock(),
+            hooks={},
+            local_path=flexmock(),
             remote_path=flexmock(),
             local_borg_version=flexmock(),
             repository_path='repo',
         )
     )
```

### Comparing `borgmatic-1.7.8/tests/unit/config/test_checks.py` & `borgmatic-1.7.9/tests/unit/config/test_checks.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/config/test_collect.py` & `borgmatic-1.7.9/tests/unit/config/test_collect.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/config/test_convert.py` & `borgmatic-1.7.9/tests/unit/config/test_convert.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/config/test_environment.py` & `borgmatic-1.7.9/tests/unit/config/test_environment.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/config/test_generate.py` & `borgmatic-1.7.9/tests/unit/config/test_generate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/config/test_legacy.py` & `borgmatic-1.7.9/tests/unit/config/test_legacy.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/config/test_normalize.py` & `borgmatic-1.7.9/tests/unit/config/test_normalize.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/config/test_override.py` & `borgmatic-1.7.9/tests/unit/config/test_override.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/config/test_validate.py` & `borgmatic-1.7.9/tests/unit/config/test_validate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/hooks/test_command.py` & `borgmatic-1.7.9/tests/unit/hooks/test_command.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/hooks/test_cronhub.py` & `borgmatic-1.7.9/tests/unit/hooks/test_cronhub.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,7 +98,15 @@
     module.ping_monitor(
         hook_config,
         'config.yaml',
         module.monitor.State.START,
         monitoring_log_level=1,
         dry_run=False,
     )
+
+
+def test_ping_monitor_with_unsupported_monitoring_state():
+    hook_config = {'ping_url': 'https://example.com'}
+    flexmock(module.requests).should_receive('get').never()
+    module.ping_monitor(
+        hook_config, 'config.yaml', module.monitor.State.LOG, monitoring_log_level=1, dry_run=False,
+    )
```

### Comparing `borgmatic-1.7.8/tests/unit/hooks/test_cronitor.py` & `borgmatic-1.7.9/tests/unit/hooks/test_cronitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,7 +83,15 @@
     module.ping_monitor(
         hook_config,
         'config.yaml',
         module.monitor.State.START,
         monitoring_log_level=1,
         dry_run=False,
     )
+
+
+def test_ping_monitor_with_unsupported_monitoring_state():
+    hook_config = {'ping_url': 'https://example.com'}
+    flexmock(module.requests).should_receive('get').never()
+    module.ping_monitor(
+        hook_config, 'config.yaml', module.monitor.State.LOG, monitoring_log_level=1, dry_run=False,
+    )
```

### Comparing `borgmatic-1.7.8/tests/unit/hooks/test_dispatch.py` & `borgmatic-1.7.9/tests/unit/hooks/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/hooks/test_dump.py` & `borgmatic-1.7.9/tests/unit/hooks/test_dump.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/hooks/test_healthchecks.py` & `borgmatic-1.7.9/tests/unit/hooks/test_healthchecks.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,31 @@
         'config.yaml',
         state=module.monitor.State.FAIL,
         monitoring_log_level=1,
         dry_run=False,
     )
 
 
+def test_ping_monitor_hits_ping_url_for_log_state():
+    hook_config = {'ping_url': 'https://example.com'}
+    payload = 'data'
+    flexmock(module).should_receive('format_buffered_logs_for_payload').and_return(payload)
+    flexmock(module.requests).should_receive('post').with_args(
+        'https://example.com/log', data=payload.encode('utf'), verify=True
+    ).and_return(flexmock(ok=True))
+
+    module.ping_monitor(
+        hook_config,
+        'config.yaml',
+        state=module.monitor.State.LOG,
+        monitoring_log_level=1,
+        dry_run=False,
+    )
+
+
 def test_ping_monitor_with_ping_uuid_hits_corresponding_url():
     hook_config = {'ping_url': 'abcd-efgh-ijkl-mnop'}
     payload = 'data'
     flexmock(module).should_receive('format_buffered_logs_for_payload').and_return(payload)
     flexmock(module.requests).should_receive('post').with_args(
         'https://hc-ping.com/{}'.format(hook_config['ping_url']),
         data=payload.encode('utf-8'),
```

### Comparing `borgmatic-1.7.8/tests/unit/hooks/test_mongodb.py` & `borgmatic-1.7.9/tests/unit/hooks/test_mongodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 def test_dump_databases_runs_mongodump_with_username_and_password():
     databases = [
         {
             'name': 'foo',
             'username': 'mongo',
             'password': 'trustsome1',
-            'authentication_database': "admin",
+            'authentication_database': 'admin',
         }
     ]
     process = flexmock()
     flexmock(module).should_receive('make_dump_path').and_return('')
     flexmock(module.dump).should_receive('make_database_dump_filename').and_return(
         'databases/localhost/foo'
     )
```

### Comparing `borgmatic-1.7.8/tests/unit/hooks/test_mysql.py` & `borgmatic-1.7.9/tests/unit/hooks/test_mysql.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/hooks/test_pagerduty.py` & `borgmatic-1.7.9/tests/unit/hooks/test_pagerduty.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/hooks/test_postgresql.py` & `borgmatic-1.7.9/tests/unit/hooks/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/test_execute.py` & `borgmatic-1.7.9/tests/unit/test_execute.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/test_logger.py` & `borgmatic-1.7.9/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/test_signals.py` & `borgmatic-1.7.9/tests/unit/test_signals.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tests/unit/test_verbosity.py` & `borgmatic-1.7.9/tests/unit/test_verbosity.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.7.8/tox.ini` & `borgmatic-1.7.9/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tox]
-envlist = py37,py38,py39,py310
+envlist = py37,py38,py39,py310,py311
 skip_missing_interpreters = True
 skipsdist = True
 minversion = 3.14.1
 
 [testenv]
 usedevelop = True
 deps = -rtest_requirements.txt
 whitelist_externals = 
     find
     sh
 passenv = COVERAGE_FILE
 commands =
     pytest {posargs}
-    py38,py39,py310: black --check .
+    py38,py39,py310,py311: black --check .
     isort --check-only --settings-path setup.cfg .
     flake8 borgmatic tests
 
 [testenv:black]
 commands =
     black {posargs} .
```

