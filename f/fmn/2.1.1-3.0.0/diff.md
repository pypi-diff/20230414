# Comparing `tmp/fmn-2.1.1.tar.gz` & `tmp/fmn-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fmn-2.1.1.tar", last modified: Thu Apr  5 15:41:38 2018, max compression
+gzip compressed data, was "fmn-3.0.0.tar", max compression
```

## Comparing `fmn-2.1.1.tar` & `fmn-3.0.0.tar`

### file list

```diff
@@ -1,278 +1,74 @@
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/alembic/
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/alembic/versions/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      425 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/167e0e6dd4e5_make_code_path_longer.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      429 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/18ebf3181f87_add_a_negated_column_for_rules.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1695 2018-03-28 19:02:28.000000 fmn-2.1.1/alembic/versions/1b6e419ea1a6_add_threshold1_to_existing_prefs.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1939 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/1be98d56336_drop_the_mention_rule_from_the_defaults.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1355 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/2136a1f22f1f_cull_removed_rules.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1651 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/226fd58fe7e5_ignore_taskotron_messages_in_the_main_.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      459 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/24533471e302_add_the_verbose_column.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      542 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/2ea9623b21fa_add_an_active_field_to_filter.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      775 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/33082c0ecf3f_add_presentation_booleans.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1578 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/362efe8fd524_add_new_masher_rules.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1829 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/38c9c18d342e_add_new_mdapi_rule.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1180 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/3de9ad66862f_cascade_removed_rules_to_filters.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      459 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/4a95022fd7f3_add_another_presentation_boolean.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1997 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/5403906cbd9f_add_new_taskotron_filter.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      440 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/59ee93c4bf71_add_the_oneshot_column.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2469 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/versions/9987c7c958c7_get_ci_error_messages.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1087 2018-04-05 15:06:39.000000 fmn-2.1.1/alembic/versions/c369fd8ee75c_replace_pkgdb_package_with_git_repo_new.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)       38 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/README
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1902 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/env.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      412 2017-12-14 00:12:22.000000 fmn-2.1.1/alembic/script.py.mako
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/apache/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      356 2017-12-14 00:12:22.000000 fmn-2.1.1/apache/fmn.web.conf
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      469 2017-12-14 00:12:22.000000 fmn-2.1.1/apache/fmn.web.wsgi
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fedmsg.d/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1954 2017-12-14 00:12:22.000000 fmn-2.1.1/fedmsg.d/base.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1861 2018-04-02 19:27:12.000000 fmn-2.1.1/fedmsg.d/endpoints.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)       92 2017-12-14 00:12:22.000000 fmn-2.1.1/fedmsg.d/fas_credentials.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1308 2017-12-14 00:12:22.000000 fmn-2.1.1/fedmsg.d/logging.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      157 2017-12-14 00:12:22.000000 fmn-2.1.1/fedmsg.d/rabbitmq.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1363 2017-12-14 00:12:22.000000 fmn-2.1.1/fedmsg.d/sse.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2320 2017-12-14 00:12:22.000000 fmn-2.1.1/fedmsg.d/ssl.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      106 2017-12-14 00:12:22.000000 fmn-2.1.1/fedmsg.d/testconfig.py
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/delivery/
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/delivery/backends/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      805 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/delivery/backends/__init__.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     3514 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/delivery/backends/android.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2822 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/delivery/backends/base.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2485 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/delivery/backends/debug.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    18626 2018-01-19 14:47:54.000000 fmn-2.1.1/fmn/delivery/backends/irc.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     4046 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/delivery/backends/mail.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     5260 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/delivery/backends/sse.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      805 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/delivery/__init__.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     9286 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/delivery/service.py
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/lib/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     9119 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/lib/__init__.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2732 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/lib/db.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    11668 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/lib/defaults.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2825 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/lib/hinting.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    31707 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/lib/models.py
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/rules/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     3145 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/__init__.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     7764 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/anitya.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1412 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/ansible.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2395 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/askbot.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2868 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/autocloud.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     9420 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/bodhi.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1051 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/bugzilla.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     8641 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/buildsys.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     8433 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/ci.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     8625 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/compose.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2835 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/coprs.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     6140 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/faf.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     3127 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/fas.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1291 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/fedbadges.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     3573 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/fedimg.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     3381 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/fedocal.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2033 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/fedora_elections.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2531 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/fedoratagger.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1633 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/fmn_notifications.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     7047 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/rules/generic.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     3960 2018-04-02 20:52:25.000000 fmn-2.1.1/fmn/rules/git.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     4991 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/github.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1228 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/greenwave.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2227 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/hotness.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      511 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/infragit.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2222 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/jenkins.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1211 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/kerneltest.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      951 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/koschei.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      449 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/logger.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      477 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/mailman.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2215 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/mbs.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      689 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/mdapi.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     4792 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/meetbot.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      370 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/nagios.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1999 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/nuancier.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     9692 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/pagure.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     7321 2018-03-28 18:55:26.000000 fmn-2.1.1/fmn/rules/pkgdb.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      445 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/planet.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1674 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/summershum.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     5379 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/taskotron.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     3574 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/trac.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    15265 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/utils.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1202 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/rules/wiki.py
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/sse/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      840 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/sse/__init__.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    13515 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/sse/server.py
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/docs/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     3907 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/docs/about.rst
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.1-dist/
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.1-dist/css/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    19791 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.1-dist/css/bootstrap-theme.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    17706 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.1-dist/css/bootstrap-theme.min.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   125975 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.1-dist/css/bootstrap.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   102593 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.1-dist/css/bootstrap.min.css
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.1-dist/fonts/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    20290 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.1-dist/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    62850 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.1-dist/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    41236 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.1-dist/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    23292 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.1-dist/fonts/glyphicons-halflings-regular.woff
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.1-dist/js/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    58411 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.1-dist/js/bootstrap.js
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    27832 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.1-dist/js/bootstrap.min.js
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.2-fedora/
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.2-fedora/css/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    19791 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.2-fedora/css/bootstrap-theme.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    17730 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.2-fedora/css/bootstrap-theme.min.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   126293 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.2-fedora/css/bootstrap.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   102818 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.2-fedora/css/bootstrap.min.css
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.2-fedora/fonts/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    20290 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.2-fedora/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    62850 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.2-fedora/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    41236 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.2-fedora/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    23292 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.2-fedora/fonts/glyphicons-halflings-regular.woff
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.2-fedora/js/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    58605 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.2-fedora/js/bootstrap.js
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    27881 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.0.2-fedora/js/bootstrap.min.js
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/css/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    14948 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/css/bootstrap-theme.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    38388 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/css/bootstrap-theme.css.map
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    13197 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/css/bootstrap-theme.min.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   121338 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/css/bootstrap.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   246329 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/css/bootstrap.css.map
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   100021 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/css/bootstrap.min.css
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/fonts/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    20335 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    62927 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    41280 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    23320 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/fonts/glyphicons-halflings-regular.woff
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/js/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    55258 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/js/bootstrap.js
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    29110 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.1.1-fedora/js/bootstrap.min.js
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/css/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    26123 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/css/bootstrap-theme.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    47285 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/css/bootstrap-theme.css.map
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    23351 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/css/bootstrap-theme.min.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   146035 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/css/bootstrap.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   388829 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/css/bootstrap.css.map
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   121182 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/css/bootstrap.min.css
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/fonts/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    20127 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   108738 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    45404 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    23424 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    18028 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/fonts/glyphicons-halflings-regular.woff2
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/js/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    67589 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/js/bootstrap.js
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    35969 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/js/bootstrap.min.js
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      484 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap-3.3.4-fedora/js/npm.js
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap/
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap/css/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    26123 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap/css/bootstrap-theme.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    47285 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap/css/bootstrap-theme.css.map
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    23351 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap/css/bootstrap-theme.min.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   146035 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap/css/bootstrap.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   388829 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap/css/bootstrap.css.map
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   121182 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap/css/bootstrap.min.css
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap/fonts/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    20127 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   108738 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    45404 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    23424 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    18028 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/bootstrap/js/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    67589 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap/js/bootstrap.js
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    35969 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap/js/bootstrap.min.js
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      484 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/bootstrap/js/npm.js
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/css/
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/css/fonts/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    24734 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-Bold-webfont.eot
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    28113 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-Bold-webfont.svg
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    49276 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-Bold-webfont.ttf
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    16708 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-Bold-webfont.woff
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    27450 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-BoldOblique-webfont.eot
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    29130 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-BoldOblique-webfont.svg
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    52200 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-BoldOblique-webfont.ttf
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    17988 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-BoldOblique-webfont.woff
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    27610 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-Oblique-webfont.eot
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    29402 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-Oblique-webfont.svg
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    50068 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-Oblique-webfont.ttf
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    17980 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-Oblique-webfont.woff
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    24350 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-Regular-webfont.eot
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    28095 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-Regular-webfont.svg
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    47504 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-Regular-webfont.ttf
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    16400 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Cantarell-Regular-webfont.woff
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    94588 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Comfortaa_Bold-webfont.eot
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   171329 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Comfortaa_Bold-webfont.svg
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   170608 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Comfortaa_Bold-webfont.ttf
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    56608 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Comfortaa_Bold-webfont.woff
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    91164 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Comfortaa_Regular-webfont.eot
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   169419 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Comfortaa_Regular-webfont.svg
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   170388 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Comfortaa_Regular-webfont.ttf
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    54684 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Comfortaa_Regular-webfont.woff
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    95020 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Comfortaa_Thin-webfont.eot
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   167898 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Comfortaa_Thin-webfont.svg
--rw-rw-r--   0 jcline    (1000) jcline    (1000)   170308 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Comfortaa_Thin-webfont.ttf
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    56100 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/fonts/Comfortaa_Thin-webfont.woff
--rw-rw-r--   0 jcline    (1000) jcline    (1000)       54 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/avatars.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      330 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/footer.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      748 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/navbar.css
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2519 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/css/text.css
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/ico/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    38078 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/ico/favicon.ico
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/img/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     4077 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/img/spinner.gif
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/static/js/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    93107 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/js/jquery-1.10.2.min.js
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     3283 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/static/js/site.js
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn/web/templates/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)        0 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/templates/__init__.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    28931 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/templates/context.html
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      152 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/templates/docs.html
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    11779 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/templates/filter.html
--rw-rw-r--   0 jcline    (1000) jcline    (1000)        0 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/templates/functions.html
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1256 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/templates/index.html
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      755 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/templates/login.html
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     7236 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/templates/master.html
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     4333 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/templates/profile.html
--rw-rw-r--   0 jcline    (1000) jcline    (1000)       24 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/__init__.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    37307 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/app.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      118 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/converters.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      315 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/default_config.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1956 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/forms.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      266 2017-12-14 00:12:23.000000 fmn-2.1.1/fmn/web/main.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)        0 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/__init__.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1641 2018-01-02 17:07:37.000000 fmn-2.1.1/fmn/celery.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    20700 2018-01-02 19:03:58.000000 fmn-2.1.1/fmn/config.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      986 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/constants.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     8636 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/consumer.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     3491 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/dogpile_backports.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      960 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/exceptions.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     4295 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/fmn_fasshim.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    23122 2018-04-02 20:35:45.000000 fmn-2.1.1/fmn/formatters.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    18759 2018-01-19 14:47:54.000000 fmn-2.1.1/fmn/tasks.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1251 2017-12-14 00:12:22.000000 fmn-2.1.1/fmn/util.py
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn.egg-info/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2063 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn.egg-info/PKG-INFO
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     9211 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn.egg-info/SOURCES.txt
--rw-rw-r--   0 jcline    (1000) jcline    (1000)        1 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn.egg-info/dependency_links.txt
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      126 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn.egg-info/entry_points.txt
--rw-rw-r--   0 jcline    (1000) jcline    (1000)        1 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn.egg-info/not-zip-safe
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      363 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn.egg-info/requires.txt
--rw-rw-r--   0 jcline    (1000) jcline    (1000)        4 2018-04-05 15:41:38.000000 fmn-2.1.1/fmn.egg-info/top_level.txt
-drwxrwxr-x   0 jcline    (1000) jcline    (1000)        0 2018-04-05 15:41:38.000000 fmn-2.1.1/systemd/
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      269 2017-12-14 00:12:23.000000 fmn-2.1.1/systemd/fmn-backend@.service
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      273 2017-12-14 00:12:23.000000 fmn-2.1.1/systemd/fmn-celerybeat.service
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      311 2017-12-14 00:12:23.000000 fmn-2.1.1/systemd/fmn-digests@.service
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      311 2017-12-14 00:12:23.000000 fmn-2.1.1/systemd/fmn-sse-python2@.service
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      313 2017-12-14 00:12:23.000000 fmn-2.1.1/systemd/fmn-sse-python3@.service
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      336 2017-12-14 00:12:23.000000 fmn-2.1.1/systemd/fmn-worker@.service
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     9399 2018-04-05 15:40:08.000000 fmn-2.1.1/CHANGELOG.rst
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    17998 2017-12-14 00:12:01.000000 fmn-2.1.1/COPYING
--rw-rw-r--   0 jcline    (1000) jcline    (1000)    26434 2017-12-14 00:12:01.000000 fmn-2.1.1/COPYING.LESSER
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      344 2017-12-14 00:12:01.000000 fmn-2.1.1/MANIFEST.in
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     1028 2017-12-14 00:12:01.000000 fmn-2.1.1/README.rst
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      966 2017-12-14 00:12:01.000000 fmn-2.1.1/alembic.ini
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      144 2017-12-14 00:12:01.000000 fmn-2.1.1/dev-requirements.txt
--rw-rw-r--   0 jcline    (1000) jcline    (1000)      364 2017-12-21 16:06:12.000000 fmn-2.1.1/requirements.txt
--rw-rw-r--   0 jcline    (1000) jcline    (1000)       70 2018-04-05 15:41:38.000000 fmn-2.1.1/setup.cfg
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2116 2018-04-05 15:40:17.000000 fmn-2.1.1/setup.py
--rw-rw-r--   0 jcline    (1000) jcline    (1000)     2063 2018-04-05 15:41:38.000000 fmn-2.1.1/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-04-11 07:21:10.424342 fmn-3.0.0/LICENSES/
+-rw-r--r--   0        0        0      371 2023-04-11 07:21:10.424342 fmn-3.0.0/README.md
+-rw-r--r--   0        0        0      147 2023-04-14 14:59:26.264728 fmn-3.0.0/fmn/__init__.py
+-rw-r--r--   0        0        0      134 2023-04-11 07:21:10.427342 fmn-3.0.0/fmn/api/__init__.py
+-rw-r--r--   0        0        0     2870 2023-04-11 07:21:10.427342 fmn-3.0.0/fmn/api/api_models.py
+-rw-r--r--   0        0        0     4293 2023-04-11 07:21:10.427342 fmn-3.0.0/fmn/api/auth.py
+-rw-r--r--   0        0        0      572 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/api/cli.py
+-rw-r--r--   0        0        0      999 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/api/database.py
+-rw-r--r--   0        0        0      142 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/api/handlers/__init__.py
+-rw-r--r--   0        0        0     2399 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/api/handlers/admin.py
+-rw-r--r--   0        0        0     3721 2023-04-14 11:57:03.281691 fmn-3.0.0/fmn/api/handlers/misc.py
+-rw-r--r--   0        0        0     9484 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/api/handlers/users.py
+-rw-r--r--   0        0        0      849 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/api/handlers/utils.py
+-rw-r--r--   0        0        0     1780 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/api/main.py
+-rw-r--r--   0        0        0     1298 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/api/messaging.py
+-rw-r--r--   0        0        0      221 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/backends/__init__.py
+-rw-r--r--   0        0        0     4008 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/backends/base.py
+-rw-r--r--   0        0        0     4151 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/backends/fasjson.py
+-rw-r--r--   0        0        0     9950 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/backends/pagure.py
+-rwxr-xr-x   0        0        0      647 2022-12-07 14:09:37.810248 fmn-3.0.0/fmn/boop.py_
+-rw-r--r--   0        0        0      143 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/cache/__init__.py
+-rw-r--r--   0        0        0     2168 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/cache/base.py
+-rw-r--r--   0        0        0     2476 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/cache/cli.py
+-rw-r--r--   0        0        0     1494 2023-04-11 07:21:10.428342 fmn-3.0.0/fmn/cache/rules.py
+-rw-r--r--   0        0        0     2478 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/cache/tracked.py
+-rw-r--r--   0        0        0     1994 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/cache/util.py
+-rw-r--r--   0        0        0      140 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/consumer/__init__.py
+-rw-r--r--   0        0        0     5083 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/consumer/consumer.py
+-rw-r--r--   0        0        0     1756 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/consumer/send_queue.py
+-rw-r--r--   0        0        0        0 2022-07-25 11:53:57.387926 fmn-3.0.0/fmn/core/__init__.py
+-rw-r--r--   0        0        0      621 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/core/amqp.py
+-rw-r--r--   0        0        0     1780 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/core/cli.py
+-rw-r--r--   0        0        0     3195 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/core/config.py
+-rw-r--r--   0        0        0      522 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/core/constants.py
+-rw-r--r--   0        0        0      165 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/core/version.py
+-rw-r--r--   0        0        0      272 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/database/__init__.py
+-rw-r--r--   0        0        0     1818 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/database/cli.py
+-rw-r--r--   0        0        0     3509 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/database/main.py
+-rw-r--r--   0        0        0        0 2022-10-11 16:56:08.025575 fmn-3.0.0/fmn/database/migrations/__init__.py
+-rw-r--r--   0        0        0     2149 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/database/migrations/env.py
+-rw-r--r--   0        0        0     3309 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/database/migrations/main.py
+-rw-r--r--   0        0        0      625 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/database/migrations/script.py.mako
+-rw-r--r--   0        0        0        0 2022-09-09 14:50:44.870927 fmn-3.0.0/fmn/database/migrations/versions/.empty
+-rw-r--r--   0        0        0     1150 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/database/migrations/versions/59e22969e199_add_generated_table.py
+-rw-r--r--   0        0        0      448 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/database/migrations/versions/7b47f8356d9f_initial_empty_migration.py
+-rw-r--r--   0        0        0      589 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/database/migrations/versions/85ea1d6c9a3f_rule_name_is_optional.py
+-rw-r--r--   0        0        0      764 2023-04-11 07:21:10.429342 fmn-3.0.0/fmn/database/migrations/versions/a6c12ef04ee5_create_rule_disabled.py
+-rw-r--r--   0        0        0      322 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/database/model/__init__.py
+-rw-r--r--   0        0        0     1679 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/database/model/destination.py
+-rw-r--r--   0        0        0     1403 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/database/model/filter.py
+-rw-r--r--   0        0        0      734 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/database/model/generated.py
+-rw-r--r--   0        0        0     1572 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/database/model/generation_rule.py
+-rw-r--r--   0        0        0     2530 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/database/model/rule.py
+-rw-r--r--   0        0        0     1531 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/database/model/tracking_rule.py
+-rw-r--r--   0        0        0      437 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/database/model/user.py
+-rw-r--r--   0        0        0     1491 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/database/setup.py
+-rw-r--r--   0        0        0        0 2022-12-05 10:09:40.216949 fmn-3.0.0/fmn/messages/__init__.py
+-rw-r--r--   0        0        0      337 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/messages/base.py
+-rw-r--r--   0        0        0     1863 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/messages/rule.py
+-rw-r--r--   0        0        0        0 2022-11-09 16:53:28.036186 fmn-3.0.0/fmn/rules/__init__.py
+-rw-r--r--   0        0        0     1723 2023-04-14 11:57:03.281691 fmn-3.0.0/fmn/rules/filter.py
+-rw-r--r--   0        0        0     1136 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/rules/notification.py
+-rw-r--r--   0        0        0      659 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/rules/requester.py
+-rw-r--r--   0        0        0     4566 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/rules/tracking_rules.py
+-rw-r--r--   0        0        0        0 2022-09-09 14:50:44.870927 fmn-3.0.0/fmn/sender/__init__.py
+-rw-r--r--   0        0        0     1757 2023-04-14 13:06:18.454302 fmn-3.0.0/fmn/sender/cli.py
+-rw-r--r--   0        0        0     1731 2023-04-11 07:21:10.430342 fmn-3.0.0/fmn/sender/config.py
+-rw-r--r--   0        0        0     1887 2023-04-14 13:06:18.454302 fmn-3.0.0/fmn/sender/consumer.py
+-rw-r--r--   0        0        0     1150 2023-04-11 07:21:10.431342 fmn-3.0.0/fmn/sender/email.py
+-rw-r--r--   0        0        0      855 2023-04-14 13:06:18.454302 fmn-3.0.0/fmn/sender/handler.py
+-rw-r--r--   0        0        0     3591 2023-04-14 13:06:18.454302 fmn-3.0.0/fmn/sender/irc.py
+-rw-r--r--   0        0        0     3194 2023-04-11 07:21:10.431342 fmn-3.0.0/fmn/sender/matrix.py
+-rw-r--r--   0        0        0     7629 2023-04-14 15:01:04.471319 fmn-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4214 1970-01-01 00:00:00.000000 fmn-3.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fmn-2.1.1/alembic/env.py` & `fmn-3.0.0/fmn/database/migrations/env.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,71 @@
-from __future__ import with_statement
+# SPDX-FileCopyrightText: Contributors to the Fedora Project
+#
+# SPDX-License-Identifier: MIT
+
 from alembic import context
 from sqlalchemy import engine_from_config, pool
