# Comparing `tmp/vit-2.2.0b1.tar.gz` & `tmp/vit-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/hunmonk/git/vit/dist/tmpl1rg5fjv/vit-2.2.0b1.tar", last modified: Fri Nov 26 20:22:25 2021, max compression
+gzip compressed data, was "vit-2.3.0.tar", last modified: Fri Apr 14 04:27:09 2023, max compression
```

## Comparing `vit-2.2.0b1.tar` & `vit-2.3.0.tar`

### file list

```diff
@@ -1,185 +1,186 @@
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2021-11-26 20:22:25.000000 vit-2.2.0b1/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      856 2020-12-24 03:52:45.000000 vit-2.2.0b1/AUTHORS.md
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2034 2020-12-24 03:52:45.000000 vit-2.2.0b1/COLOR.md
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     7080 2021-11-04 13:51:45.000000 vit-2.2.0b1/CUSTOMIZE.md
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2118 2020-12-24 03:52:45.000000 vit-2.2.0b1/DEVELOPMENT.md
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1763 2020-12-24 03:52:45.000000 vit-2.2.0b1/INSTALL.md
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1070 2020-12-24 03:52:45.000000 vit-2.2.0b1/LICENSE
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      299 2020-12-24 03:52:45.000000 vit-2.2.0b1/MANIFEST.in
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2950 2021-11-26 20:22:25.000000 vit-2.2.0b1/PKG-INFO
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1985 2021-11-04 13:51:57.000000 vit-2.2.0b1/README.md
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      104 2021-02-28 21:10:00.000000 vit-2.2.0b1/pyproject.toml
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       56 2021-11-04 13:51:45.000000 vit-2.2.0b1/requirements.txt
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2021-11-26 20:22:25.000000 vit-2.2.0b1/scripts/
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2021-11-26 20:22:25.000000 vit-2.2.0b1/scripts/bash/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      153 2020-12-24 03:52:45.000000 vit-2.2.0b1/scripts/bash/vit.bash_completion
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       38 2021-11-26 20:22:25.000000 vit-2.2.0b1/setup.cfg
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1790 2021-11-26 19:52:16.000000 vit-2.2.0b1/setup.py
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2021-11-26 20:22:25.000000 vit-2.2.0b1/test/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        0 2020-12-24 03:52:45.000000 vit-2.2.0b1/test/__init__.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2934 2021-11-04 13:51:45.000000 vit-2.2.0b1/test/test_list_batcher.py
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2021-11-26 20:22:25.000000 vit-2.2.0b1/vit/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      194 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/__init__.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2507 2021-11-22 14:10:12.000000 vit-2.2.0b1/vit/action_manager.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     3842 2021-11-04 13:51:57.000000 vit-2.2.0b1/vit/actions.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    43597 2021-11-22 14:12:28.000000 vit-2.2.0b1/vit/application.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    11402 2021-11-04 13:51:45.000000 vit-2.2.0b1/vit/autocomplete.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5041 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/base_list_box.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    11636 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/color.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2491 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/color_mappings.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5474 2020-12-28 17:26:46.000000 vit-2.2.0b1/vit/command_bar.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      168 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/command_line.py
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2021-11-26 20:22:25.000000 vit-2.2.0b1/vit/config/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     9000 2021-11-04 13:51:57.000000 vit-2.2.0b1/vit/config/config.sample.ini
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    16323 2021-11-04 13:51:57.000000 vit-2.2.0b1/vit/config_parser.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      296 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/debug.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6442 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/denotation.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       36 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/env.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      503 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/event.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       92 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/exception.py
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2021-11-26 20:22:25.000000 vit-2.2.0b1/vit/formatter/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6662 2021-02-02 03:25:28.000000 vit-2.2.0b1/vit/formatter/__init__.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      342 2021-02-02 03:24:52.000000 vit-2.2.0b1/vit/formatter/depends.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      206 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/depends_count.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      224 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/depends_indicator.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       80 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/depends_list.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2436 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/description.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      100 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/description_combined.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      846 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/description_count.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      316 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/description_desc.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      637 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/description_oneline.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      442 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/description_truncated.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      677 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/description_truncated_count.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      253 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/due.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      125 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/due_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/due_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      129 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/due_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       69 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/due_formatted.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      125 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/due_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      131 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/due_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      135 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/due_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/due_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       66 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/end.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      116 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/end_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/end_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      120 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/end_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      116 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/end_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      122 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/end_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      126 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/end_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/end_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/entry.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/entry_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      140 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/entry_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      132 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/entry_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       77 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/entry_formatted.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/entry_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      134 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/entry_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      138 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/entry_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      140 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/entry_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       61 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/id.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       62 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/id_number.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6451 2021-10-19 13:36:03.000000 vit-2.2.0b1/vit/formatter/markers.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       71 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/modified.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      146 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/modified_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      158 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/modified_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      150 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/modified_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      146 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/modified_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      152 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/modified_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      156 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/modified_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      158 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/modified_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      140 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/parent.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       76 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/parent_long.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      190 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/parent_short.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1102 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/project.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       80 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/project_full.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      162 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/project_indented.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      301 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/project_parent.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/recur.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       76 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/recur_duration.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      178 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/recur_indicator.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      307 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/scheduled.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      161 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/scheduled_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      173 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/scheduled_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      165 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/scheduled_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       93 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/scheduled_formatted.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      161 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/scheduled_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      167 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/scheduled_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      171 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/scheduled_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      173 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/scheduled_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      275 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/start.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      202 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/start_active.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/start_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/start_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      141 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/start_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       77 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/start_formatted.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/start_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      143 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/start_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      147 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/start_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/start_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      312 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/status.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       76 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/status_long.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      139 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/status_short.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      736 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/tags.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      440 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/tags_count.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      275 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/tags_indicator.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/tags_list.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      771 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/uda_date.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      344 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/uda_duration.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      430 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/uda_indicator.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      363 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/uda_numeric.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      328 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/uda_string.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      271 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/until.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/until_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/until_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      141 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/until_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       77 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/until_formatted.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/until_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      143 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/until_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      147 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/until_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/until_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      135 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/urgency.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      152 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/urgency_integer.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       80 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/urgency_real.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       63 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/uuid.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/uuid_long.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      152 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/uuid_short.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       67 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/wait.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      122 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/wait_age.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      134 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/wait_countdown.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      126 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/wait_epoch.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      122 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/wait_iso.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/wait_julian.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      132 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/wait_relative.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      134 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/formatter/wait_remaining.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5342 2021-10-19 13:10:45.000000 vit-2.2.0b1/vit/formatter_base.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     7304 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/help.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2308 2020-12-30 19:07:59.000000 vit-2.2.0b1/vit/key_cache.py
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2021-11-26 20:22:25.000000 vit-2.2.0b1/vit/keybinding/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1573 2020-12-30 18:53:00.000000 vit-2.2.0b1/vit/keybinding/vi.ini
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6809 2020-12-30 19:10:59.000000 vit-2.2.0b1/vit/keybinding_parser.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1670 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/list_batcher.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1190 2021-11-04 13:51:45.000000 vit-2.2.0b1/vit/loader.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     3195 2021-04-24 00:12:31.000000 vit-2.2.0b1/vit/markers.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2050 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/multi_widget.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1674 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/option_parser.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2095 2021-11-04 13:51:45.000000 vit-2.2.0b1/vit/process.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5614 2021-11-04 13:51:45.000000 vit-2.2.0b1/vit/readline.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2002 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/registry.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5222 2021-11-04 13:51:57.000000 vit-2.2.0b1/vit/task.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    23336 2021-07-15 16:06:41.000000 vit-2.2.0b1/vit/task_list.py
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2021-11-26 20:22:25.000000 vit-2.2.0b1/vit/theme/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        0 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/theme/__init__.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      842 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/theme/classic.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      926 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/theme/default.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      410 2020-12-24 03:52:45.000000 vit-2.2.0b1/vit/uda.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1418 2021-11-04 13:51:45.000000 vit-2.2.0b1/vit/util.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       16 2021-11-26 19:57:31.000000 vit-2.2.0b1/vit/version.py
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      483 2021-11-04 13:51:45.000000 vit-2.2.0b1/vit/xdg.py
-drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2021-11-26 20:22:25.000000 vit-2.2.0b1/vit.egg-info/
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2950 2021-11-26 20:22:25.000000 vit-2.2.0b1/vit.egg-info/PKG-INFO
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     4435 2021-11-26 20:22:25.000000 vit-2.2.0b1/vit.egg-info/SOURCES.txt
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        1 2021-11-26 20:22:25.000000 vit-2.2.0b1/vit.egg-info/dependency_links.txt
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       47 2021-11-26 20:22:25.000000 vit-2.2.0b1/vit.egg-info/entry_points.txt
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        1 2019-09-28 15:34:44.000000 vit-2.2.0b1/vit.egg-info/not-zip-safe
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       56 2021-11-26 20:22:25.000000 vit-2.2.0b1/vit.egg-info/requires.txt
--rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        4 2021-11-26 20:22:25.000000 vit-2.2.0b1/vit.egg-info/top_level.txt
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.157355 vit-2.3.0/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      856 2020-12-24 03:52:45.000000 vit-2.3.0/AUTHORS.md
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2034 2020-12-24 03:52:45.000000 vit-2.3.0/COLOR.md
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     9309 2023-04-14 04:10:49.000000 vit-2.3.0/CUSTOMIZE.md
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     3048 2022-04-28 02:43:50.000000 vit-2.3.0/DEVELOPMENT.md
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1763 2020-12-24 03:52:45.000000 vit-2.3.0/INSTALL.md
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1070 2020-12-24 03:52:45.000000 vit-2.3.0/LICENSE
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      299 2020-12-24 03:52:45.000000 vit-2.3.0/MANIFEST.in
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2911 2023-04-14 04:27:09.153355 vit-2.3.0/PKG-INFO
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1985 2022-05-09 14:29:06.000000 vit-2.3.0/README.md
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      104 2021-02-28 21:10:00.000000 vit-2.3.0/pyproject.toml
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2022-04-17 22:57:32.000000 vit-2.3.0/requirements.txt
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.101356 vit-2.3.0/scripts/
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.109356 vit-2.3.0/scripts/bash/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      153 2020-12-24 03:52:45.000000 vit-2.3.0/scripts/bash/vit.bash_completion
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       38 2023-04-14 04:27:09.157355 vit-2.3.0/setup.cfg
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1823 2023-04-14 04:10:49.000000 vit-2.3.0/setup.py
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.109356 vit-2.3.0/test/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        0 2020-12-24 03:52:45.000000 vit-2.3.0/test/__init__.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2934 2021-11-04 13:51:45.000000 vit-2.3.0/test/test_list_batcher.py
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.117355 vit-2.3.0/vit/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      194 2020-12-24 03:52:45.000000 vit-2.3.0/vit/__init__.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2491 2023-04-14 04:10:49.000000 vit-2.3.0/vit/action_manager.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     3834 2023-04-14 04:10:49.000000 vit-2.3.0/vit/actions.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    45170 2023-04-14 04:10:49.000000 vit-2.3.0/vit/application.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    11394 2023-04-14 04:10:49.000000 vit-2.3.0/vit/autocomplete.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5154 2022-10-26 13:33:43.000000 vit-2.3.0/vit/base_list_box.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    12121 2023-04-14 04:10:49.000000 vit-2.3.0/vit/color.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2491 2020-12-24 03:52:45.000000 vit-2.3.0/vit/color_mappings.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5466 2023-04-14 04:10:49.000000 vit-2.3.0/vit/command_bar.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      168 2022-04-28 01:54:06.000000 vit-2.3.0/vit/command_line.py
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.121355 vit-2.3.0/vit/config/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     9749 2022-10-21 16:59:04.000000 vit-2.3.0/vit/config/config.sample.ini
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    16940 2023-04-14 04:10:49.000000 vit-2.3.0/vit/config_parser.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      296 2020-12-24 03:52:45.000000 vit-2.3.0/vit/debug.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6442 2020-12-24 03:52:45.000000 vit-2.3.0/vit/denotation.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       73 2022-04-28 19:54:53.000000 vit-2.3.0/vit/env.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      495 2023-04-14 04:10:49.000000 vit-2.3.0/vit/event.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       92 2020-12-24 03:52:45.000000 vit-2.3.0/vit/exception.py
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.153355 vit-2.3.0/vit/formatter/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6781 2023-04-14 04:10:49.000000 vit-2.3.0/vit/formatter/__init__.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      342 2021-02-02 03:24:52.000000 vit-2.3.0/vit/formatter/depends.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      206 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/depends_count.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      224 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/depends_indicator.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       80 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/depends_list.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2493 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/description.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      100 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/description_combined.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      895 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/description_count.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      357 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/description_desc.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      637 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/description_oneline.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      483 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/description_truncated.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      718 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/description_truncated_count.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      253 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      125 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      129 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       69 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_formatted.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      125 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      131 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      135 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/due_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       66 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      116 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      120 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      116 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      122 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      126 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/end_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      140 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      132 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       77 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_formatted.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      134 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      138 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      140 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/entry_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       61 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/id.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       62 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/id_number.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6424 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/markers.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       71 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      146 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      158 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      150 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      146 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      152 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      156 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      158 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/modified_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      140 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/parent.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       76 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/parent_long.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      190 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/parent_short.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1143 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/project.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       80 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/project_full.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      162 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/project_indented.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      342 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/project_parent.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/recur.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       76 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/recur_duration.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      178 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/recur_indicator.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      307 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      161 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      173 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      165 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       93 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_formatted.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      161 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      167 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      171 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      173 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/scheduled_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      275 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      202 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_active.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      141 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       77 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_formatted.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      143 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      147 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/start_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      312 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/status.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       76 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/status_long.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      139 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/status_short.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      785 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/tags.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      440 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/tags_count.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      275 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/tags_indicator.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/tags_list.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      812 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/uda_date.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      385 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/uda_duration.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      471 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/uda_indicator.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      404 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/uda_numeric.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      369 2022-10-14 23:05:54.000000 vit-2.3.0/vit/formatter/uda_string.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      271 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      141 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       77 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_formatted.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      137 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      143 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      147 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      149 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/until_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      135 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/urgency.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      152 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/urgency_integer.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       80 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/urgency_real.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       63 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/uuid.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       68 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/uuid_long.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      152 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/uuid_short.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       67 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      122 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait_age.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      134 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait_countdown.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      126 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait_epoch.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      122 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait_iso.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      128 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait_julian.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      132 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait_relative.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      134 2020-12-24 03:52:45.000000 vit-2.3.0/vit/formatter/wait_remaining.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5402 2023-04-14 04:10:49.000000 vit-2.3.0/vit/formatter_base.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     7345 2023-04-14 04:10:49.000000 vit-2.3.0/vit/help.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2300 2023-04-14 04:10:49.000000 vit-2.3.0/vit/key_cache.py
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.153355 vit-2.3.0/vit/keybinding/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1573 2020-12-30 18:53:00.000000 vit-2.3.0/vit/keybinding/vi.ini
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     6801 2023-04-14 04:10:49.000000 vit-2.3.0/vit/keybinding_parser.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1662 2023-04-14 04:10:49.000000 vit-2.3.0/vit/list_batcher.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1182 2023-04-14 04:10:49.000000 vit-2.3.0/vit/loader.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     3187 2023-04-14 04:10:49.000000 vit-2.3.0/vit/markers.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2050 2020-12-24 03:52:45.000000 vit-2.3.0/vit/multi_widget.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2692 2023-01-06 12:19:59.000000 vit-2.3.0/vit/option_parser.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1491 2023-04-14 04:10:49.000000 vit-2.3.0/vit/pid_manager.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2087 2023-04-14 04:10:49.000000 vit-2.3.0/vit/process.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5606 2023-04-14 04:10:49.000000 vit-2.3.0/vit/readline.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1978 2023-04-14 04:10:49.000000 vit-2.3.0/vit/registry.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     5214 2023-04-14 04:10:49.000000 vit-2.3.0/vit/task.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)    23608 2023-04-14 04:10:49.000000 vit-2.3.0/vit/task_list.py
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.153355 vit-2.3.0/vit/theme/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        0 2020-12-24 03:52:45.000000 vit-2.3.0/vit/theme/__init__.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      842 2020-12-24 03:52:45.000000 vit-2.3.0/vit/theme/classic.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      926 2020-12-24 03:52:45.000000 vit-2.3.0/vit/theme/default.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      410 2020-12-24 03:52:45.000000 vit-2.3.0/vit/uda.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     1529 2022-12-25 20:06:26.000000 vit-2.3.0/vit/util.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       14 2023-04-14 04:10:49.000000 vit-2.3.0/vit/version.py
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)      483 2021-11-04 13:51:45.000000 vit-2.3.0/vit/xdg.py
+drwxrwxr-x   0 hunmonk   (1000) hunmonk   (1000)        0 2023-04-14 04:27:09.117355 vit-2.3.0/vit.egg-info/
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     2911 2023-04-14 04:27:09.000000 vit-2.3.0/vit.egg-info/PKG-INFO
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)     4454 2023-04-14 04:27:09.000000 vit-2.3.0/vit.egg-info/SOURCES.txt
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        1 2023-04-14 04:27:09.000000 vit-2.3.0/vit.egg-info/dependency_links.txt
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       46 2023-04-14 04:27:09.000000 vit-2.3.0/vit.egg-info/entry_points.txt
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        1 2019-09-28 15:34:44.000000 vit-2.3.0/vit.egg-info/not-zip-safe
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)       74 2023-04-14 04:27:09.000000 vit-2.3.0/vit.egg-info/requires.txt
+-rw-rw-r--   0 hunmonk   (1000) hunmonk   (1000)        4 2023-04-14 04:27:09.000000 vit-2.3.0/vit.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vit-2.2.0b1/AUTHORS.md` & `vit-2.3.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `vit-2.2.0b1/COLOR.md` & `vit-2.3.0/COLOR.md`

 * *Files identical despite different names*

