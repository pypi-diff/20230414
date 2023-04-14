# Comparing `tmp/moodlepy-0.8.1.tar.gz` & `tmp/moodlepy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moodlepy-0.8.1.tar", last modified: Thu Sep 17 04:52:48 2020, max compression
+gzip compressed data, was "moodlepy-0.9.0.tar", last modified: Thu Sep 17 15:39:03 2020, max compression
```

## Comparing `moodlepy-0.8.1.tar` & `moodlepy-0.9.0.tar`

### file list

```diff
@@ -1,113 +1,114 @@
--rw-r--r--   0        0        0     1090 2020-09-03 07:06:14.121239 moodlepy-0.8.1/LICENSE
--rw-r--r--   0        0        0     1090 2020-09-03 07:06:14.121239 moodlepy-0.8.1/LICENSE
--rw-r--r--   0        0        0      832 2020-09-08 15:23:54.192259 moodlepy-0.8.1/moodle/__init__.py
--rw-r--r--   0        0        0      149 2020-09-03 15:06:12.635444 moodlepy-0.8.1/moodle/__main__.py
--rw-r--r--   0        0        0       91 2020-09-04 14:39:24.778674 moodlepy-0.8.1/moodle/auth/__init__.py
--rw-r--r--   0        0        0      991 2020-09-04 14:56:14.931565 moodlepy-0.8.1/moodle/auth/auth.py
--rw-r--r--   0        0        0       56 2020-09-04 14:38:37.668303 moodlepy-0.8.1/moodle/auth/email/__init__.py
--rw-r--r--   0        0        0      591 2020-09-04 12:46:29.069941 moodlepy-0.8.1/moodle/auth/email/base.py
--rw-r--r--   0        0        0        0 2020-09-03 15:06:12.635444 moodlepy-0.8.1/moodle/base/__init__.py
--rw-r--r--   0        0        0      392 2020-09-07 15:21:51.035831 moodlepy-0.8.1/moodle/base/base_moodle.py
--rw-r--r--   0        0        0      677 2020-09-08 04:29:59.021261 moodlepy-0.8.1/moodle/base/moodle_object.py
--rw-r--r--   0        0        0      104 2020-09-15 15:43:41.226635 moodlepy-0.8.1/moodle/base/name_value.py
--rw-r--r--   0        0        0      950 2020-09-03 15:06:12.643444 moodlepy-0.8.1/moodle/base/preference/__init__.py
--rw-r--r--   0        0        0      256 2020-09-03 15:06:12.644444 moodlepy-0.8.1/moodle/base/preference/notification_component.py
--rw-r--r--   0        0        0      132 2020-09-03 15:06:12.645445 moodlepy-0.8.1/moodle/base/preference/notification_info.py
--rw-r--r--   0        0        0      275 2020-09-03 15:06:12.645445 moodlepy-0.8.1/moodle/base/preference/notification_processor.py
--rw-r--r--   0        0        0      269 2020-09-03 15:06:12.646443 moodlepy-0.8.1/moodle/base/preference/preference_component.py
--rw-r--r--   0        0        0      184 2020-09-03 15:06:12.647445 moodlepy-0.8.1/moodle/base/preference/preference_processor.py
--rw-r--r--   0        0        0      105 2020-09-03 15:06:12.648443 moodlepy-0.8.1/moodle/base/preference/preference_user.py
--rw-r--r--   0        0        0      710 2020-09-06 07:24:55.582268 moodlepy-0.8.1/moodle/base/responses.py
--rw-r--r--   0        0        0      250 2020-09-05 12:34:00.716022 moodlepy-0.8.1/moodle/base/warning.py
--rw-r--r--   0        0        0      131 2020-09-06 01:58:34.409588 moodlepy-0.8.1/moodle/config.py
--rw-r--r--   0        0        0      687 2020-09-08 17:58:51.515432 moodlepy-0.8.1/moodle/core/__init__.py
--rw-r--r--   0        0        0      210 2020-09-05 13:17:01.820997 moodlepy-0.8.1/moodle/core/badges/__init__.py
--rw-r--r--   0        0        0     3137 2020-09-05 13:44:19.137798 moodlepy-0.8.1/moodle/core/badges/badge.py
--rw-r--r--   0        0        0     1655 2020-09-05 16:21:12.993020 moodlepy-0.8.1/moodle/core/badges/base.py
--rw-r--r--   0        0        0      163 2020-09-06 01:35:02.433979 moodlepy-0.8.1/moodle/core/block/__init__.py
--rw-r--r--   0        0        0     1595 2020-09-06 02:22:02.426811 moodlepy-0.8.1/moodle/core/block/base.py
--rw-r--r--   0        0        0     2793 2020-09-10 12:30:33.878250 moodlepy-0.8.1/moodle/core/block/block.py
--rw-r--r--   0        0        0      204 2020-09-06 03:02:44.131800 moodlepy-0.8.1/moodle/core/blog/__init__.py
--rw-r--r--   0        0        0     1552 2020-09-06 03:18:07.515743 moodlepy-0.8.1/moodle/core/blog/base.py
--rw-r--r--   0        0        0     6034 2020-09-06 08:59:50.803549 moodlepy-0.8.1/moodle/core/blog/blog_entry.py
--rw-r--r--   0        0        0      390 2020-09-06 03:10:53.433283 moodlepy-0.8.1/moodle/core/blog/view_entry.py
--rw-r--r--   0        0        0      939 2020-09-10 15:22:07.932989 moodlepy-0.8.1/moodle/core/calendar/__init__.py
--rw-r--r--   0        0        0      624 2020-09-10 13:47:22.294015 moodlepy-0.8.1/moodle/core/calendar/access_information.py
--rw-r--r--   0        0        0      400 2020-09-10 13:48:20.797774 moodlepy-0.8.1/moodle/core/calendar/allowed_event_types.py
--rw-r--r--   0        0        0     7023 2020-09-10 15:31:27.945197 moodlepy-0.8.1/moodle/core/calendar/base.py
--rw-r--r--   0        0        0     7802 2020-09-10 15:26:18.493389 moodlepy-0.8.1/moodle/core/calendar/course_event.py
--rw-r--r--   0        0        0      658 2020-09-10 15:01:16.079419 moodlepy-0.8.1/moodle/core/calendar/date_view.py
--rw-r--r--   0        0        0     1353 2020-09-10 15:26:38.504659 moodlepy-0.8.1/moodle/core/calendar/day_view.py
--rw-r--r--   0        0        0     4731 2020-09-10 15:43:20.269994 moodlepy-0.8.1/moodle/core/calendar/event.py
--rw-r--r--   0        0        0     3073 2020-09-10 15:20:52.429736 moodlepy-0.8.1/moodle/core/calendar/monthly_view.py
--rw-r--r--   0        0        0      658 2020-09-10 15:04:18.869733 moodlepy-0.8.1/moodle/core/calendar/period.py
--rw-r--r--   0        0        0       58 2020-09-04 14:44:52.560234 moodlepy-0.8.1/moodle/core/cohort/__init__.py
--rw-r--r--   0        0        0     1016 2020-09-04 14:23:28.082007 moodlepy-0.8.1/moodle/core/cohort/base.py
--rw-r--r--   0        0        0       60 2020-09-04 14:45:11.865402 moodlepy-0.8.1/moodle/core/comment/__init__.py
--rw-r--r--   0        0        0      410 2020-09-04 14:30:56.418227 moodlepy-0.8.1/moodle/core/comment/base.py
--rw-r--r--   0        0        0       66 2020-09-04 15:09:45.227799 moodlepy-0.8.1/moodle/core/competency/__init__.py
--rw-r--r--   0        0        0    14447 2020-09-04 15:14:21.512688 moodlepy-0.8.1/moodle/core/competency/base.py
--rw-r--r--   0        0        0     1846 2020-09-08 17:58:51.515432 moodlepy-0.8.1/moodle/core/core.py
--rw-r--r--   0        0        0      836 2020-09-17 04:41:21.649837 moodlepy-0.8.1/moodle/core/course/__init__.py
--rw-r--r--   0        0        0      741 2020-09-15 15:38:32.119958 moodlepy-0.8.1/moodle/core/course/activity_overview.py
--rw-r--r--   0        0        0    11353 2020-09-17 04:47:14.225617 moodlepy-0.8.1/moodle/core/course/base.py
--rw-r--r--   0        0        0     2467 2020-09-06 07:10:45.800289 moodlepy-0.8.1/moodle/core/course/category.py
--rw-r--r--   0        0        0     1491 2020-09-06 07:05:33.677854 moodlepy-0.8.1/moodle/core/course/check_updates.py
--rw-r--r--   0        0        0     6001 2020-09-15 16:12:58.750733 moodlepy-0.8.1/moodle/core/course/content.py
--rw-r--r--   0        0        0     1153 2020-09-15 15:46:52.767480 moodlepy-0.8.1/moodle/core/course/content_option.py
--rw-r--r--   0        0        0     6452 2020-09-17 04:43:12.761811 moodlepy-0.8.1/moodle/core/course/course.py
--rw-r--r--   0        0        0     3098 2020-09-15 17:00:20.645887 moodlepy-0.8.1/moodle/core/course/course_module.py
--rw-r--r--   0        0        0     1074 2020-09-15 16:40:18.069896 moodlepy-0.8.1/moodle/core/course/navigation_option.py
--rw-r--r--   0        0        0      216 2020-09-15 16:53:49.750747 moodlepy-0.8.1/moodle/core/course/view.py
--rw-r--r--   0        0        0       60 2020-09-04 14:45:58.334826 moodlepy-0.8.1/moodle/core/message/__init__.py
--rw-r--r--   0        0        0      590 2020-09-05 16:21:53.232445 moodlepy-0.8.1/moodle/core/message/base.py
--rw-r--r--   0        0        0      384 2020-09-08 17:14:05.494779 moodlepy-0.8.1/moodle/core/notes/__init__.py
--rw-r--r--   0        0        0     2164 2020-09-08 17:19:56.922675 moodlepy-0.8.1/moodle/core/notes/base.py
--rw-r--r--   0        0        0      871 2020-09-08 16:52:23.668589 moodlepy-0.8.1/moodle/core/notes/course_note.py
--rw-r--r--   0        0        0     1033 2020-09-08 17:49:09.381965 moodlepy-0.8.1/moodle/core/notes/course_notes.py
--rw-r--r--   0        0        0     1312 2020-09-08 18:00:07.912098 moodlepy-0.8.1/moodle/core/notes/note.py
--rw-r--r--   0        0        0      839 2020-09-08 16:52:56.525692 moodlepy-0.8.1/moodle/core/notes/personal_note.py
--rw-r--r--   0        0        0      831 2020-09-08 17:17:17.055590 moodlepy-0.8.1/moodle/core/notes/site_note.py
--rw-r--r--   0        0        0      355 2020-09-08 17:04:49.673984 moodlepy-0.8.1/moodle/core/notes/view_notes.py
--rw-r--r--   0        0        0       54 2020-09-04 14:46:07.664663 moodlepy-0.8.1/moodle/core/user/__init__.py
--rw-r--r--   0        0        0      430 2020-09-05 16:23:16.194097 moodlepy-0.8.1/moodle/core/user/base.py
--rw-r--r--   0        0        0      108 2020-09-04 14:46:50.207232 moodlepy-0.8.1/moodle/core/webservice/__init__.py
--rw-r--r--   0        0        0      166 2020-09-03 15:06:12.663444 moodlepy-0.8.1/moodle/core/webservice/advanced_feature.py
--rw-r--r--   0        0        0      387 2020-09-05 16:23:38.857657 moodlepy-0.8.1/moodle/core/webservice/base.py
--rw-r--r--   0        0        0      101 2020-09-03 15:06:12.668444 moodlepy-0.8.1/moodle/core/webservice/function.py
--rw-r--r--   0        0        0      721 2020-09-03 15:06:12.668444 moodlepy-0.8.1/moodle/core/webservice/info.py
--rw-r--r--   0        0        0      625 2020-09-05 13:56:36.915890 moodlepy-0.8.1/moodle/exception.py
--rw-r--r--   0        0        0     4331 2020-09-15 15:40:21.273725 moodlepy-0.8.1/moodle/mdl.py
--rw-r--r--   0        0        0      134 2020-09-11 13:55:21.156392 moodlepy-0.8.1/moodle/mod/__init__.py
--rw-r--r--   0        0        0      670 2020-09-12 16:01:01.830119 moodlepy-0.8.1/moodle/mod/assign/__init__.py
--rw-r--r--   0        0        0     1526 2020-09-11 13:53:47.788506 moodlepy-0.8.1/moodle/mod/assign/advance_grading_data.py
--rw-r--r--   0        0        0     5661 2020-09-15 15:23:16.781922 moodlepy-0.8.1/moodle/mod/assign/assignment.py
--rw-r--r--   0        0        0    10000 2020-09-15 17:01:50.708206 moodlepy-0.8.1/moodle/mod/assign/base.py
--rw-r--r--   0        0        0     2430 2020-09-11 12:29:18.166089 moodlepy-0.8.1/moodle/mod/assign/grade.py
--rw-r--r--   0        0        0     5069 2020-09-11 13:53:42.596506 moodlepy-0.8.1/moodle/mod/assign/participant.py
--rw-r--r--   0        0        0      645 2020-09-11 11:31:53.045400 moodlepy-0.8.1/moodle/mod/assign/plugin_data.py
--rw-r--r--   0        0        0      945 2020-09-11 13:38:16.554324 moodlepy-0.8.1/moodle/mod/assign/user_flag.py
--rw-r--r--   0        0        0      304 2020-09-11 13:50:09.270276 moodlepy-0.8.1/moodle/mod/assign/view.py
--rw-r--r--   0        0        0       93 2020-09-04 14:53:41.379457 moodlepy-0.8.1/moodle/mod/forum/__init__.py
--rw-r--r--   0        0        0      509 2020-09-15 15:11:28.577904 moodlepy-0.8.1/moodle/mod/forum/base.py
--rw-r--r--   0        0        0     3735 2020-09-08 04:00:10.317071 moodlepy-0.8.1/moodle/mod/forum/forum.py
--rw-r--r--   0        0        0      389 2020-09-11 13:56:02.961904 moodlepy-0.8.1/moodle/mod/mod.py
--rw-r--r--   0        0        0      106 2020-09-04 14:34:38.740478 moodlepy-0.8.1/moodle/tool/__init__.py
--rw-r--r--   0        0        0      504 2020-09-06 08:56:46.739016 moodlepy-0.8.1/moodle/tool/mobile/__init__.py
--rw-r--r--   0        0        0     3594 2020-09-06 08:58:14.142768 moodlepy-0.8.1/moodle/tool/mobile/base.py
--rw-r--r--   0        0        0      536 2020-09-06 08:56:46.739016 moodlepy-0.8.1/moodle/tool/mobile/config.py
--rw-r--r--   0        0        0     2689 2020-09-06 08:44:11.254566 moodlepy-0.8.1/moodle/tool/mobile/content.py
--rw-r--r--   0        0        0     1432 2020-09-06 08:14:22.876349 moodlepy-0.8.1/moodle/tool/mobile/function.py
--rw-r--r--   0        0        0      493 2020-09-06 08:57:52.881518 moodlepy-0.8.1/moodle/tool/mobile/key.py
--rw-r--r--   0        0        0      240 2020-09-03 15:06:12.678444 moodlepy-0.8.1/moodle/tool/mobile/plugin.py
--rw-r--r--   0        0        0      817 2020-09-03 15:06:12.679443 moodlepy-0.8.1/moodle/tool/mobile/public_config.py
--rw-r--r--   0        0        0      258 2020-09-04 14:36:24.543582 moodlepy-0.8.1/moodle/tool/tool.py
--rw-r--r--   0        0        0        0 2020-09-03 15:06:12.682444 moodlepy-0.8.1/moodle/utils/__init__.py
--rw-r--r--   0        0        0      338 2020-09-03 15:06:12.683444 moodlepy-0.8.1/moodle/utils/decorator.py
--rw-r--r--   0        0        0     1099 2020-09-06 02:01:36.758889 moodlepy-0.8.1/moodle/utils/helper.py
--rw-r--r--   0        0        0       23 2020-09-17 04:49:59.957528 moodlepy-0.8.1/moodle/version.py
--rw-r--r--   0        0        0      774 2020-09-17 04:49:32.361116 moodlepy-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     6396 2020-09-10 15:25:35.853389 moodlepy-0.8.1/README.md
--rw-r--r--   0        0        0     6396 2020-09-10 15:25:35.853389 moodlepy-0.8.1/README.md
--rw-r--r--   0        0        0     7673 2020-09-17 04:52:49.589639 moodlepy-0.8.1/setup.py
--rw-r--r--   0        0        0     6895 2020-09-17 04:52:49.590639 moodlepy-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2020-09-03 07:06:14.121239 moodlepy-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1090 2020-09-03 07:06:14.121239 moodlepy-0.9.0/LICENSE
+-rw-r--r--   0        0        0      879 2020-09-17 15:08:15.520955 moodlepy-0.9.0/moodle/__init__.py
+-rw-r--r--   0        0        0      149 2020-09-03 15:06:12.635444 moodlepy-0.9.0/moodle/__main__.py
+-rw-r--r--   0        0        0       91 2020-09-04 14:39:24.778674 moodlepy-0.9.0/moodle/auth/__init__.py
+-rw-r--r--   0        0        0      991 2020-09-04 14:56:14.931565 moodlepy-0.9.0/moodle/auth/auth.py
+-rw-r--r--   0        0        0       56 2020-09-04 14:38:37.668303 moodlepy-0.9.0/moodle/auth/email/__init__.py
+-rw-r--r--   0        0        0      591 2020-09-04 12:46:29.069941 moodlepy-0.9.0/moodle/auth/email/base.py
+-rw-r--r--   0        0        0        0 2020-09-03 15:06:12.635444 moodlepy-0.9.0/moodle/base/__init__.py
+-rw-r--r--   0        0        0      392 2020-09-07 15:21:51.035831 moodlepy-0.9.0/moodle/base/base_moodle.py
+-rw-r--r--   0        0        0      677 2020-09-08 04:29:59.021261 moodlepy-0.9.0/moodle/base/moodle_object.py
+-rw-r--r--   0        0        0      104 2020-09-15 15:43:41.226635 moodlepy-0.9.0/moodle/base/name_value.py
+-rw-r--r--   0        0        0      950 2020-09-03 15:06:12.643444 moodlepy-0.9.0/moodle/base/preference/__init__.py
+-rw-r--r--   0        0        0      256 2020-09-03 15:06:12.644444 moodlepy-0.9.0/moodle/base/preference/notification_component.py
+-rw-r--r--   0        0        0      132 2020-09-03 15:06:12.645445 moodlepy-0.9.0/moodle/base/preference/notification_info.py
+-rw-r--r--   0        0        0      275 2020-09-03 15:06:12.645445 moodlepy-0.9.0/moodle/base/preference/notification_processor.py
+-rw-r--r--   0        0        0      269 2020-09-03 15:06:12.646443 moodlepy-0.9.0/moodle/base/preference/preference_component.py
+-rw-r--r--   0        0        0      184 2020-09-03 15:06:12.647445 moodlepy-0.9.0/moodle/base/preference/preference_processor.py
+-rw-r--r--   0        0        0      105 2020-09-03 15:06:12.648443 moodlepy-0.9.0/moodle/base/preference/preference_user.py
+-rw-r--r--   0        0        0      710 2020-09-06 07:24:55.582268 moodlepy-0.9.0/moodle/base/responses.py
+-rw-r--r--   0        0        0      250 2020-09-05 12:34:00.716022 moodlepy-0.9.0/moodle/base/warning.py
+-rw-r--r--   0        0        0      131 2020-09-06 01:58:34.409588 moodlepy-0.9.0/moodle/config.py
+-rw-r--r--   0        0        0      687 2020-09-08 17:58:51.515432 moodlepy-0.9.0/moodle/core/__init__.py
+-rw-r--r--   0        0        0      210 2020-09-05 13:17:01.820997 moodlepy-0.9.0/moodle/core/badges/__init__.py
+-rw-r--r--   0        0        0     3137 2020-09-05 13:44:19.137798 moodlepy-0.9.0/moodle/core/badges/badge.py
+-rw-r--r--   0        0        0     1655 2020-09-05 16:21:12.993020 moodlepy-0.9.0/moodle/core/badges/base.py
+-rw-r--r--   0        0        0      163 2020-09-06 01:35:02.433979 moodlepy-0.9.0/moodle/core/block/__init__.py
+-rw-r--r--   0        0        0     1595 2020-09-06 02:22:02.426811 moodlepy-0.9.0/moodle/core/block/base.py
+-rw-r--r--   0        0        0     2793 2020-09-10 12:30:33.878250 moodlepy-0.9.0/moodle/core/block/block.py
+-rw-r--r--   0        0        0      204 2020-09-06 03:02:44.131800 moodlepy-0.9.0/moodle/core/blog/__init__.py
+-rw-r--r--   0        0        0     1552 2020-09-17 15:00:17.719402 moodlepy-0.9.0/moodle/core/blog/base.py
+-rw-r--r--   0        0        0     6034 2020-09-06 08:59:50.803549 moodlepy-0.9.0/moodle/core/blog/blog_entry.py
+-rw-r--r--   0        0        0      390 2020-09-06 03:10:53.433283 moodlepy-0.9.0/moodle/core/blog/view_entry.py
+-rw-r--r--   0        0        0      939 2020-09-10 15:22:07.932989 moodlepy-0.9.0/moodle/core/calendar/__init__.py
+-rw-r--r--   0        0        0      624 2020-09-10 13:47:22.294015 moodlepy-0.9.0/moodle/core/calendar/access_information.py
+-rw-r--r--   0        0        0      400 2020-09-10 13:48:20.797774 moodlepy-0.9.0/moodle/core/calendar/allowed_event_types.py
+-rw-r--r--   0        0        0     7023 2020-09-10 15:31:27.945197 moodlepy-0.9.0/moodle/core/calendar/base.py
+-rw-r--r--   0        0        0     7802 2020-09-10 15:26:18.493389 moodlepy-0.9.0/moodle/core/calendar/course_event.py
+-rw-r--r--   0        0        0      658 2020-09-10 15:01:16.079419 moodlepy-0.9.0/moodle/core/calendar/date_view.py
+-rw-r--r--   0        0        0     1353 2020-09-10 15:26:38.504659 moodlepy-0.9.0/moodle/core/calendar/day_view.py
+-rw-r--r--   0        0        0     4731 2020-09-10 15:43:20.269994 moodlepy-0.9.0/moodle/core/calendar/event.py
+-rw-r--r--   0        0        0     3073 2020-09-10 15:20:52.429736 moodlepy-0.9.0/moodle/core/calendar/monthly_view.py
+-rw-r--r--   0        0        0      658 2020-09-10 15:04:18.869733 moodlepy-0.9.0/moodle/core/calendar/period.py
+-rw-r--r--   0        0        0       58 2020-09-04 14:44:52.560234 moodlepy-0.9.0/moodle/core/cohort/__init__.py
+-rw-r--r--   0        0        0     1016 2020-09-04 14:23:28.082007 moodlepy-0.9.0/moodle/core/cohort/base.py
+-rw-r--r--   0        0        0       60 2020-09-04 14:45:11.865402 moodlepy-0.9.0/moodle/core/comment/__init__.py
+-rw-r--r--   0        0        0      410 2020-09-04 14:30:56.418227 moodlepy-0.9.0/moodle/core/comment/base.py
+-rw-r--r--   0        0        0       66 2020-09-04 15:09:45.227799 moodlepy-0.9.0/moodle/core/competency/__init__.py
+-rw-r--r--   0        0        0    14447 2020-09-04 15:14:21.512688 moodlepy-0.9.0/moodle/core/competency/base.py
+-rw-r--r--   0        0        0     1846 2020-09-08 17:58:51.515432 moodlepy-0.9.0/moodle/core/core.py
+-rw-r--r--   0        0        0      836 2020-09-17 04:41:21.649837 moodlepy-0.9.0/moodle/core/course/__init__.py
+-rw-r--r--   0        0        0      741 2020-09-15 15:38:32.119958 moodlepy-0.9.0/moodle/core/course/activity_overview.py
+-rw-r--r--   0        0        0    11392 2020-09-17 15:24:42.709399 moodlepy-0.9.0/moodle/core/course/base.py
+-rw-r--r--   0        0        0     2467 2020-09-06 07:10:45.800289 moodlepy-0.9.0/moodle/core/course/category.py
+-rw-r--r--   0        0        0     1491 2020-09-06 07:05:33.677854 moodlepy-0.9.0/moodle/core/course/check_updates.py
+-rw-r--r--   0        0        0     6001 2020-09-15 16:12:58.750733 moodlepy-0.9.0/moodle/core/course/content.py
+-rw-r--r--   0        0        0     1153 2020-09-15 15:46:52.767480 moodlepy-0.9.0/moodle/core/course/content_option.py
+-rw-r--r--   0        0        0     6452 2020-09-17 04:43:12.761811 moodlepy-0.9.0/moodle/core/course/course.py
+-rw-r--r--   0        0        0     3098 2020-09-15 17:00:20.645887 moodlepy-0.9.0/moodle/core/course/course_module.py
+-rw-r--r--   0        0        0     1074 2020-09-15 16:40:18.069896 moodlepy-0.9.0/moodle/core/course/navigation_option.py
+-rw-r--r--   0        0        0      216 2020-09-15 16:53:49.750747 moodlepy-0.9.0/moodle/core/course/view.py
+-rw-r--r--   0        0        0       60 2020-09-04 14:45:58.334826 moodlepy-0.9.0/moodle/core/message/__init__.py
+-rw-r--r--   0        0        0      590 2020-09-05 16:21:53.232445 moodlepy-0.9.0/moodle/core/message/base.py
+-rw-r--r--   0        0        0      384 2020-09-08 17:14:05.494779 moodlepy-0.9.0/moodle/core/notes/__init__.py
+-rw-r--r--   0        0        0     2164 2020-09-08 17:19:56.922675 moodlepy-0.9.0/moodle/core/notes/base.py
+-rw-r--r--   0        0        0      871 2020-09-08 16:52:23.668589 moodlepy-0.9.0/moodle/core/notes/course_note.py
+-rw-r--r--   0        0        0     1033 2020-09-08 17:49:09.381965 moodlepy-0.9.0/moodle/core/notes/course_notes.py
+-rw-r--r--   0        0        0     1312 2020-09-08 18:00:07.912098 moodlepy-0.9.0/moodle/core/notes/note.py
+-rw-r--r--   0        0        0      839 2020-09-08 16:52:56.525692 moodlepy-0.9.0/moodle/core/notes/personal_note.py
+-rw-r--r--   0        0        0      831 2020-09-08 17:17:17.055590 moodlepy-0.9.0/moodle/core/notes/site_note.py
+-rw-r--r--   0        0        0      355 2020-09-08 17:04:49.673984 moodlepy-0.9.0/moodle/core/notes/view_notes.py
+-rw-r--r--   0        0        0       54 2020-09-04 14:46:07.664663 moodlepy-0.9.0/moodle/core/user/__init__.py
+-rw-r--r--   0        0        0      430 2020-09-05 16:23:16.194097 moodlepy-0.9.0/moodle/core/user/base.py
+-rw-r--r--   0        0        0      108 2020-09-04 14:46:50.207232 moodlepy-0.9.0/moodle/core/webservice/__init__.py
+-rw-r--r--   0        0        0      166 2020-09-03 15:06:12.663444 moodlepy-0.9.0/moodle/core/webservice/advanced_feature.py
+-rw-r--r--   0        0        0      387 2020-09-05 16:23:38.857657 moodlepy-0.9.0/moodle/core/webservice/base.py
+-rw-r--r--   0        0        0      101 2020-09-03 15:06:12.668444 moodlepy-0.9.0/moodle/core/webservice/function.py
+-rw-r--r--   0        0        0      721 2020-09-03 15:06:12.668444 moodlepy-0.9.0/moodle/core/webservice/info.py
+-rw-r--r--   0        0        0      625 2020-09-05 13:56:36.915890 moodlepy-0.9.0/moodle/exception.py
+-rw-r--r--   0        0        0     4331 2020-09-17 15:08:36.645703 moodlepy-0.9.0/moodle/mdl.py
+-rw-r--r--   0        0        0      134 2020-09-11 13:55:21.156392 moodlepy-0.9.0/moodle/mod/__init__.py
+-rw-r--r--   0        0        0      670 2020-09-12 16:01:01.830119 moodlepy-0.9.0/moodle/mod/assign/__init__.py
+-rw-r--r--   0        0        0     1526 2020-09-11 13:53:47.788506 moodlepy-0.9.0/moodle/mod/assign/advance_grading_data.py
+-rw-r--r--   0        0        0     5661 2020-09-15 15:23:16.781922 moodlepy-0.9.0/moodle/mod/assign/assignment.py
+-rw-r--r--   0        0        0    10000 2020-09-15 17:01:50.708206 moodlepy-0.9.0/moodle/mod/assign/base.py
+-rw-r--r--   0        0        0     2430 2020-09-11 12:29:18.166089 moodlepy-0.9.0/moodle/mod/assign/grade.py
+-rw-r--r--   0        0        0     5069 2020-09-11 13:53:42.596506 moodlepy-0.9.0/moodle/mod/assign/participant.py
+-rw-r--r--   0        0        0      645 2020-09-11 11:31:53.045400 moodlepy-0.9.0/moodle/mod/assign/plugin_data.py
+-rw-r--r--   0        0        0      945 2020-09-11 13:38:16.554324 moodlepy-0.9.0/moodle/mod/assign/user_flag.py
+-rw-r--r--   0        0        0      304 2020-09-11 13:50:09.270276 moodlepy-0.9.0/moodle/mod/assign/view.py
+-rw-r--r--   0        0        0       93 2020-09-04 14:53:41.379457 moodlepy-0.9.0/moodle/mod/forum/__init__.py
+-rw-r--r--   0        0        0      509 2020-09-15 15:11:28.577904 moodlepy-0.9.0/moodle/mod/forum/base.py
+-rw-r--r--   0        0        0     3735 2020-09-08 04:00:10.317071 moodlepy-0.9.0/moodle/mod/forum/forum.py
+-rw-r--r--   0        0        0      389 2020-09-11 13:56:02.961904 moodlepy-0.9.0/moodle/mod/mod.py
+-rw-r--r--   0        0        0      106 2020-09-04 14:34:38.740478 moodlepy-0.9.0/moodle/tool/__init__.py
+-rw-r--r--   0        0        0      504 2020-09-06 08:56:46.739016 moodlepy-0.9.0/moodle/tool/mobile/__init__.py
+-rw-r--r--   0        0        0     3594 2020-09-06 08:58:14.142768 moodlepy-0.9.0/moodle/tool/mobile/base.py
+-rw-r--r--   0        0        0      536 2020-09-06 08:56:46.739016 moodlepy-0.9.0/moodle/tool/mobile/config.py
+-rw-r--r--   0        0        0     2689 2020-09-06 08:44:11.254566 moodlepy-0.9.0/moodle/tool/mobile/content.py
+-rw-r--r--   0        0        0     1432 2020-09-06 08:14:22.876349 moodlepy-0.9.0/moodle/tool/mobile/function.py
+-rw-r--r--   0        0        0      493 2020-09-06 08:57:52.881518 moodlepy-0.9.0/moodle/tool/mobile/key.py
+-rw-r--r--   0        0        0      240 2020-09-03 15:06:12.678444 moodlepy-0.9.0/moodle/tool/mobile/plugin.py
+-rw-r--r--   0        0        0      817 2020-09-03 15:06:12.679443 moodlepy-0.9.0/moodle/tool/mobile/public_config.py
+-rw-r--r--   0        0        0      258 2020-09-04 14:36:24.543582 moodlepy-0.9.0/moodle/tool/tool.py
+-rw-r--r--   0        0        0        0 2020-09-03 15:06:12.682444 moodlepy-0.9.0/moodle/utils/__init__.py
+-rw-r--r--   0        0        0      338 2020-09-03 15:06:12.683444 moodlepy-0.9.0/moodle/utils/decorator.py
+-rw-r--r--   0        0        0     1717 2020-09-17 15:21:50.853678 moodlepy-0.9.0/moodle/utils/helper.py
+-rw-r--r--   0        0        0       40 2020-09-17 14:47:10.628107 moodlepy-0.9.0/moodle/utils/typing.py
+-rw-r--r--   0        0        0       23 2020-09-17 15:30:19.447011 moodlepy-0.9.0/moodle/version.py
+-rw-r--r--   0        0        0      774 2020-09-17 15:29:51.450095 moodlepy-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6396 2020-09-10 15:25:35.853389 moodlepy-0.9.0/README.md
+-rw-r--r--   0        0        0     6396 2020-09-10 15:25:35.853389 moodlepy-0.9.0/README.md
+-rw-r--r--   0        0        0     7673 2020-09-17 15:39:03.894087 moodlepy-0.9.0/setup.py
+-rw-r--r--   0        0        0     6895 2020-09-17 15:39:03.895087 moodlepy-0.9.0/PKG-INFO
```

### Comparing `moodlepy-0.8.1/LICENSE` & `moodlepy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/__init__.py` & `moodlepy-0.9.0/moodle/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .base.base_moodle import BaseMoodle
 from .base.warning import Warning
 from .base.responses import ResponsesFactory
 from .base.preference import (MessagePreference, NotificationPreference,
                               UserPreference)
 
 from .exception import MoodleException