-from logging.config import fileConfig
+
+# Alembic imports this module in a way that it can’t do relative imports from outside the
+# fmn/database/migrations directory, therefore it has to use absolute imports.
+from fmn.database.main import metadata
 
 # this is the Alembic Config object, which provides
 # access to the values within the .ini file in use.
-config = context.config
-
-# Interpret the config file for Python logging.
-# This line sets up loggers basically.
-fileConfig(config.config_file_name)
+alembic_config = context.config
 
-import fmn.lib.models
-target_metadata = fmn.lib.models.BASE.metadata
+# add your model's MetaData object here
+# for 'autogenerate' support
+target_metadata = metadata
 
 # other values from the config, defined by the needs of env.py,
 # can be acquired:
-# my_important_option = config.get_main_option("my_important_option")
+# my_important_option = alembic_config.get_main_option("my_important_option")
 # ... etc.
 
-def run_migrations_offline():
+
+def run_migrations_offline():  # pragma: no cover
     """Run migrations in 'offline' mode.
 
     This configures the context with just a URL
     and not an Engine, though an Engine is acceptable
     here as well.  By skipping the Engine creation
     we don't even need a DBAPI to be available.
 
     Calls to context.execute() here emit the given string to the
     script output.
-
     """
-    url = config.get_main_option("sqlalchemy.url")
-    context.configure(url=url)
+    url = alembic_config.get_main_option("sqlalchemy.url")
+    context.configure(
+        url=url,
+        target_metadata=target_metadata,
+        literal_binds=True,
+        dialect_opts={"paramstyle": "named"},
+    )
 
     with context.begin_transaction():
         context.run_migrations()
 