### Comparing `vit-2.2.0b1/INSTALL.md` & `vit-2.3.0/INSTALL.md`

 * *Files identical despite different names*

### Comparing `vit-2.2.0b1/LICENSE` & `vit-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vit-2.2.0b1/PKG-INFO` & `vit-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: vit
-Version: 2.2.0b1
+Version: 2.3.0
 Summary: Visual Interactive Taskwarrior full-screen terminal interface
 Home-page: https://github.com/vit-project/vit
 Author: Chad Phillips
 Author-email: chad@apartmentlines.com
-License: UNKNOWN
 Keywords: taskwarrior,console,tui,text-user-interface
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Natural Language :: English
 Classifier: Topic :: Text Processing :: General
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # VIT
 
 <img src="images/great-tit-square-small.png" alt="Logo" width="150" height="150" align="right" />
@@ -39,15 +37,15 @@
  * Multiple/customizable themes
  * Override/customize column formatters
  * Intelligent sub-project indenting
 
 ## Requirements
 
  * [Taskwarrior](https://taskwarrior.org)
- * [Python](https://www.python.org) 3.5+
+ * [Python](https://www.python.org) 3.7+
  * [pip](https://pypi.org/project/pip)
 
 ## Installation
 
 Follow the directions in [INSTALL.md](https://github.com/vit-project/vit/blob/2.x/INSTALL.md)
 
 ## Quick start
@@ -81,9 +79,7 @@
 
 ##### In tribute
 
  Our friend and collaborator Steve Rader passed away in May 2013.  We owe a lot to Steve for his excellent work, and so vit is preserved, maintained and continued.
 
  Taskwarrior Team
  support@taskwarrior.org
-
-
```

### Comparing `vit-2.2.0b1/README.md` & `vit-2.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  * Multiple/customizable themes
  * Override/customize column formatters
  * Intelligent sub-project indenting
 
 ## Requirements
 
  * [Taskwarrior](https://taskwarrior.org)
- * [Python](https://www.python.org) 3.5+
+ * [Python](https://www.python.org) 3.7+
  * [pip](https://pypi.org/project/pip)
 
 ## Installation
 
 Follow the directions in [INSTALL.md](INSTALL.md)
 
 ## Quick start
```

### Comparing `vit-2.2.0b1/setup.py` & `vit-2.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from setuptools import setup
 from os import path
 
 DEFAULT_BRANCH = "2.x"
 BASE_GITHUB_URL = "https://github.com/vit-project/vit/blob"
 
-MARKUP_LINK_REGEX = "\[([^]]+)\]\(([\w]+\.md)\)"
+MARKUP_LINK_REGEX = r"\[([^]]+)\]\(([\w]+\.md)\)"
 FILE_DIR = path.dirname(path.abspath(path.realpath(__file__)))
 
 with open(path.join(FILE_DIR, 'README.md')) as f:
     readme_contents = f.read()
     markup_link_substitution = '[\\1](%s/%s/\\2)' % (BASE_GITHUB_URL, DEFAULT_BRANCH)
     README = re.sub(MARKUP_LINK_REGEX, markup_link_substitution, readme_contents, flags=re.MULTILINE)
 
@@ -17,15 +17,15 @@
     INSTALL_PACKAGES = f.read().splitlines()
 
 with open(path.join(FILE_DIR, 'vit', 'version.py')) as f:
     VERSION = re.match(r"^VIT = '([\w\.]+)'$", f.read().strip())[1]
 
 setup(
     name='vit',
-    packages=['vit', 'vit.formatter', 'vit.theme'],
+    packages=['vit', 'vit.config', 'vit.formatter', 'vit.keybinding', 'vit.theme'],
     description="Visual Interactive Taskwarrior full-screen terminal interface",
     long_description=README,
     long_description_content_type='text/markdown',
     install_requires=INSTALL_PACKAGES,
     version=VERSION,
     url='https://github.com/vit-project/vit',
     author='Chad Phillips',
@@ -48,10 +48,10 @@
     ],
     entry_points = {
         'console_scripts': [
             'vit=vit.command_line:main',
         ],
     },
     include_package_data=True,
-    python_requires='>=3.5',
+    python_requires='>=3.7',
     zip_safe=False
 )
```

### Comparing `vit-2.2.0b1/test/test_list_batcher.py` & `vit-2.3.0/test/test_list_batcher.py`

 * *Files identical despite different names*

### Comparing `vit-2.2.0b1/vit/action_manager.py` & `vit-2.3.0/vit/action_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 
-class ActionManagerRegistrar(object):
+class ActionManagerRegistrar:
     def __init__(self, registry):
         self.registry = registry
         self.uuid = uuid.uuid4()
 
     def register(self, name, callback):
         self.registry.register(self.uuid, name, callback)
 
@@ -33,15 +33,15 @@
     def handled_action(self, keys):
         keybindings = self.registry.keybindings
         actions = self.actions()
         if keys in keybindings and 'action_name' in keybindings[keys] and keybindings[keys]['action_name'] in actions:
             return actions[keybindings[keys]['action_name']]
         return None
 
-class ActionManagerRegistry(object):
+class ActionManagerRegistry:
     def __init__(self, action_registry, keybindings, event=None):
         self.actions = {}
         self.action_registry = action_registry
         self.keybindings = keybindings
         self.event = event
 
     def get_registrar(self):
```

### Comparing `vit-2.2.0b1/vit/actions.py` & `vit-2.3.0/vit/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class Actions(object):
+class Actions:
 
     def __init__(self, action_registry):
         self.action_registry = action_registry
 
     def register(self):
         self.action_registrar = self.action_registry.get_registrar()
         # Global.
```

### Comparing `vit-2.2.0b1/vit/application.py` & `vit-2.3.0/vit/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 
 from importlib import import_module
 
+import os
+import signal
 import subprocess
 # TODO: Use regex module for better PCRE support?
 #       https://bitbucket.org/mrabarnett/mrab-regex
 import re
 import time
 import copy
 from inspect import isfunction
@@ -31,14 +33,15 @@
 from vit.color import TaskColorConfig, TaskColorizer
 from vit.task_list import TaskTable
 from vit.multi_widget import MultiWidget
 from vit.command_bar import CommandBar
 from vit.registry import ActionRegistry, RequestReply
 from vit.action_manager import ActionManagerRegistry
 from vit.denotation import DenotationPopupLauncher
+from vit.pid_manager import PidManager
 
 # NOTE: This entire class is a workaround for the fact that urwid catches the
 # 'ctrl l' keypress in its unhandled_input code, and prevents that from being
 # used for the refresh report functionality. Sadly, that is the default
 # keybinding, therefore the only way to make it work is to catch the refresh
 # action here in the top frame.
 class MainFrame(urwid.Frame):
@@ -63,24 +66,47 @@
             # action-manager:action-executed event, which clobbers the load
             # time currently.
             self.refresh()
             return None
         else:
             return super().keypress(size, key)
 
-class Application():
+class Application:
     def __init__(self, option, filters):
         self.extra_filters = filters
         self.loader = Loader()
         self.load_early_config()
         self.set_report()
         self.setup_main_loop()
+        self.setup_signal_listeners()
         self.refresh(False)
+        self.setup_pid()
         self.loop.run()
 
+    def setup_signal_listeners(self):
+        # Since not all platforms may have all signals, ensure they are
+        # supported before adding a handler.
+        if hasattr(signal, 'SIGUSR1'):
+            pipe = self.loop.watch_pipe(self.async_refresh)
+            def sigusr1_handler(signum, frame):
+                os.write(pipe, b'x')
+            signal.signal(signal.SIGUSR1, sigusr1_handler)
+        if hasattr(signal, 'SIGTERM'):
+            def sigterm_handler(signum, frame):
+                self.signal_quit("SIGTERM")
+            signal.signal(signal.SIGTERM, sigterm_handler)
+        if hasattr(signal, 'SIGINT'):
+            def sigint_handler(signum, frame):
+                self.signal_quit("SIGINT")
+            signal.signal(signal.SIGINT, sigint_handler)
+        if hasattr(signal, 'SIGQUIT'):
+            def sigquit_handler(signum, frame):
+                self.signal_quit("SIGQUIT")
+            signal.signal(signal.SIGQUIT, sigquit_handler)
+
     def load_early_config(self):
         self.config = ConfigParser(self.loader)
         self.task_config = TaskParser(self.config)
         self.reports = self.task_config.get_reports()
 
     def set_report(self):
         if len(self.extra_filters) == 0:
@@ -93,14 +119,21 @@
     def setup_main_loop(self):
         self.loop = urwid.MainLoop(urwid.Text(''), unhandled_input=self.key_pressed, pop_ups=True, handle_mouse=self.config.mouse_enabled)
         try:
             self.loop.screen.set_terminal_properties(colors=256)
         except:
             pass
 
+    def setup_pid(self):
+        self.pid_manager = PidManager(self.config)
+        self.pid_manager.setup()
+
+    def teardown_pid(self):
+        self.pid_manager.teardown()
+
     def set_active_context(self):
         self.context = self.task_config.get_active_context()
 
     def load_contexts(self):
         self.contexts = self.task_config.get_contexts()
 
     def bootstrap(self, load_early_config=True):
@@ -179,15 +212,15 @@
         self.action_manager_registrar.register('TASK_WAIT', self.task_action_wait)
         self.action_manager_registrar.register('TASK_EDIT', self.task_action_edit)
         self.action_manager_registrar.register('TASK_SHOW', self.task_action_show)
 
     def default_keybinding_replacements(self):
         import json
         from datetime import datetime
-        task_replacement_match = re.compile("^TASK_(\w+)$")
+        task_replacement_match = re.compile(r"^TASK_(\w+)$")
         def _task_attribute_match(variable):
             matches = re.match(task_replacement_match, variable)
             if matches:
                 attribute = matches.group(1).lower()
                 if attribute in self.available_columns:
                     return [attribute]
         def _task_attribute_replace(task, attribute):
@@ -505,28 +538,29 @@
 
     def search_rows(self, term, start_index=0, reverse=False):
         escaped_term = re.escape(term)
         search_regex = re.compile(escaped_term, re.MULTILINE)
         rows = self.table.rows
         current_index = start_index
         last_index = len(rows) - 1
-        start_matches = self.search_row_has_search_term(rows[start_index], search_regex)
-        current_index = self.search_increment_index(current_index, reverse)
-        while True:
-            if reverse and current_index < 0:
-                self.search_loop_warning('TOP', reverse)
-                current_index = last_index
-            elif not reverse and current_index > last_index:
-                self.search_loop_warning('BOTTOM', reverse)
-                current_index = 0
-            if self.search_row_has_search_term(rows[current_index], search_regex):
-                return current_index
-            if current_index == start_index:
-                return start_index if start_matches else None
+        if len(rows) > 0:
+            start_matches = self.search_row_has_search_term(rows[start_index], search_regex)
             current_index = self.search_increment_index(current_index, reverse)
+            while True:
+                if reverse and current_index < 0:
+                    self.search_loop_warning('TOP', reverse)
+                    current_index = last_index
+                elif not reverse and current_index > last_index:
+                    self.search_loop_warning('BOTTOM', reverse)
+                    current_index = 0
+                if self.search_row_has_search_term(rows[current_index], search_regex):
+                    return current_index
+                if current_index == start_index:
+                    return start_index if start_matches else None
+                current_index = self.search_increment_index(current_index, reverse)
 
     def search_increment_index(self, current_index, reverse=False):
         return current_index + (-1 if reverse else 1)
 
     def search_display_message(self, reverse=False):
         self.activate_message_bar("Search %s for: %s" % ('reverse' if reverse else 'forward', self.search_term_active))
 
@@ -560,15 +594,21 @@
             uuid = self.task_list.focus.uuid
             task = self.model.get_task(uuid)
             return uuid, task
         except:
             pass
         return False, False
 
+    def signal_quit(self, signal):
+        #import debug
+        #debug.file("VIT received %s signal, quitting" % signal)
+        self.quit()
+
     def quit(self):
+        self.teardown_pid()
         raise urwid.ExitMainLoop()
 
     def build_task_table(self):
         self.table = TaskTable(self.config, self.task_config, self.formatter, self.loop.screen, on_select=self.on_select, event=self.event, action_manager=self.action_manager, request_reply=self.request_reply, markers=self.markers, draw_screen_callback=self.loop.draw_screen)
 
     def update_task_table(self):
         self.table.update_data(self.reports[self.report], self.model.tasks)
@@ -912,14 +952,17 @@
         if returncode == 0:
             num_tasks = int(stdout.strip())
             text = '%s %s completed' % (num_tasks, num_tasks == 1 and 'task' or 'tasks')
             self.status_tasks_completed.original_widget.set_text(text)
         else:
             raise RuntimeError("Error retrieving completed tasks: %s" % stderr)
 
+    def async_refresh(self, _):
+        self.refresh()
+
     def refresh(self, load_early_config=True):
         self.bootstrap(load_early_config)
         self.build_main_widget()
         # NOTE: Don't see any other way to clear the old palette.
         self.loop.screen._palette = {}
         self.loop.screen.register_palette(self.theme)
         self.loop.screen.clear()
```

### Comparing `vit-2.2.0b1/vit/autocomplete.py` & `vit-2.3.0/vit/autocomplete.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import reduce
 
 import re
 
 from vit import util
 from vit.process import Command
 
-class AutoComplete(object):
+class AutoComplete:
 
     def __init__(self, config, default_filters=None, extra_filters=None):
         self.default_filters = default_filters or ('column', 'project', 'tag')
         self.extra_filters = extra_filters or {}
         self.default_filter_config = {
             'column': {
                 'suffixes': [':'],
```

### Comparing `vit-2.2.0b1/vit/base_list_box.py` & `vit-2.3.0/vit/base_list_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,19 +67,21 @@
     def keypress_page_up(self, size):
         self.keypress(size, '<Page Up>')
 
     def keypress_page_down(self, size):
         self.keypress(size, '<Page Down>')
 
     def keypress_home(self, size):
-        self.set_focus(0)
+        if len(self.body) > 0:
+            self.set_focus(0)
 
     def keypress_end(self, size):
-        self.set_focus(len(self.body) - 1)
-        self.set_focus_valign('bottom')
+        if len(self.body) > 0:
+            self.set_focus(len(self.body) - 1)
+            self.set_focus_valign('bottom')
 
     def keypress_screen_top(self, size):
         top, _, _ = self.get_top_middle_bottom_rows(size)
         if top:
             self.set_focus(top.position)
 
     def keypress_screen_middle(self, size):
@@ -89,16 +91,17 @@
 
     def keypress_screen_bottom(self, size):
         _, _, bottom = self.get_top_middle_bottom_rows(size)
         if bottom:
             self.set_focus(bottom.position)
 
     def keypress_focus_valign_center(self, size):
-        self.set_focus(self.focus_position)
-        self.set_focus_valign('middle')
+        if len(self.body) > 0:
+            self.set_focus(self.focus_position)
+            self.set_focus_valign('middle')
 
     def transform_special_keys(self, key):
         # NOTE: These are special key presses passed to allow navigation
         #       keys to be managed via keybinding configuration. They are
         #       converted back to standard key presses here.
         if key in ['<Up>', '<Down>', '<Page Up>', '<Page Down>']:
             key = re.sub(BRACKETS_REGEX, '', key).lower()
```

### Comparing `vit-2.2.0b1/vit/color.py` & `vit-2.3.0/vit/color.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,30 +5,34 @@
 from vit.color_mappings import task_256_to_urwid_256, task_bright_to_color
 
 VALID_COLOR_MODIFIERS = [
     'bold',
     'underline',
 ]
 
-class TaskColorConfig(object):
+INVALID_COLOR_MODIFIERS = [
+    'inverse',
+]
+
+class TaskColorConfig:
     """Colorized task output.
     """
     def __init__(self, config, task_config, theme, theme_alt_backgrounds):
         self.config = config
         self.task_config = task_config
         self.theme = theme
         self.theme_alt_backgrounds = theme_alt_backgrounds
         self.include_subprojects = self.config.get('color', 'include_subprojects')
         self.task_256_to_urwid_256 = task_256_to_urwid_256()
         # NOTE: Because Taskwarrior disables color on piped commands, and I don't
         # see any portable way to get output from a system command in Python
         # without pipes, the 'color' config setting in Taskwarrior is not used, and
         # instead a custom setting is used.
         self.color_enabled = self.config.get('color', 'enabled')
-        self.display_attrs_available, self.display_attrs = self.convert_color_config(self.task_config.filter_to_dict('^color\.'))
+        self.display_attrs_available, self.display_attrs = self.convert_color_config(self.task_config.filter_to_dict(r'^color\.'))
         self.project_display_attrs = self.get_project_display_attrs()
         if self.include_subprojects:
             self.add_project_children()
         self.inject_alt_background_display_attrs()
 
     def inject_alt_background_display_attrs(self):
         for display_attr in self.display_attrs.copy():
@@ -92,22 +96,29 @@
         return self.convert_color_parts(foreground_parts), self.convert_color_parts(background_parts)
 
     def convert_color_parts(self, color_parts):
         sorted_parts = self.sort_color_parts(color_parts)
         remapped_colors = self.map_named_colors(sorted_parts)
         return ','.join(remapped_colors)
 
+    def check_invalid_color_parts(self, color_parts):
+        invalid_color_parts = {*color_parts} & {*INVALID_COLOR_MODIFIERS}
+        if invalid_color_parts:
+            raise ValueError("The following TaskWarrior color definitions are unsupported in VIT: %s -- read the documentation for possible workarounds" % ", ".join(invalid_color_parts))
+
     def map_named_colors(self, color_parts):
         if len(color_parts) > 0 and color_parts[0] in self.task_256_to_urwid_256:
             color_parts[0] = self.task_256_to_urwid_256[color_parts[0]]
         return color_parts
 
     def make_color_parts(self, foreground, background):
         foreground_parts = self.split_color_parts(foreground)
+        self.check_invalid_color_parts(foreground_parts)
         background_parts = self.split_color_parts(background)
+        self.check_invalid_color_parts(background_parts)
         return foreground_parts, background_parts
 
     def split_color_parts(self, color_parts):
         parts = color_parts.split() if color_parts else []
         return parts
 
     def is_modifier(self, elem):
@@ -119,16 +130,16 @@
                 return 1
             elif not self.is_modifier(first) and self.is_modifier(second):
                 return -1
             else:
                 return 0
         return sorted(color_parts, key=cmp_to_key(comparator))
 
-class TaskColorizer(object):
-    class Decorator(object):
+class TaskColorizer:
+    class Decorator:
         def color_enabled(func):
             @wraps(func)
             def verify_color_enabled(self, *args, **kwargs):
                 return func(self, *args, **kwargs) if self.color_enabled else None
             return verify_color_enabled
     def __init__(self, color_config):
         self.color_config = color_config
```

### Comparing `vit-2.2.0b1/vit/color_mappings.py` & `vit-2.3.0/vit/color_mappings.py`

 * *Files identical despite different names*

### Comparing `vit-2.2.0b1/vit/command_bar.py` & `vit-2.3.0/vit/command_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     def set_metadata(self, metadata):
         self.metadata = self.prepare_metadata(metadata)
 
     def set_edit_text_callback(self):
         return self.set_edit_text
 
-class CommandBarHistory(object):
+class CommandBarHistory:
     """Holds command-specific history for the command bar.
     """
     def __init__(self):
         self.commands = {}
         self.scrolling = False
 
     def add(self, command, text):
```

### Comparing `vit-2.2.0b1/vit/config/config.sample.ini` & `vit-2.3.0/vit/config/config.sample.ini`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,32 @@
 # Boolean. If true, hitting backspace against an empty prompt aborts the prompt.
 #abort_backspace = False
 
 # Boolean. If true, VIT will focus on the newly added task. Note: the new task must be
 #included in the active filter for this setting to have effect.
 #focus_on_add = False
 
+# Path to a directory to manage pid files for running instances of VIT.
+# If no path is provided, no pid files will be managed.
+# The special token $UID may be used, and will be substituted with the user ID
+# of the user starting VIT.
+# VIT can be run with the '--list-pids' argument, which will output a list of
+# all pids in pid_dir; useful for sending signals to the running processes.
+# If you use this feature, it's suggested to choose a directory that is
+# automatically cleaned on boot, e.g.:
+#   /var/run/user/$UID/vit
+#   /tmp/vit_pids
+#pid_dir =
+
+# Int. The number of flash repetitions focusing on the edit made
+#flash_focus_repeat_times = 2
+
+# Float. Waiting time for the blink focusing on the edit made
+#flash_focus_pause_seconds = 0.1
+
 [report]
 
 # The default Taskwarrior report to load when VIT first starts, if no report
 # or filters are passed at the command line.
 #default_report = next
 
 # The default Taskwarrior report to load when VIT first starts, if filters are
```

### Comparing `vit-2.2.0b1/vit/config_parser.py` & `vit-2.3.0/vit/config_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 from vit import env, xdg
 from vit.process import Command
 
 SORT_ORDER_CHARACTERS = ['+', '-']
 SORT_COLLATE_CHARACTERS = ['/']
 VIT_CONFIG_FILE = 'config.ini'
-FILTER_EXCLUSION_REGEX = re.compile('^limit:')
-FILTER_PARENS_REGEX = re.compile('([\(\)])')
-CONFIG_BOOLEAN_TRUE_REGEX = re.compile('1|yes|true', re.IGNORECASE)
+FILTER_EXCLUSION_REGEX = re.compile(r'^limit:')
+FILTER_PARENS_REGEX = re.compile(r'([\(\)])')
+CONFIG_BOOLEAN_TRUE_REGEX = re.compile(r'1|yes|true', re.IGNORECASE)
 # TaskParser expects clean hierarchies in the Taskwarrior dotted config names.
 # However, this is occasionally violated, with a leaf ending in both a string
 # value and another branch. The below list contains the config values that
 # violate this convention, and transform them into a single additional branch
 # of value CONFIG_STRING_LEAVES_DEFAULT_BRANCH
 CONFIG_STRING_LEAVES = [
     'color.calendar.due',
@@ -42,14 +42,17 @@
         'default_keybindings': 'vi',
         'theme': 'default',
         'confirmation': True,
         'wait': True,
         'mouse': False,
         'abort_backspace': False,
         'focus_on_add': False,
+        'pid_dir': '',
+        'flash_focus_repeat_times': 2,
+        'flash_focus_pause_seconds': 0.1,
     },
     'report': {
         'default_report': 'next',
         'default_filter_only_report': 'next',
         'indent_subprojects': True,
         'row_striping': True,
     },
@@ -90,26 +93,26 @@
     'A': '%A',                           # Complete English day name, eg 'monday', 'tuesday'
     'b': '%b',                           # 3-character English month name abbreviation, eg 'jan', 'feb'
     'B': '%B',                           # Complete English month name, eg 'january', 'february'
     'j': '%%%sj' % NO_PAD_FORMAT_CODE,   # 1, 2 or 3 digit day-of-year number, sometimes referred to as a Julian date, eg '1', '11', or '365'
     'J': '%j',                           # 3 digit day of year number, sometimes referred to as a Julian date, eg '001', '011', or '365'
 }
 
-class ConfigParser(object):
+class ConfigParser:
     def __init__(self, loader):
         self.loader = loader
         self.config = configparser.SafeConfigParser()
         self.config.optionxform = str
         self.user_config_dir = self.loader.user_config_dir
         self.user_config_filepath = '%s/%s' % (self.user_config_dir, VIT_CONFIG_FILE)
         if not self.config_file_exists(self.user_config_filepath):
             self.optional_create_config_file(self.user_config_filepath)
+        self.config.read(self.user_config_filepath)
         self.taskrc_path = self.get_taskrc_path()
         self.validate_taskrc()
-        self.config.read(self.user_config_filepath)
         self.defaults = DEFAULTS
         self.set_config_data()
 
     def set_config_data(self):
         self.subproject_indentable = self.is_subproject_indentable()
         self.row_striping_enabled = self.is_row_striping_enabled()
         self.confirmation_enabled = self.is_confirmation_enabled()
@@ -161,35 +164,45 @@
         copyfile('%s/config/config.sample.ini' % basedir, filepath)
 
     def get(self, section, key):
         default = DEFAULTS[section][key]
         try:
             value = self.config.get(section, key)
             return self.transform(key, value, default)
-        except (configparser.NoSectionError, configparser.NoOptionError):
+        except (configparser.NoSectionError, configparser.NoOptionError, ValueError):
             return default
 
     def items(self, section):
         try:
             return self.config.items(section)
         except configparser.NoSectionError:
             return []
 
     def has_section(self, section):
         return self.config.has_section(section)
 
     def transform(self, key, value, default):
         if isinstance(default, bool):
             return self.transform_bool(value)
+        elif isinstance(default, int):
+            return self.transform_int(value)
+        elif isinstance(default, float):
+            return self.transform_float(value)
         else:
             return value
 
     def transform_bool(self, value):
         return True if CONFIG_BOOLEAN_TRUE_REGEX.match(value) else False
 
+    def transform_int(self, value):
+        return int(value)
+
+    def transform_float(self, value):
+        return float(value)
+
     def get_taskrc_path(self):
         taskrc_path = os.path.expanduser('TASKRC' in env.user and env.user['TASKRC'] or self.get('taskwarrior', 'taskrc'))
 
         if not os.path.exists(taskrc_path):
             xdg_dir = xdg.get_xdg_config_dir(taskrc_path, "task")
             if xdg_dir:
                 taskrc_path = os.path.join(xdg_dir, "taskrc")
@@ -207,15 +220,21 @@
 
     def is_wait_enabled(self):
         return self.get('vit', 'wait')
 
     def is_mouse_enabled(self):
         return self.get('vit', 'mouse')
 
-class TaskParser(object):
+    def get_flash_focus_repeat_times(self):
+        return self.get('vit', 'flash_focus_repeat_times')
+
+    def get_flash_focus_pause_seconds(self):
+        return self.get('vit', 'flash_focus_pause_seconds')
+
+class TaskParser:
     def __init__(self, config):
         self.config = config
         self.task_config = []
         self.projects = []
         self.contexts = {}
         self.reports = {}
         self.disallowed_reports = [
@@ -271,15 +290,15 @@
 
     def filter(self, matcher_regex):
         return list(filter(lambda config_pair: re.match(matcher_regex, config_pair[0]), self.task_config))
 
     def subtree(self, matcher, walk_subtree=True):
         matcher_regex = matcher
         if walk_subtree:
-            matcher_regex = r'%s' % (('^%s' % matcher).replace('.', '\.'))
+            matcher_regex = r'%s' % (('^%s' % matcher).replace(r'.', r'\.'))
         full_tree = {}
         lines = self.filter(matcher_regex)
         for (hierarchy, value) in lines:
             # NOTE: This is necessary in order to convert Taskwarrior's dotted
             # config syntax into a full tree, as some leaves are both branches
             # and leaves.
             hierarchy = self.transform_string_leaves(hierarchy)
```

### Comparing `vit-2.2.0b1/vit/denotation.py` & `vit-2.3.0/vit/denotation.py`

 * *Files identical despite different names*

### Comparing `vit-2.2.0b1/vit/formatter/__init__.py` & `vit-2.3.0/vit/formatter/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import math
 from datetime import datetime
-from pytz import timezone
+try:
+    from zoneinfo import ZoneInfo
+except ImportError:
+    from backports.zoneinfo import ZoneInfo
+
+from vit.util import unicode_len
 
 TIME_UNIT_MAP = {
     'seconds': {
         'label': 's',
         'divisor': 1,
         'threshold': 60,
      },
@@ -35,37 +40,37 @@
      },
     'years': {
         'label': 'y',
         'divisor': 86400 * 365,
      },
 }
 
-class Formatter(object):
+class Formatter:
     def __init__(self, column, report, formatter_base, blocking_task_uuids, **kwargs):
         self.column = column
         self.report = report
         self.formatter = formatter_base
         self.colorizer = self.formatter.task_colorizer
         self.blocking_task_uuids = blocking_task_uuids
 
     def format(self, obj, task):
         if not obj:
             return self.empty()
         obj = str(obj)
-        return (len(obj), self.markup_element(obj))
+        return (unicode_len(obj), self.markup_element(obj))
 
     def empty(self):
         return (0, '')
 
     def markup_element(self, obj):
         return (self.colorize(obj), obj)
 
     def markup_none(self, color):
         if color:
-            return (len(self.formatter.none_label), (color, self.formatter.none_label))
+            return (unicode_len(self.formatter.none_label), (color, self.formatter.none_label))
         else:
             return self.empty()
 
     def colorize(self, obj):
         return None
 
     def filter_by_blocking_task_uuids(self, depends):
@@ -90,15 +95,15 @@
     pass
 
 class Duration(Formatter):
     def format(self, obj, task):
         if not obj:
             return self.empty()
         formatted_duration = self.format_duration(obj)
-        return (len(formatted_duration), self.markup_element(obj, formatted_duration))
+        return (unicode_len(formatted_duration), self.markup_element(obj, formatted_duration))
 
     def format_duration(self, obj):
         return obj
 
     def markup_element(self, obj, formatted_duration):
         return (self.colorize(obj), formatted_duration)
 
@@ -107,15 +112,15 @@
         self.custom_formatter = None if not 'custom_formatter' in kwargs else kwargs['custom_formatter']
         super().__init__(column, report, defaults, blocking_task_uuids)
 
     def format(self, dt, task):
         if not dt:
             return self.empty()
         formatted_date = self.format_datetime(dt, task)
-        return (len(formatted_date), self.markup_element(dt, formatted_date, task))
+        return (unicode_len(formatted_date), self.markup_element(dt, formatted_date, task))
 
     def format_datetime(self, dt, task):
         return dt.strftime(self.custom_formatter or self.formatter.report)
 
     def markup_element(self, dt, formatted_date, task):
         return (self.colorize(dt, task), formatted_date)
 
@@ -146,38 +151,38 @@
             unit = 'years'
         age = test // TIME_UNIT_MAP[unit]['divisor']
         return '%s%d%s' % (sign, age, TIME_UNIT_MAP[unit]['label'])
 
     def age(self, dt):
         if dt == None:
             return ''
-        now = datetime.now(self.formatter.zone)
+        now = datetime.now().astimezone()
         seconds = (now - dt).total_seconds()
         return self.format_duration_vague(seconds)
 
     def countdown(self, dt):
         if dt == None:
             return ''
-        now = datetime.now(self.formatter.zone)
+        now = datetime.now().astimezone()
         if dt < now:
             return ''
         seconds = (dt - now).total_seconds()
         return self.format_duration_vague(seconds)
 
     def relative(self, dt):
         if dt == None:
             return ''
-        now = datetime.now(self.formatter.zone)
+        now = datetime.now().astimezone()
         seconds = (dt - now).total_seconds()
         return self.format_duration_vague(seconds)
 
     def remaining(self, dt):
         if dt == None:
             return ''
-        now = datetime.now(self.formatter.zone)
+        now = datetime.now().astimezone()
         if dt < now:
             return ''
         seconds = (dt - now).total_seconds()
         return self.format_duration_vague(seconds)
 
     def epoch(self, dt):
         if dt == None:
@@ -194,23 +199,23 @@
         jdn = dt.day + math.floor((153*m + 2)/5) + 365*y + math.floor(y/4) - math.floor(y/100) + math.floor(y/400) - 32045
         jd = jdn + (dt.hour - 12) / 24 + dt.minute / 1440 + dt.second / 86400 + dt.microsecond / 86400000000
         return str(jd)
 
     def iso(self, dt):
         if dt == None:
             return ''
-        dt = dt.replace(tzinfo=timezone('UTC'))
+        dt = dt.replace(tzinfo=ZoneInfo('UTC'))
         return dt.isoformat()
 
 class List(Formatter):
 
     def format(self, obj, task):
         if not obj:
             return self.empty()
         formatted = self.format_list(obj, task)
-        return (len(formatted), self.markup_element(obj, formatted))
+        return (unicode_len(formatted), self.markup_element(obj, formatted))
 
     def markup_element(self, obj, formatted):
         return (self.colorize(obj), formatted)
 
     def format_list(self, obj, task):
         return ','.join(obj) if obj else ''
```

### Comparing `vit-2.2.0b1/vit/formatter/description.py` & `vit-2.3.0/vit/formatter/description.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from functools import reduce
 
 from vit.formatter import String
+from vit.util import unicode_len
 
 class Description(String):
     def format(self, description, task):
         if not description:
             return self.empty()
-        width = len(description)
+        width = unicode_len(description)
         colorized_description = self.colorize_description(description)
         if task['annotations']:
             annotation_width, colorized_description = self.format_combined(colorized_description, task)
             if annotation_width > width:
                 width = annotation_width
         return (width, colorized_description)
 
     def format_description_truncated(self, description):
-        return '%s...' % description[:self.formatter.description_truncate_len] if len(description) > self.formatter.description_truncate_len else description
+        return '%s...' % description[:self.formatter.description_truncate_len] if unicode_len(description) > self.formatter.description_truncate_len else description
 
     def format_combined(self, colorized_description, task):
         annotation_width, formatted_annotations = self.format_annotations(task)
         return annotation_width, colorized_description + [(None, "\n"), (None, formatted_annotations)]
 
     def format_annotations(self, task):
         def reducer(accum, annotation):
             width, formatted_list = accum
             formatted = self.format_annotation(annotation)
-            new_width = len(formatted)
+            new_width = unicode_len(formatted)
             if new_width > width:
                 width = new_width
             formatted_list.append(formatted)
             return (width, formatted_list)
         width, formatted_annotations = reduce(reducer, task['annotations'], (0, []))
         return width, "\n".join(formatted_annotations)
```

### Comparing `vit-2.2.0b1/vit/formatter/description_count.py` & `vit-2.3.0/vit/formatter/description_count.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from vit.formatter.description import Description
+from vit.util import unicode_len
 
 class DescriptionCount(Description):
     def format(self, description, task):
         if not description:
             return self.empty()
-        width = len(description)
+        width = unicode_len(description)
         colorized_description = self.colorize_description(description)
         if not task['annotations']:
             return (width, colorized_description)
         else:
             count_width, colorized_description = self.format_count(colorized_description, task)
             return (width + count_width, colorized_description)
 
     def format_count(self, colorized_description, task):
         count_string = self.format_annotation_count(task)
-        return len(count_string), colorized_description + [(None, count_string)]
+        return unicode_len(count_string), colorized_description + [(None, count_string)]
 
     def format_annotation_count(self, task):
         return " [%d]" % len(task['annotations'])
```

### Comparing `vit-2.2.0b1/vit/formatter/description_oneline.py` & `vit-2.3.0/vit/formatter/description_oneline.py`

 * *Files identical despite different names*

### Comparing `vit-2.2.0b1/vit/formatter/markers.py` & `vit-2.3.0/vit/formatter/markers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unicodedata
 from vit.formatter import Marker
+from vit.util import unicode_len
 
 class Markers(Marker):
     def format(self, _, task):
         text_markup = []
         width = 0
         if self.mark_tags:
             width, text_markup = self.format_tags(width, text_markup, task['tags'])
@@ -32,15 +33,15 @@
 
     def color_required(self, color):
         return self.require_color and not color
 
     def add_label(self, color, label, width, text_markup):
         if self.color_required(color) or not label:
             return width, text_markup
-        width += len(label) + len([c for c in label if unicodedata.east_asian_width(c) == 'W'])
+        width += unicode_len(label)
         text_markup += [(color, label)]
         return width, text_markup
 
     def format_tags(self, width, text_markup, tags):
         if not tags:
             color = self.colorizer.tag_none()
             label = self.labels['tag.none.label']
```

### Comparing `vit-2.2.0b1/vit/formatter/project.py` & `vit-2.3.0/vit/formatter/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from vit.formatter import String
+from vit.util import unicode_len
 
 class Project(String):
     def __init__(self, column, report, defaults, blocking_task_uuids, **kwargs):
         super().__init__(column, report, defaults, blocking_task_uuids)
         self.indent_subprojects = self.is_subproject_indentable()
 
     def format(self, project, task):
         return self.format_project(project, task) if project else self.markup_none(self.colorizer.project_none())
 
     def format_project(self, project, task):
-        return self.format_subproject_indented(project, task) if self.indent_subprojects else (len(project), self.markup_element(project))
+        return self.format_subproject_indented(project, task) if self.indent_subprojects else (unicode_len(project), self.markup_element(project))
 
     def format_subproject_indented(self, project, task):
         parts = project.split('.')
         (width, spaces, marker, subproject) = self.formatter.format_subproject_indented(parts)
         return (width, [spaces, marker, (self.colorize(project), subproject)])
 
     def is_subproject_indentable(self):
```

### Comparing `vit-2.2.0b1/vit/formatter/tags.py` & `vit-2.3.0/vit/formatter/tags.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from vit.formatter import Formatter
+from vit.util import unicode_len
 
 class Tags(Formatter):
     def format(self, tags, task):
         if not tags:
             return self.markup_none(self.colorizer.tag_none())
         elif len(tags) == 1:
             tag = list(tags)[0]
-            return (len(tag), self.markup_element(tag))
+            return (unicode_len(tag), self.markup_element(tag))
         else:
             last_tag = list(tags)[-1]
             width = 0
             text_markup = []
             for tag in tags:
-                width += len(tag)
+                width += unicode_len(tag)
                 text_markup += [self.markup_element(tag)]
                 if tag != last_tag:
                     width += 1
                     text_markup += [',']
             return (width, text_markup)
 
     def colorize(self, tag):
```

### Comparing `vit-2.2.0b1/vit/formatter/uda_date.py` & `vit-2.3.0/vit/formatter/uda_date.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import datetime
 from vit.formatter import DateTime
+from vit.util import unicode_len
 
 # TODO: Remove this once tasklib bug is fixed.
 from tasklib.serializing import SerializingObject
 serializer = SerializingObject({})
 
 class UdaDate(DateTime):
     def format(self, dt, task):
         if not dt:
             return self.markup_none(self.colorize())
         # TODO: Remove this once tasklib bug is fixed.
         # https://github.com/robgolding/tasklib/issues/30
         dt = dt if isinstance(dt, datetime.datetime) else serializer.timestamp_deserializer(dt)
         formatted_date = dt.strftime(self.custom_formatter or self.formatter.report)
-        return (len(formatted_date), (self.colorize(dt), formatted_date))
+        return (unicode_len(formatted_date), (self.colorize(dt), formatted_date))
     def colorize(self, dt=None):
         return self.colorizer.uda_date(self.column, dt)
```

### Comparing `vit-2.2.0b1/vit/formatter_base.py` & `vit-2.3.0/vit/formatter_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from importlib import import_module
 from datetime import datetime, timedelta
-from tzlocal import get_localzone
-from pytz import timezone
+try:
+    from zoneinfo import ZoneInfo
+except ImportError:
+    from backports.zoneinfo import ZoneInfo
 
 from vit import util
 from vit import uda
+from vit.util import unicode_len
 
 INDICATORS = [
     'active',
     'dependency',
     'recurrence',
     'tag',
 ]
 UDA_DEFAULT_INDICATOR = 'U'
 
 DEFAULT_DESCRIPTION_TRUNCATE_LEN=20
 
-class FormatterBase(object):
+class FormatterBase:
     def __init__(self, loader, config, task_config, markers, task_colorizer):
         self.loader = loader
         self.config = config
         self.task_config = task_config
         self.markers = markers
         self.task_colorizer = task_colorizer
         self.date_default = self.task_config.translate_date_markers(self.task_config.subtree('dateformat')["default"])
         self.report = self.task_config.translate_date_markers(self.task_config.subtree('dateformat.report')) or self.date_default
         self.annotation = self.task_config.translate_date_markers(self.task_config.subtree('dateformat.annotation')) or self.date_default
         self.description_truncate_len = DEFAULT_DESCRIPTION_TRUNCATE_LEN
-        self.zone = get_localzone()
-        self.epoch_datetime = datetime(1970, 1, 1, tzinfo=timezone('UTC'))
+        self.epoch_datetime = datetime(1970, 1, 1, tzinfo=ZoneInfo('UTC'))
         self.due_days = int(self.task_config.subtree('due'))
         self.none_label = config.get('color', 'none_label')
         self.build_indicators()
 
     def build_indicators(self):
         for indicator in INDICATORS:
             label = self.task_config.subtree('%s.indicator' % indicator)
@@ -84,24 +86,24 @@
                 if formatter_class:
                     return name, formatter_class
         return name, Formatter
 
     def format_subproject_indented(self, project_parts):
         if len(project_parts) == 1:
             subproject = project_parts[0]
-            return (len(subproject), '', '', subproject)
+            return (unicode_len(subproject), '', '', subproject)
         else:
             subproject = project_parts.pop()
             space_padding = (len(project_parts) * 2) - 1
             indicator = u'\u21aa '
-            width = space_padding + len(indicator) + len(subproject)
+            width = space_padding + unicode_len(indicator) + unicode_len(subproject)
             return (width, ' ' * space_padding , indicator, subproject)
 
     def recalculate_due_datetimes(self):
-        self.now = datetime.now(self.zone)
+        self.now = datetime.now().astimezone()
         # NOTE: For some reason using self.zone for the tzinfo below results
         # in the tzinfo object having a zone of 'LMT', which is wrong. Using
         # the tzinfo associated with self.now returns the correct value, no
         # idea why this glitch happens.
         self.end_of_day = datetime(self.now.year, self.now.month, self.now.day, 23, 59, 59, tzinfo=self.now.tzinfo)
         self.due_soon = self.end_of_day + timedelta(days=self.due_days)
```

### Comparing `vit-2.2.0b1/vit/help.py` & `vit-2.3.0/vit/help.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 
 import urwid
 
 from vit.base_list_box import BaseListBox
+from vit.util import unicode_len
 
 CURLY_BRACES_REGEX = re.compile("[{}]")
 SPECIAL_KEY_SUBSTITUTIONS = {
     '<Colon>': ':',
     '<Equals>': '=',
 }
 
@@ -53,16 +54,16 @@
 
     def calculate_column_widths(self, entries):
         column_widths = {
             'type': 0,
             'keys': 0,
         }
         for entry in entries:
-            type_len = len(entry[0])
-            keys_len = len(entry[1])
+            type_len = unicode_len(entry[0])
+            keys_len = unicode_len(entry[1])
             if type_len > column_widths['type']:
                 column_widths['type'] = type_len
             if keys_len > column_widths['keys']:
                 column_widths['keys'] = keys_len
         return column_widths
 
     def reload_entries(self, entries):
@@ -74,15 +75,15 @@
 
     def exit_help(self, data):
         self.event.emit("help:exit")
 
     def eat_other_keybindings(self):
         return True
 
-class Help(object):
+class Help:
     """Generates help list/display.
     """
     def __init__(self, keybinding_parser, actions, event=None, request_reply=None, action_manager=None):
         self.keybinding_parser = keybinding_parser
         self.actions = actions
         self.event = event
         self.request_reply = request_reply
```

### Comparing `vit-2.2.0b1/vit/key_cache.py` & `vit-2.3.0/vit/key_cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import reduce
 
 class KeyCacheError(Exception):
     pass
 
-class KeyCache(object):
+class KeyCache:
     def __init__(self, keybindings):
         self.keybindings = keybindings
         self.cached_keys = ''
         self.build_multi_key_cache()
 
     def get(self, key=None):
         return '%s%s' % (self.cached_keys, key) if key else self.cached_keys
```

### Comparing `vit-2.2.0b1/vit/keybinding/vi.ini` & `vit-2.3.0/vit/keybinding/vi.ini`

 * *Files identical despite different names*

### Comparing `vit-2.2.0b1/vit/keybinding_parser.py` & `vit-2.3.0/vit/keybinding_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     'space': ' ',
     'semicolon': ';',
 }
 
 class KeybindingError(Exception):
     pass
 
-class KeybindingParser(object):
+class KeybindingParser:
     def __init__(self, loader, config, action_registry):
         self.loader = loader
         self.config = config
         self.action_registry = action_registry
         self.actions = self.action_registry.get_actions()
         self.noop_action_name = self.action_registry.make_action_name(self.action_registry.noop_action_name)
         self.default_keybinding_name = self.config.get('vit', 'default_keybindings')
```

### Comparing `vit-2.2.0b1/vit/list_batcher.py` & `vit-2.3.0/vit/list_batcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 DEFAULT_BATCH_SIZE=100
 
 class ListBatchError(Exception):
     pass
 
-class ListBatcher(object):
+class ListBatcher:
     def __init__(self, batch_from, batch_to, batch_to_formatter=None, default_batch_size=DEFAULT_BATCH_SIZE):
         self.batch_from = batch_from
         self.batch_to = batch_to
         self.batch_to_formatter = batch_to_formatter
         self.default_batch_size = default_batch_size
         self.last_position = 0
         self.batching_complete = False
```

### Comparing `vit-2.2.0b1/vit/loader.py` & `vit-2.3.0/vit/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 except:
     import imp
 
 from vit import env, xdg
 
 DEFAULT_VIT_DIR = '~/.vit'
 
-class Loader(object):
+class Loader:
     def __init__(self):
         self.user_config_dir = os.path.expanduser('VIT_DIR' in env.user and env.user['VIT_DIR'] or DEFAULT_VIT_DIR)
 
         if not os.path.exists(self.user_config_dir):
             xdg_dir = xdg.get_xdg_config_dir(self.user_config_dir, "vit")
             if xdg_dir:
                 self.user_config_dir = xdg_dir
```

### Comparing `vit-2.2.0b1/vit/markers.py` & `vit-2.3.0/vit/markers.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     'tag.label': '(T)',
     'tag.none.label': '',
     'uda.label': '',
     'uda.priority.label': '(PR)',
     'until.label': '(U)',
 }
 
-class Markers(object):
+class Markers:
     def __init__(self, config, task_config):
         self.config = config
         self.task_config = task_config
         self.enabled = self.config.get('marker', 'enabled')
         if self.enabled:
             self.udas = uda.get_configured(self.task_config)
             self.markable_columns = MARKABLE_COLUMNS + list(self.udas.keys())
```

### Comparing `vit-2.2.0b1/vit/multi_widget.py` & `vit-2.3.0/vit/multi_widget.py`

 * *Files identical despite different names*

### Comparing `vit-2.2.0b1/vit/process.py` & `vit-2.3.0/vit/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import copy
 
 from vit import env
 from vit.util import clear_screen, string_to_args
 
 DEFAULT_CONFIRM = 'Press Enter to continue...'
 
-class Command(object):
+class Command:
 
     def __init__(self, config):
         self.config = config
         self.env = env.user.copy()
         self.env['TASKRC'] = self.config.taskrc_path
 
     def run(self, command, capture_output=False, custom_env={}):
```

### Comparing `vit-2.2.0b1/vit/readline.py` & `vit-2.3.0/vit/readline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import string
 import re
 
-class Readline(object):
+class Readline:
     def __init__(self, edit_obj):
         self.edit_obj = edit_obj
         word_chars = string.ascii_letters + string.digits + "_"
         self._word_regex1 = re.compile(
             "([%s]+)" % "|".join(re.escape(ch) for ch in word_chars)
         )
         self._word_regex2 = re.compile(
```

### Comparing `vit-2.2.0b1/vit/registry.py` & `vit-2.3.0/vit/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 
-class ActionRegistrar(object):
+class ActionRegistrar:
     def __init__(self, registry):
         self.registry = registry
         self.uuid = uuid.uuid4()
 
     def register(self, name, description):
         self.registry.register(self.uuid, name, description)
 
@@ -13,15 +13,15 @@
             self.registry.deregister(name)
         else:
             any(self.registry.deregister(action) for _, action in self.actions().items())
 
     def actions(self):
         return self.registry.get_registered(self.uuid)
 
-class ActionRegistry(object):
+class ActionRegistry:
     def __init__(self):
         self.actions = {}
         self.noop_action_name = 'NOOP'
 
     def get_registrar(self):
         return ActionRegistrar(self)
 
@@ -44,15 +44,15 @@
 
     def make_action_name(self, name):
         return 'ACTION_%s' % name
 
     def noop(self):
         pass
 
-class RequestReply(object):
+class RequestReply:
     def __init__(self):
         self.handlers = {}
 
     def set_handler(self, name, description, callback):
         self.handlers[name] = {
             'description': description,
             'callback': callback,
```

### Comparing `vit-2.2.0b1/vit/task.py` & `vit-2.3.0/vit/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import tasklib
 from tasklib.task import Task
 from tasklib.backends import TaskWarriorException
 
 from vit import util
 from vit.exception import VitException
 
-class TaskListModel(object):
+class TaskListModel:
     def __init__(self, task_config, reports, report=None, data_location=None):
 
         if not data_location:
             data_location = task_config.subtree('data.location')
         self.data_location = os.path.expanduser(data_location)
         self.tw = tasklib.TaskWarrior(self.data_location)
         self.reports = reports
```

### Comparing `vit-2.2.0b1/vit/task_list.py` & `vit-2.3.0/vit/task_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 
 import urwid
 
 from vit import util
 from vit.base_list_box import BaseListBox
 from vit.list_batcher import ListBatcher
 from vit.formatter.project import Project as ProjectFormatter
+from vit.util import unicode_len
+
 
 REDUCE_COLUMN_WIDTH_LIMIT = 20
 COLUMN_PADDING = 2
 MARKER_COLUMN_NAME = 'markers'
 
-class TaskTable(object):
+class TaskTable:
 
     def __init__(self, config, task_config, formatter, screen, on_select=None, event=None, action_manager=None, request_reply=None, markers=None, draw_screen_callback=None):
         self.config = config
         self.task_config = task_config
         self.formatter = formatter
         self.screen = screen
         self.on_select = on_select
@@ -147,18 +149,22 @@
             self.listbox.previous_focus_position = None
 
     def update_focus_attr(self, attr, position=None):
         if position is None:
             position = self.listbox.focus_position
         self.list_walker[position].row.set_attr_map({None: attr})
 
-    def flash_focus(self, repeat_times=2, pause_seconds=0.1):
+    def flash_focus(self, repeat_times=None, pause_seconds=None):
+        if repeat_times is None:
+            repeat_times = self.config.get_flash_focus_repeat_times()
+        if pause_seconds is None:
+            pause_seconds = self.config.get_flash_focus_pause_seconds()
         if self.listbox.focus:
             position = self.listbox.focus_position if self.listbox.focus_position is not None else self.listbox.previous_focus_position if self.listbox.previous_focus_position is not None else None
-            if position is not None:
+            if position is not None and repeat_times > 0:
                 self.update_focus_attr('flash on', position)
                 self.draw_screen()
                 for i in repeat(None, repeat_times):
                     sleep(pause_seconds)
                     self.update_focus_attr('flash off', position)
                     self.draw_screen()
                     sleep(pause_seconds)
@@ -244,15 +250,15 @@
         if new_width > current_width:
             self.columns[idx]['width'] = new_width
 
     def build_row_column(self, formatted_value):
         if isinstance(formatted_value, tuple):
             return formatted_value
         else:
-            width = len(formatted_value) if formatted_value else 0
+            width = unicode_len(formatted_value) if formatted_value else 0
             return width, formatted_value
 
     def subproject_indentable(self):
         return self.config.subproject_indentable and self.report['subproject_indentable']
 
     def inject_project_placeholders(self, task):
         project = task['project']
@@ -325,15 +331,15 @@
         to_adjust = list(map(lambda c: c.update({'percentage': c['ratio'] / ratio_total}) or c, to_adjust))
         for c in to_adjust:
             adjusted_width = c['width'] - math.ceil(reduce_by * c['percentage'])
             self.columns[c['idx']]['width'] = adjusted_width if adjusted_width > REDUCE_COLUMN_WIDTH_LIMIT else REDUCE_COLUMN_WIDTH_LIMIT
 
     def reconcile_column_width_for_label(self):
         for idx, column in enumerate(self.columns):
-            label_len = len(column['label'])
+            label_len = unicode_len(column['label'])
             if column['width'] < label_len:
                 self.columns[idx]['width'] = label_len
 
     def get_alt_row_background_modifier(self):
         return '.striped-table-row'
 
     def task_row_striping_reset(self):
@@ -384,23 +390,23 @@
 
     def size_changed(self, data):
         self.update_header(data['new_size'])
         grew = self.rows_size_grew(data)
         if grew > 0:
             self.batcher.add(grew)
 
-class TaskRow():
+class TaskRow:
     def __init__(self, task, data, alt_row):
         self.task = task
         self.data = data
         self.alt_row = alt_row
         self.uuid = self.task['uuid']
         self.id = self.task['id']
 
-class ProjectRow():
+class ProjectRow:
     def __init__(self, project, placeholder, alt_row):
         self.project = project
         self.placeholder = placeholder
         self.alt_row = alt_row
 
 class SelectableRow(urwid.WidgetWrap):
     """Wraps 'urwid.Columns' to make it selectable.
```

### Comparing `vit-2.2.0b1/vit/theme/classic.py` & `vit-2.3.0/vit/theme/classic.py`

 * *Files identical despite different names*

### Comparing `vit-2.2.0b1/vit/theme/default.py` & `vit-2.3.0/vit/theme/default.py`

 * *Files identical despite different names*

### Comparing `vit-2.2.0b1/vit/util.py` & `vit-2.3.0/vit/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import sys
 import curses
 import shlex
 from functools import reduce
 
+from urwid.str_util import calc_width
+
 curses.setupterm()
 e3_seq = curses.tigetstr('E3') or b''
 clear_screen_seq = curses.tigetstr('clear') or b''
 
 def clear_screen():
     os.write(sys.stdout.fileno(), e3_seq + clear_screen_seq)
 
@@ -51,7 +53,10 @@
 
 def file_to_class_name(file_name):
     words = file_name.split('_')
     return ''.join((w.capitalize() for w in words))
 
 def file_readable(filepath):
     return os.path.isfile(filepath) and os.access(filepath, os.R_OK)
+
+def unicode_len(string):
+    return calc_width(string, 0, len(string))
```

### Comparing `vit-2.2.0b1/vit.egg-info/PKG-INFO` & `vit-2.3.0/vit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: vit
-Version: 2.2.0b1
+Version: 2.3.0
 Summary: Visual Interactive Taskwarrior full-screen terminal interface
 Home-page: https://github.com/vit-project/vit
 Author: Chad Phillips
 Author-email: chad@apartmentlines.com
-License: UNKNOWN
 Keywords: taskwarrior,console,tui,text-user-interface
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Natural Language :: English
 Classifier: Topic :: Text Processing :: General
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # VIT
 
 <img src="images/great-tit-square-small.png" alt="Logo" width="150" height="150" align="right" />
@@ -39,15 +37,15 @@
  * Multiple/customizable themes
  * Override/customize column formatters
  * Intelligent sub-project indenting
 
 ## Requirements
 
  * [Taskwarrior](https://taskwarrior.org)
- * [Python](https://www.python.org) 3.5+
+ * [Python](https://www.python.org) 3.7+
  * [pip](https://pypi.org/project/pip)
 
 ## Installation
 
 Follow the directions in [INSTALL.md](https://github.com/vit-project/vit/blob/2.x/INSTALL.md)
 
 ## Quick start
@@ -81,9 +79,7 @@
 
 ##### In tribute
 
  Our friend and collaborator Steve Rader passed away in May 2013.  We owe a lot to Steve for his excellent work, and so vit is preserved, maintained and continued.
 
  Taskwarrior Team
  support@taskwarrior.org
-
-
```

### Comparing `vit-2.2.0b1/vit.egg-info/SOURCES.txt` & `vit-2.3.0/vit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 vit/key_cache.py
 vit/keybinding_parser.py
 vit/list_batcher.py
 vit/loader.py
 vit/markers.py
 vit/multi_widget.py
 vit/option_parser.py
+vit/pid_manager.py
 vit/process.py
 vit/readline.py
 vit/registry.py
 vit/task.py
 vit/task_list.py
 vit/uda.py
 vit/util.py
```