+from .utils.typing import Array
 
 from .tool import Tool
 from .auth import Auth
 from .core import Core
 from .mod import Mod
 from .mdl import Moodle
 
@@ -22,13 +23,14 @@
     'BaseMoodle',
     'Warning',
     'ResponsesFactory',
     'MessagePreference',
     'NotificationPreference',
     'UserPreference',
     'MoodleException',
+    'Array',
     'Auth',
     'Core',
     'Mod',
     'Tool',
     'Moodle',
 ]
```

### Comparing `moodlepy-0.8.1/moodle/auth/auth.py` & `moodlepy-0.9.0/moodle/auth/auth.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/auth/email/base.py` & `moodlepy-0.9.0/moodle/auth/email/base.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/base/moodle_object.py` & `moodlepy-0.9.0/moodle/base/moodle_object.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/base/preference/__init__.py` & `moodlepy-0.9.0/moodle/base/preference/__init__.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/base/responses.py` & `moodlepy-0.9.0/moodle/base/responses.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/__init__.py` & `moodlepy-0.9.0/moodle/core/__init__.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/badges/badge.py` & `moodlepy-0.9.0/moodle/core/badges/badge.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/badges/base.py` & `moodlepy-0.9.0/moodle/core/badges/base.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/block/base.py` & `moodlepy-0.9.0/moodle/core/block/base.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/block/block.py` & `moodlepy-0.9.0/moodle/core/block/block.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/blog/base.py` & `moodlepy-0.9.0/moodle/core/blog/base.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/blog/blog_entry.py` & `moodlepy-0.9.0/moodle/core/blog/blog_entry.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/calendar/__init__.py` & `moodlepy-0.9.0/moodle/core/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/calendar/access_information.py` & `moodlepy-0.9.0/moodle/core/calendar/access_information.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/calendar/base.py` & `moodlepy-0.9.0/moodle/core/calendar/base.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/calendar/course_event.py` & `moodlepy-0.9.0/moodle/core/calendar/course_event.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/calendar/date_view.py` & `moodlepy-0.9.0/moodle/core/calendar/date_view.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/calendar/day_view.py` & `moodlepy-0.9.0/moodle/core/calendar/day_view.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/calendar/event.py` & `moodlepy-0.9.0/moodle/core/calendar/event.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/calendar/monthly_view.py` & `moodlepy-0.9.0/moodle/core/calendar/monthly_view.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/calendar/period.py` & `moodlepy-0.9.0/moodle/core/calendar/period.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/cohort/base.py` & `moodlepy-0.9.0/moodle/core/cohort/base.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/competency/base.py` & `moodlepy-0.9.0/moodle/core/competency/base.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/core.py` & `moodlepy-0.9.0/moodle/core/core.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/course/__init__.py` & `moodlepy-0.9.0/moodle/core/course/__init__.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/course/activity_overview.py` & `moodlepy-0.9.0/moodle/core/course/activity_overview.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/course/base.py` & `moodlepy-0.9.0/moodle/core/course/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List, Optional
-from moodle import BaseMoodle
+from moodle import BaseMoodle, Array
 from moodle.utils.helper import from_dict
 from . import (ActivityOverview, Course, CourseByField, SearchResult,
                CoursesBTC, CheckUpdate, Category, ContentOption, Section,
                CourseModule, NavigationOptions, ViewCourse)
 
 
 class BaseCourse(BaseMoodle):
     def check_updates(self,
                       courseid: int,
                       tocheck: List[CheckUpdate.ToCheck],
-                      filter: List[str] = []) -> CheckUpdate:
+                      filter: Optional[List[str]] = None) -> CheckUpdate:
         """Check if there is updates affecting the user for the given course and contexts.
 
         Args:
             courseid (int): Course id to check
             tocheck (List[CourseToCheck]): Instances to check
             filter (List[str], optional): Check only for updates in these areas. Defaults to [].
 
@@ -118,15 +118,16 @@
 
         Args:
             ids (List[int], optional): List of course id. If empty return all courses except front page course. Defaults to None.
 
         Returns:
             List[Course]: Return course details
         """