+
 def run_migrations_online():
     """Run migrations in 'online' mode.
 
     In this scenario we need to create an Engine
     and associate a connection with the context.
-
     """
-    engine = engine_from_config(
-                config.get_section(config.config_ini_section),
-                prefix='sqlalchemy.',
-                poolclass=pool.NullPool)
+    connectable = engine_from_config(
+        alembic_config.get_section(alembic_config.config_ini_section),
+        prefix="sqlalchemy.",
+        poolclass=pool.NullPool,
+    )
 
-    connection = engine.connect()
-    context.configure(
-                connection=connection,
-                target_metadata=target_metadata
-                )
+    with connectable.connect() as connection:
+        context.configure(connection=connection, target_metadata=target_metadata)
 
-    try:
         with context.begin_transaction():
             context.run_migrations()
-    finally:
-        connection.close()
 
-if context.is_offline_mode():
+
+if context.is_offline_mode():  # pragma: no cover
     run_migrations_offline()
 else:
     run_migrations_online()
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fmn-2.1.1/fedmsg.d/logging.py` & `fmn-3.0.0/fmn/sender/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,62 @@
-# Setup fedmsg logging.
-# See the following for constraints on this format http://bit.ly/Xn1WDn
-config = dict(
-    logging=dict(
-        version=1,
-        formatters=dict(
-            bare={
-                "datefmt": "%Y-%m-%d %H:%M:%S",
-                "format": "[%(asctime)s][%(name)10s %(levelname)7s] %(message)s"
-            },
-        ),
-        handlers=dict(
-            console={
+# SPDX-FileCopyrightText: Contributors to the Fedora Project
+#
+# SPDX-License-Identifier: MIT
+
+import logging
+import logging.config
+from importlib import import_module
+
+import tomli
+
+_log = logging.getLogger(__name__)
+
+
+DEFAULTS = dict(
+    amqp_url="amqp://?connection_attempts=3&retry_delay=5",
+    queue="fmn",
+    handler={
+        "class": "fmn.sender.handler:PrintHandler",
+    },
+    log_config={
+        "version": 1,
+        "disable_existing_loggers": False,
+        "formatters": {"simple": {"format": "[%(name)s %(levelname)s] %(message)s"}},
+        "handlers": {
+            "console": {
                 "class": "logging.StreamHandler",
-                "formatter": "bare",
-                "level": "DEBUG",
+                "formatter": "simple",
                 "stream": "ext://sys.stdout",
             }
-        ),
-        loggers=dict(
-            fedmsg={
-                "level": "DEBUG",
-                "propagate": False,
-                "handlers": ["console"],
-            },
-            fmn={
-                "level": "DEBUG",
-                "propagate": False,
-                "handlers": ["console"],
-            },
-            moksha={
-                "level": "DEBUG",
+        },
+        "loggers": {
+            "fmn": {
+                "level": "INFO",
                 "propagate": False,
                 "handlers": ["console"],
-            },
-        ),
+            }
+        },
         # The root logger configuration; this is a catch-all configuration
         # that applies to all log messages not handled by a different logger
-        root={
-            'level': 'INFO',
-            'handlers': ['console'],
-        },
-    ),
+        "root": {"level": "WARNING", "handlers": ["console"]},
+    },
 )
+
+
+def get_config(path):
+    with open(path, "rb") as fh:
+        config = tomli.load(fh)
+    for key, value in DEFAULTS.items():
+        if key not in config:
+            config[key] = value
+    return config
+
+
+def get_handler(config):
+    handler_module_path, handler_class_name = config["handler"]["class"].split(":", 1)
+    handler_module = import_module(handler_module_path)
+    handler_class = getattr(handler_module, handler_class_name)
+    return handler_class(config["handler"])
+
+
+def setup_logging(config):
+    logging.config.dictConfig(config["log_config"])
```