-        options = {} if ids is None else {'ids': ids}
+        options = Array(ids if ids else [])
+        options.name = 'ids'
         res = self.moodle.post("core_course_get_courses", options=options)
         return [from_dict(Course, data) for data in res] if res else []
 
     def get_courses_by_field(self,
                              field: str = '',
                              value: str = '') -> CourseByField:
         """Get courses matching a specific field (id/s, shortname, idnumber, category)
```

### Comparing `moodlepy-0.8.1/moodle/core/course/category.py` & `moodlepy-0.9.0/moodle/core/course/category.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/course/check_updates.py` & `moodlepy-0.9.0/moodle/core/course/check_updates.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/course/content.py` & `moodlepy-0.9.0/moodle/core/course/content.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/course/content_option.py` & `moodlepy-0.9.0/moodle/core/course/content_option.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/course/course.py` & `moodlepy-0.9.0/moodle/core/course/course.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/course/course_module.py` & `moodlepy-0.9.0/moodle/core/course/course_module.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/course/navigation_option.py` & `moodlepy-0.9.0/moodle/core/course/navigation_option.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/message/base.py` & `moodlepy-0.9.0/moodle/core/message/base.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/notes/base.py` & `moodlepy-0.9.0/moodle/core/notes/base.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/notes/course_note.py` & `moodlepy-0.9.0/moodle/core/notes/course_note.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/notes/course_notes.py` & `moodlepy-0.9.0/moodle/core/notes/course_notes.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/notes/note.py` & `moodlepy-0.9.0/moodle/core/notes/note.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/notes/personal_note.py` & `moodlepy-0.9.0/moodle/core/notes/personal_note.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/notes/site_note.py` & `moodlepy-0.9.0/moodle/core/notes/site_note.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/core/webservice/info.py` & `moodlepy-0.9.0/moodle/core/webservice/info.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/exception.py` & `moodlepy-0.9.0/moodle/exception.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/mdl.py` & `moodlepy-0.9.0/moodle/mdl.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/mod/assign/__init__.py` & `moodlepy-0.9.0/moodle/mod/assign/__init__.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/mod/assign/advance_grading_data.py` & `moodlepy-0.9.0/moodle/mod/assign/advance_grading_data.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/mod/assign/assignment.py` & `moodlepy-0.9.0/moodle/mod/assign/assignment.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/mod/assign/base.py` & `moodlepy-0.9.0/moodle/mod/assign/base.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/mod/assign/grade.py` & `moodlepy-0.9.0/moodle/mod/assign/grade.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/mod/assign/participant.py` & `moodlepy-0.9.0/moodle/mod/assign/participant.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/mod/assign/plugin_data.py` & `moodlepy-0.9.0/moodle/mod/assign/plugin_data.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/mod/assign/user_flag.py` & `moodlepy-0.9.0/moodle/mod/assign/user_flag.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/mod/forum/forum.py` & `moodlepy-0.9.0/moodle/mod/forum/forum.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/tool/mobile/base.py` & `moodlepy-0.9.0/moodle/tool/mobile/base.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/tool/mobile/config.py` & `moodlepy-0.9.0/moodle/tool/mobile/config.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/tool/mobile/content.py` & `moodlepy-0.9.0/moodle/tool/mobile/content.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/tool/mobile/function.py` & `moodlepy-0.9.0/moodle/tool/mobile/function.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/moodle/tool/mobile/public_config.py` & `moodlepy-0.9.0/moodle/tool/mobile/public_config.py`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/pyproject.toml` & `moodlepy-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "moodlepy"
-version = "0.8.1"
+version = "0.9.0"
 description = "Client for moodle webservice"
 authors = ["hexatester <habibrohman@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/hexatester/moodlepy"
 repository = "https://github.com/hexatester/moodlepy"
 packages = [
```

### Comparing `moodlepy-0.8.1/README.md` & `moodlepy-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `moodlepy-0.8.1/setup.py` & `moodlepy-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ['dacite>=1.5.1,<2.0.0', 'requests>=2.24.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['moodle = moodle.__main__:main']}
 
 setup_kwargs = {
     'name': 'moodlepy',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': 'Client for moodle webservice',
     'long_description': "# moodlepy\n\n[![moodlepy - PyPi](https://img.shields.io/pypi/v/moodlepy)](https://pypi.org/project/moodlepy/)\n[![codecov](https://codecov.io/gh/hexatester/moodlepy/branch/master/graph/badge.svg)](https://codecov.io/gh/hexatester/moodlepy)\n[![BUILD](https://img.shields.io/travis/com/hexatester/moodlepy)](https://travis-ci.com/github/hexatester/moodlepy)\n[![LICENSE](https://img.shields.io/github/license/hexatester/moodlepy)](https://github.com/hexatester/moodlepy/blob/master/LICENSE)\n\nPython client for moodle webservice\n\n## Introduction\n\nThis library provide a pure Python interface for [Moodle Web Service](https://docs.moodle.org/dev/Web_services). It's compatible with Python versions 3.7+\n\n## Installing\n\nYou can install or upgrade moodlepy with:\n\n```bash\npip install moodlepy --upgrade\n```\n\nOr you can install from source with:\n\n```bash\ngit clone https://github.com/hexatester/moodlepy\ncd moodlepy\npython setup.py install\n```\n\n## Usage\n\nExample usage\n\n```python\nfrom moodle import Moodle\nurl = 'https://my.domain/webservice/rest/server.php'\ntoken = 'super secret token'\nmoodle = Moodle(url, token)\nraw_site_info = moodle('core_webservice_get_site_info')\nsite_info = moodle.core.webservice.get_site_info()  # return typed site_info\n\nprint(raw_site_info)\nprint(site_info)\n```\n\nIn the future all [Web service functions](https://docs.moodle.org/dev/Web_service_API_functions) will be covered by moodlepy\n\n# Moodle Web Service support\n\n❗️ Not all types and methods are supported, since moodlepy is not yet released.\nA = Added, W = Work In Progress\n\n| Area                 | Functions | Types | Tests | Status |\n| -------------------- | --------- | ----- | ----- | ------ |\n| auth_email           |           |       |       |        |\n| block                |           |       |       |        |\n| core_auth            |           |       |       |        |\n| core_backup          |           |       |       |        |\n| core_badge           | A         | A     | A     |        |\n| core_blog            | A         | A     | A     |        |\n| core_calendar        | A         | A     |       | W      |\n| core_cohort          |           |       |       |        |\n| core_comment         |           |       |       | W      |\n| core_competency      |           |       |       |        |\n| core_course          |           |       |       | W      |\n| core_customfield     |           |       |       |        |\n| core_enrol           |           |       |       |        |\n| core_fetch           |           |       |       | W      |\n| core_files           |           |       |       | W      |\n| core_filters         |           |       |       |        |\n| core_form            |           |       |       | W      |\n| core_get             |           |       |       | W      |\n| core_grade           |           |       |       | W      |\n| core_grades          |           |       |       |        |\n| core_grading         |           |       |       |        |\n| core_group           |           |       |       |        |\n| core_h5p             |           |       |       |        |\n| core_message         |           |       |       | W      |\n| core_notes           | A         | A     |       | W      |\n| core_output          |           |       |       |        |\n| core_question        | W         |       |       | W      |\n| core_rating          |           |       |       |        |\n| core_role            |           |       |       |        |\n| core_search          |           |       |       | W      |\n| core_session         |           |       |       | W      |\n| core_tag             |           |       |       |        |\n| core_update          |           |       |       |        |\n| core_user            |           |       |       | W      |\n| core_webservice      | A         | A     | A     | A      |\n| enrol_guest          |           |       |       |        |\n| enrol_manual         |           |       |       |        |\n| enrol_self           |           |       |       |        |\n| gradereport_overview |           |       |       |        |\n| gradereport_user     |           |       |       |        |\n| gradingform_guide    |           |       |       |        |\n| gradingform_rubric   |           |       |       |        |\n| local_mobile         |           |       |       | W      |\n| message_airnotifier  |           |       |       | W      |\n| message_popup        |           |       |       | W      |\n| mod_assign           |           |       |       | W      |\n| mod_book             |           |       |       |        |\n| mod_chat             |           |       |       | W      |\n| mod_choice           |           |       |       |        |\n| mod_data             |           |       |       |        |\n| mod_feedback         |           |       |       |        |\n| mod_folder           |           |       |       |        |\n| mod_forum            |           |       |       | W      |\n| mod_glossary         |           |       |       |        |\n| mod_imscp            |           |       |       |        |\n| mod_label            |           |       |       |        |\n| mod_lesson           |           |       |       | W      |\n| mod_lti              |           |       |       |        |\n| mod_page             |           |       |       | W      |\n| mod_quiz             |           |       |       | W      |\n| mod_resource         |           |       |       |        |\n| mod_scorm            |           |       |       |        |\n| mod_survey           |           |       |       | W      |\n| mod_url              |           |       |       | W      |\n| mod_wiki             |           |       |       |        |\n| mod_workshop         |           |       |       |        |\n| report_competency    |           |       |       |        |\n| report_insights      |           |       |       |        |\n| tool_analytics       |           |       |       |        |\n| tool_lp              |           |       |       |        |\n| tool_mobile          | A         | A     |       | W      |\n| tool_templatelibrary |           |       |       |        |\n| tool_usertours       |           |       |       |        |\n| tool_xmldb           |           |       |       |        |\n",
     'author': 'hexatester',
     'author_email': 'habibrohman@protonmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/hexatester/moodlepy',
```

### Comparing `moodlepy-0.8.1/PKG-INFO` & `moodlepy-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodlepy
-Version: 0.8.1
+Version: 0.9.0
 Summary: Client for moodle webservice
 Home-page: https://github.com/hexatester/moodlepy
 License: MIT
 Author: hexatester
 Author-email: habibrohman@protonmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

