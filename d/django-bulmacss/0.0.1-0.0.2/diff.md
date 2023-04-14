# Comparing `tmp/django-bulmacss-0.0.1.tar.gz` & `tmp/django-bulmacss-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bulmacss-0.0.1.tar", last modified: Fri Apr 14 02:30:27 2023, max compression
+gzip compressed data, was "django-bulmacss-0.0.2.tar", last modified: Fri Apr 14 05:54:17 2023, max compression
```

## Comparing `django-bulmacss-0.0.1.tar` & `django-bulmacss-0.0.2.tar`

### file list

```diff
@@ -1,189 +1,190 @@
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.343842 django-bulmacss-0.0.1/
--rw-r--r--   0 chen      (1000) chen      (1000)     1063 2022-05-27 08:19:55.000000 django-bulmacss-0.0.1/LICENSE
--rw-r--r--   0 chen      (1000) chen      (1000)      103 2023-04-14 02:04:21.000000 django-bulmacss-0.0.1/MANIFEST.in
--rw-r--r--   0 chen      (1000) chen      (1000)     1473 2023-04-14 02:30:27.343842 django-bulmacss-0.0.1/PKG-INFO
--rw-r--r--   0 chen      (1000) chen      (1000)      599 2023-04-14 02:22:38.000000 django-bulmacss-0.0.1/README.rst
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.323841 django-bulmacss-0.0.1/bulma/
--rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-27 08:10:38.000000 django-bulmacss-0.0.1/bulma/__init__.py
--rw-r--r--   0 chen      (1000) chen      (1000)       63 2022-05-27 08:10:38.000000 django-bulmacss-0.0.1/bulma/admin.py
--rw-r--r--   0 chen      (1000) chen      (1000)      142 2022-05-27 08:10:38.000000 django-bulmacss-0.0.1/bulma/apps.py
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.323841 django-bulmacss-0.0.1/bulma/migrations/
--rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-27 08:10:38.000000 django-bulmacss-0.0.1/bulma/migrations/__init__.py
--rw-r--r--   0 chen      (1000) chen      (1000)       57 2022-05-27 08:10:38.000000 django-bulmacss-0.0.1/bulma/models.py
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.320508 django-bulmacss-0.0.1/bulma/static/
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.323841 django-bulmacss-0.0.1/bulma/static/bulma/
--rw-r--r--   0 chen      (1000) chen      (1000)   259362 2023-04-14 01:36:45.000000 django-bulmacss-0.0.1/bulma/static/bulma/bulma.min.css
--rw-r--r--   0 chen      (1000) chen      (1000)    75779 2023-04-14 01:38:28.000000 django-bulmacss-0.0.1/bulma/static/bulma/feather.min.js
--rw-r--r--   0 chen      (1000) chen      (1000)    80886 2023-04-14 01:38:28.000000 django-bulmacss-0.0.1/bulma/static/bulma/feather.min.js.map
--rw-r--r--   0 chen      (1000) chen      (1000)     8907 2023-04-14 01:38:38.000000 django-bulmacss-0.0.1/bulma/static/bulma/jdenticon.min.js
--rw-r--r--   0 chen      (1000) chen      (1000)    82680 2023-04-14 01:38:38.000000 django-bulmacss-0.0.1/bulma/static/bulma/jdenticon.min.js.map
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.327175 django-bulmacss-0.0.1/bulma/templates/
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.330508 django-bulmacss-0.0.1/bulma/templates/account/
--rw-r--r--   0 chen      (1000) chen      (1000)      342 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/account_inactive.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1004 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/base.html
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.330508 django-bulmacss-0.0.1/bulma/templates/account/email/
--rw-r--r--   0 chen      (1000) chen      (1000)      342 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/email/base_message.txt
--rw-r--r--   0 chen      (1000) chen      (1000)      484 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/email/email_confirmation_message.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       61 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/email/email_confirmation_signup_message.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       61 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/email/email_confirmation_signup_subject.txt
--rw-r--r--   0 chen      (1000) chen      (1000)      127 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/email/email_confirmation_subject.txt
--rw-r--r--   0 chen      (1000) chen      (1000)      530 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/email/password_reset_key_message.txt
--rw-r--r--   0 chen      (1000) chen      (1000)      114 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/email/password_reset_key_subject.txt
--rw-r--r--   0 chen      (1000) chen      (1000)     2902 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/email.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1143 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/email_confirm.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1565 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/index.html
--rw-r--r--   0 chen      (1000) chen      (1000)     2997 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/login.html
--rw-r--r--   0 chen      (1000) chen      (1000)      716 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/logout.html
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.330508 django-bulmacss-0.0.1/bulma/templates/account/messages/
--rw-r--r--   0 chen      (1000) chen      (1000)      110 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/messages/cannot_delete_primary_email.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       90 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/messages/email_confirmation_sent.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       81 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/messages/email_confirmed.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       85 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/messages/email_deleted.txt
--rw-r--r--   0 chen      (1000) chen      (1000)      138 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/messages/logged_in.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       72 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/messages/logged_out.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       82 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/messages/password_changed.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       78 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/messages/password_set.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       79 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/messages/primary_email_set.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       97 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/messages/unverified_primary_email.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       83 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/password_change.html
--rw-r--r--   0 chen      (1000) chen      (1000)      842 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/password_reset.html
--rw-r--r--   0 chen      (1000) chen      (1000)      554 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/password_reset_done.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1149 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/password_reset_from_key.html
--rw-r--r--   0 chen      (1000) chen      (1000)      343 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/password_reset_from_key_done.html
--rw-r--r--   0 chen      (1000) chen      (1000)      441 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/password_set.html
--rw-r--r--   0 chen      (1000) chen      (1000)      849 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/settings.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1177 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/signup.html
--rw-r--r--   0 chen      (1000) chen      (1000)      264 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/signup_closed.html
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.330508 django-bulmacss-0.0.1/bulma/templates/account/snippets/
--rw-r--r--   0 chen      (1000) chen      (1000)      204 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/snippets/already_logged_in.html
--rw-r--r--   0 chen      (1000) chen      (1000)      437 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/verification_sent.html
--rw-r--r--   0 chen      (1000) chen      (1000)      919 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/account/verified_email_required.html
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.333841 django-bulmacss-0.0.1/bulma/templates/accounts/
--rw-r--r--   0 chen      (1000) chen      (1000)      495 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/accounts/group_list.html
--rw-r--r--   0 chen      (1000) chen      (1000)      852 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/accounts/login_by_invite.html
--rw-r--r--   0 chen      (1000) chen      (1000)      676 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/accounts/phone_change.html
--rw-r--r--   0 chen      (1000) chen      (1000)      328 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/accounts/profile.html
--rw-r--r--   0 chen      (1000) chen      (1000)      617 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/accounts/set_password.html
--rw-r--r--   0 chen      (1000) chen      (1000)     3680 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/accounts/settings.html
--rw-r--r--   0 chen      (1000) chen      (1000)      812 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/accounts/signup_by_invite.html
--rw-r--r--   0 chen      (1000) chen      (1000)      277 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/accounts/tabs.html
--rw-r--r--   0 chen      (1000) chen      (1000)      736 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/accounts/user_confirm_delete.html
--rw-r--r--   0 chen      (1000) chen      (1000)      716 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/accounts/user_form.html
--rw-r--r--   0 chen      (1000) chen      (1000)     2819 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/accounts/user_list.html
--rw-r--r--   0 chen      (1000) chen      (1000)      371 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/accounts/user_tree.html
--rw-r--r--   0 chen      (1000) chen      (1000)     3363 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/accounts/user_tree_input.html
--rw-r--r--   0 chen      (1000) chen      (1000)      173 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/attrs.html
--rw-r--r--   0 chen      (1000) chen      (1000)      421 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/avatar.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1383 2023-04-14 01:37:49.000000 django-bulmacss-0.0.1/bulma/templates/base.html
--rw-r--r--   0 chen      (1000) chen      (1000)      342 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/breadcrumb.html
--rw-r--r--   0 chen      (1000) chen      (1000)      830 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/console.html
--rw-r--r--   0 chen      (1000) chen      (1000)      626 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/dir_tree.html
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.320508 django-bulmacss-0.0.1/bulma/templates/django/
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.333841 django-bulmacss-0.0.1/bulma/templates/django/forms/
--rw-r--r--   0 chen      (1000) chen      (1000)      165 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/attrs.html
--rw-r--r--   0 chen      (1000) chen      (1000)      609 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/default.html
--rw-r--r--   0 chen      (1000) chen      (1000)      874 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/div.html
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.323841 django-bulmacss-0.0.1/bulma/templates/django/forms/errors/
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.333841 django-bulmacss-0.0.1/bulma/templates/django/forms/errors/dict/
--rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/errors/dict/default.html
--rw-r--r--   0 chen      (1000) chen      (1000)      113 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/errors/dict/text.txt
--rw-r--r--   0 chen      (1000) chen      (1000)      137 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/errors/dict/ul.html
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.333841 django-bulmacss-0.0.1/bulma/templates/django/forms/errors/list/
--rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/errors/list/default.html
--rw-r--r--   0 chen      (1000) chen      (1000)       52 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/errors/list/text.txt
--rw-r--r--   0 chen      (1000) chen      (1000)      200 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/errors/list/ul.html
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.337175 django-bulmacss-0.0.1/bulma/templates/django/forms/formsets/
--rw-r--r--   0 chen      (1000) chen      (1000)       77 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/formsets/default.html
--rw-r--r--   0 chen      (1000) chen      (1000)       82 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/formsets/p.html
--rw-r--r--   0 chen      (1000) chen      (1000)       86 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/formsets/table.html
--rw-r--r--   0 chen      (1000) chen      (1000)       83 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/formsets/ul.html
--rw-r--r--   0 chen      (1000) chen      (1000)      128 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/label.html
--rw-r--r--   0 chen      (1000) chen      (1000)      684 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/p.html
--rw-r--r--   0 chen      (1000) chen      (1000)      825 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/table.html
--rw-r--r--   0 chen      (1000) chen      (1000)      723 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/ul.html
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.340508 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/
--rw-r--r--   0 chen      (1000) chen      (1000)      172 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/attrs.html
--rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/checkbox.html
--rw-r--r--   0 chen      (1000) chen      (1000)      506 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/checkbox_option.html
--rw-r--r--   0 chen      (1000) chen      (1000)      510 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/checkbox_select.html
--rw-r--r--   0 chen      (1000) chen      (1000)      511 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/clearable_file_input.html
--rw-r--r--   0 chen      (1000) chen      (1000)       65 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/date.html
--rw-r--r--   0 chen      (1000) chen      (1000)      183 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/datetime.html
--rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/email.html
--rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/file.html
--rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/hidden.html
--rw-r--r--   0 chen      (1000) chen      (1000)      259 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/input.html
--rw-r--r--   0 chen      (1000) chen      (1000)      219 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/input_option.html
--rw-r--r--   0 chen      (1000) chen      (1000)       54 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/multiple_hidden.html
--rw-r--r--   0 chen      (1000) chen      (1000)      426 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/multiple_input.html
--rw-r--r--   0 chen      (1000) chen      (1000)      146 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/multiwidget.html
--rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/number.html
--rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/password.html
--rw-r--r--   0 chen      (1000) chen      (1000)       57 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/radio.html
--rw-r--r--   0 chen      (1000) chen      (1000)       55 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/radio_option.html
--rw-r--r--   0 chen      (1000) chen      (1000)      465 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/select.html
--rw-r--r--   0 chen      (1000) chen      (1000)       54 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/select_date.html
--rw-r--r--   0 chen      (1000) chen      (1000)      127 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/select_option.html
--rw-r--r--   0 chen      (1000) chen      (1000)       54 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/splitdatetime.html
--rw-r--r--   0 chen      (1000) chen      (1000)       54 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/splithiddendatetime.html
--rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/text.html
--rw-r--r--   0 chen      (1000) chen      (1000)      194 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/textarea.html
--rw-r--r--   0 chen      (1000) chen      (1000)       65 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/time.html
--rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/django/forms/widgets/url.html
--rw-r--r--   0 chen      (1000) chen      (1000)       84 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/empty.html
--rw-r--r--   0 chen      (1000) chen      (1000)      343 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/field_display.html
--rw-r--r--   0 chen      (1000) chen      (1000)      662 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/field_horizontal.html
--rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-27 08:10:38.000000 django-bulmacss-0.0.1/bulma/templates/file_line.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1995 2023-04-14 01:27:02.000000 django-bulmacss-0.0.1/bulma/templates/filters.html
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.340508 django-bulmacss-0.0.1/bulma/templates/flatpages/
--rw-r--r--   0 chen      (1000) chen      (1000)      318 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/flatpages/default.html
--rw-r--r--   0 chen      (1000) chen      (1000)      208 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/footer.html
--rw-r--r--   0 chen      (1000) chen      (1000)      710 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/form_display.html
--rw-r--r--   0 chen      (1000) chen      (1000)     2225 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/form_horizontal.html
--rw-r--r--   0 chen      (1000) chen      (1000)      452 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/form_modal.html
--rw-r--r--   0 chen      (1000) chen      (1000)      113 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/form_submit.html
--rw-r--r--   0 chen      (1000) chen      (1000)      491 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/formset_widget_display.html
--rw-r--r--   0 chen      (1000) chen      (1000)     3763 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/index.html
--rw-r--r--   0 chen      (1000) chen      (1000)      858 2023-04-14 01:27:58.000000 django-bulmacss-0.0.1/bulma/templates/main_menu.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1450 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/menus.html
--rw-r--r--   0 chen      (1000) chen      (1000)      669 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/messages.html
--rw-r--r--   0 chen      (1000) chen      (1000)      737 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/modal.html
--rw-r--r--   0 chen      (1000) chen      (1000)     2402 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/navbar.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1627 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/pagination.html
--rw-r--r--   0 chen      (1000) chen      (1000)      828 2023-04-13 08:58:39.000000 django-bulmacss-0.0.1/bulma/templates/profile_menu.html
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.343842 django-bulmacss-0.0.1/bulma/templates/registration/
--rw-r--r--   0 chen      (1000) chen      (1000)      243 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/account_inactive.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1004 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/base.html
--rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-27 08:10:38.000000 django-bulmacss-0.0.1/bulma/templates/registration/change-password.html
--rw-r--r--   0 chen      (1000) chen      (1000)     2796 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/email.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1143 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/email_confirm.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1565 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/index.html
--rw-r--r--   0 chen      (1000) chen      (1000)      540 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/login.html
--rw-r--r--   0 chen      (1000) chen      (1000)      838 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/logout.html
--rw-r--r--   0 chen      (1000) chen      (1000)      560 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/password_change.html
--rw-r--r--   0 chen      (1000) chen      (1000)      414 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/password_change_form.html
--rw-r--r--   0 chen      (1000) chen      (1000)      999 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/password_reset.html
--rw-r--r--   0 chen      (1000) chen      (1000)      554 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/password_reset_done.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1149 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/password_reset_from_key.html
--rw-r--r--   0 chen      (1000) chen      (1000)      343 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/password_reset_from_key_done.html
--rw-r--r--   0 chen      (1000) chen      (1000)      421 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/password_set.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1347 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/profile.html
--rw-r--r--   0 chen      (1000) chen      (1000)      849 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/settings.html
--rw-r--r--   0 chen      (1000) chen      (1000)     1062 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/signup.html
--rw-r--r--   0 chen      (1000) chen      (1000)      264 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/signup_closed.html
--rw-r--r--   0 chen      (1000) chen      (1000)      437 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/verification_sent.html
--rw-r--r--   0 chen      (1000) chen      (1000)      797 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/registration/verified_email_required.html
--rw-r--r--   0 chen      (1000) chen      (1000)      274 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/render_boolean.html
--rw-r--r--   0 chen      (1000) chen      (1000)      331 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/search_bar.html
--rw-r--r--   0 chen      (1000) chen      (1000)      751 2023-04-13 08:56:56.000000 django-bulmacss-0.0.1/bulma/templates/sorting.html
--rw-r--r--   0 chen      (1000) chen      (1000)       60 2022-05-27 08:10:38.000000 django-bulmacss-0.0.1/bulma/tests.py
--rw-r--r--   0 chen      (1000) chen      (1000)       63 2022-05-27 08:10:38.000000 django-bulmacss-0.0.1/bulma/views.py
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 02:30:27.343842 django-bulmacss-0.0.1/django_bulmacss.egg-info/
--rw-r--r--   0 chen      (1000) chen      (1000)     1473 2023-04-14 02:30:27.000000 django-bulmacss-0.0.1/django_bulmacss.egg-info/PKG-INFO
--rw-r--r--   0 chen      (1000) chen      (1000)     7064 2023-04-14 02:30:27.000000 django-bulmacss-0.0.1/django_bulmacss.egg-info/SOURCES.txt
--rw-r--r--   0 chen      (1000) chen      (1000)        1 2023-04-14 02:30:27.000000 django-bulmacss-0.0.1/django_bulmacss.egg-info/dependency_links.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       12 2023-04-14 02:30:27.000000 django-bulmacss-0.0.1/django_bulmacss.egg-info/requires.txt
--rw-r--r--   0 chen      (1000) chen      (1000)        6 2023-04-14 02:30:27.000000 django-bulmacss-0.0.1/django_bulmacss.egg-info/top_level.txt
--rw-r--r--   0 chen      (1000) chen      (1000)      100 2023-04-14 02:24:12.000000 django-bulmacss-0.0.1/pyproject.toml
--rw-r--r--   0 chen      (1000) chen      (1000)      884 2023-04-14 02:30:27.343842 django-bulmacss-0.0.1/setup.cfg
--rw-r--r--   0 chen      (1000) chen      (1000)       38 2023-04-14 02:03:27.000000 django-bulmacss-0.0.1/setup.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.247539 django-bulmacss-0.0.2/
+-rw-r--r--   0 chen      (1000) chen      (1000)     1063 2022-05-27 08:19:55.000000 django-bulmacss-0.0.2/LICENSE
+-rw-r--r--   0 chen      (1000) chen      (1000)      103 2023-04-14 02:04:21.000000 django-bulmacss-0.0.2/MANIFEST.in
+-rw-r--r--   0 chen      (1000) chen      (1000)     1999 2023-04-14 05:54:17.247539 django-bulmacss-0.0.2/PKG-INFO
+-rw-r--r--   0 chen      (1000) chen      (1000)     1125 2023-04-14 05:53:50.000000 django-bulmacss-0.0.2/README.rst
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.227539 django-bulmacss-0.0.2/bulma/
+-rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-27 08:10:38.000000 django-bulmacss-0.0.2/bulma/__init__.py
+-rw-r--r--   0 chen      (1000) chen      (1000)       63 2022-05-27 08:10:38.000000 django-bulmacss-0.0.2/bulma/admin.py
+-rw-r--r--   0 chen      (1000) chen      (1000)      142 2022-05-27 08:10:38.000000 django-bulmacss-0.0.2/bulma/apps.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.227539 django-bulmacss-0.0.2/bulma/migrations/
+-rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-27 08:10:38.000000 django-bulmacss-0.0.2/bulma/migrations/__init__.py
+-rw-r--r--   0 chen      (1000) chen      (1000)       57 2022-05-27 08:10:38.000000 django-bulmacss-0.0.2/bulma/models.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.224205 django-bulmacss-0.0.2/bulma/static/
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.230872 django-bulmacss-0.0.2/bulma/static/bulma/
+-rw-r--r--   0 chen      (1000) chen      (1000)   259362 2023-04-14 01:36:45.000000 django-bulmacss-0.0.2/bulma/static/bulma/bulma.min.css
+-rw-r--r--   0 chen      (1000) chen      (1000)    75779 2023-04-14 01:38:28.000000 django-bulmacss-0.0.2/bulma/static/bulma/feather.min.js
+-rw-r--r--   0 chen      (1000) chen      (1000)    80886 2023-04-14 01:38:28.000000 django-bulmacss-0.0.2/bulma/static/bulma/feather.min.js.map
+-rw-r--r--   0 chen      (1000) chen      (1000)     8907 2023-04-14 01:38:38.000000 django-bulmacss-0.0.2/bulma/static/bulma/jdenticon.min.js
+-rw-r--r--   0 chen      (1000) chen      (1000)    82680 2023-04-14 01:38:38.000000 django-bulmacss-0.0.2/bulma/static/bulma/jdenticon.min.js.map
+-rw-r--r--   0 chen      (1000) chen      (1000)   190940 2023-04-14 03:28:45.000000 django-bulmacss-0.0.2/bulma/static/bulma/login_bg.jpg
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.234205 django-bulmacss-0.0.2/bulma/templates/
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.234205 django-bulmacss-0.0.2/bulma/templates/account/
+-rw-r--r--   0 chen      (1000) chen      (1000)      342 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/account_inactive.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1004 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/base.html
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.234205 django-bulmacss-0.0.2/bulma/templates/account/email/
+-rw-r--r--   0 chen      (1000) chen      (1000)      342 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/email/base_message.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)      484 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/email/email_confirmation_message.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       61 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/email/email_confirmation_signup_message.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       61 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/email/email_confirmation_signup_subject.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)      127 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/email/email_confirmation_subject.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)      530 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/email/password_reset_key_message.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)      114 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/email/password_reset_key_subject.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)     2868 2023-04-14 03:34:16.000000 django-bulmacss-0.0.2/bulma/templates/account/email.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1143 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/email_confirm.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1565 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/index.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     2543 2023-04-14 03:32:05.000000 django-bulmacss-0.0.2/bulma/templates/account/login.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      716 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/logout.html
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.237539 django-bulmacss-0.0.2/bulma/templates/account/messages/
+-rw-r--r--   0 chen      (1000) chen      (1000)      110 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/messages/cannot_delete_primary_email.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       90 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/messages/email_confirmation_sent.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       81 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/messages/email_confirmed.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       85 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/messages/email_deleted.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)      138 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/messages/logged_in.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       72 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/messages/logged_out.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       82 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/messages/password_changed.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       78 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/messages/password_set.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       79 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/messages/primary_email_set.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       97 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/messages/unverified_primary_email.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       83 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/password_change.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      842 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/password_reset.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      554 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/password_reset_done.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1149 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/password_reset_from_key.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      343 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      441 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/password_set.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      849 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/settings.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1177 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/signup.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      357 2023-04-14 03:30:41.000000 django-bulmacss-0.0.2/bulma/templates/account/signup_closed.html
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.237539 django-bulmacss-0.0.2/bulma/templates/account/snippets/
+-rw-r--r--   0 chen      (1000) chen      (1000)      204 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/snippets/already_logged_in.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      437 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/verification_sent.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      919 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/account/verified_email_required.html
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.237539 django-bulmacss-0.0.2/bulma/templates/accounts/
+-rw-r--r--   0 chen      (1000) chen      (1000)      495 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/accounts/group_list.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      852 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/accounts/login_by_invite.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      676 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/accounts/phone_change.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      303 2023-04-14 03:33:38.000000 django-bulmacss-0.0.2/bulma/templates/accounts/profile.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      617 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/accounts/set_password.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     3299 2023-04-14 03:37:19.000000 django-bulmacss-0.0.2/bulma/templates/accounts/settings.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      812 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/accounts/signup_by_invite.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      277 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/accounts/tabs.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      736 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/accounts/user_confirm_delete.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      716 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/accounts/user_form.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     2819 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/accounts/user_list.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      371 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/accounts/user_tree.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     3363 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/accounts/user_tree_input.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      173 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/attrs.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      421 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/avatar.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1394 2023-04-14 03:10:37.000000 django-bulmacss-0.0.2/bulma/templates/base.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      342 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/breadcrumb.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      830 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/console.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      626 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/dir_tree.html
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.224205 django-bulmacss-0.0.2/bulma/templates/django/
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.240872 django-bulmacss-0.0.2/bulma/templates/django/forms/
+-rw-r--r--   0 chen      (1000) chen      (1000)      165 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/attrs.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      609 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/default.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      874 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/div.html
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.224205 django-bulmacss-0.0.2/bulma/templates/django/forms/errors/
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.240872 django-bulmacss-0.0.2/bulma/templates/django/forms/errors/dict/
+-rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/errors/dict/default.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      113 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/errors/dict/text.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)      137 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/errors/dict/ul.html
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.240872 django-bulmacss-0.0.2/bulma/templates/django/forms/errors/list/
+-rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/errors/list/default.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       52 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/errors/list/text.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)      200 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/errors/list/ul.html
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.240872 django-bulmacss-0.0.2/bulma/templates/django/forms/formsets/
+-rw-r--r--   0 chen      (1000) chen      (1000)       77 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/formsets/default.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       82 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/formsets/p.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       86 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/formsets/table.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       83 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/formsets/ul.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      128 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/label.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      684 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/p.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      825 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/table.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      723 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/ul.html
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.244206 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/
+-rw-r--r--   0 chen      (1000) chen      (1000)      172 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/attrs.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/checkbox.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      506 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/checkbox_option.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      510 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/checkbox_select.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      511 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/clearable_file_input.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       65 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/date.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      183 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/datetime.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/email.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/file.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/hidden.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      259 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/input.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      219 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/input_option.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       54 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/multiple_hidden.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      426 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/multiple_input.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      146 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/multiwidget.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/number.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/password.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       57 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/radio.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       55 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/radio_option.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      465 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/select.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       54 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/select_date.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      127 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/select_option.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       54 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/splitdatetime.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       54 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/splithiddendatetime.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/text.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      194 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/textarea.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       65 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/time.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       48 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/django/forms/widgets/url.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       84 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/empty.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      343 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/field_display.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      662 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/field_horizontal.html
+-rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-27 08:10:38.000000 django-bulmacss-0.0.2/bulma/templates/file_line.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1995 2023-04-14 01:27:02.000000 django-bulmacss-0.0.2/bulma/templates/filters.html
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.244206 django-bulmacss-0.0.2/bulma/templates/flatpages/
+-rw-r--r--   0 chen      (1000) chen      (1000)      318 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/flatpages/default.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      220 2023-04-14 03:11:14.000000 django-bulmacss-0.0.2/bulma/templates/footer.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      710 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/form_display.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     2225 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/form_horizontal.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      452 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/form_modal.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      113 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/form_submit.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      491 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/formset_widget_display.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     3814 2023-04-14 03:17:33.000000 django-bulmacss-0.0.2/bulma/templates/index.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      858 2023-04-14 01:27:58.000000 django-bulmacss-0.0.2/bulma/templates/main_menu.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1450 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/menus.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      669 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/messages.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      737 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/modal.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     2413 2023-04-14 03:11:47.000000 django-bulmacss-0.0.2/bulma/templates/navbar.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1627 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/pagination.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      828 2023-04-13 08:58:39.000000 django-bulmacss-0.0.2/bulma/templates/profile_menu.html
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.247539 django-bulmacss-0.0.2/bulma/templates/registration/
+-rw-r--r--   0 chen      (1000) chen      (1000)      243 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/account_inactive.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1004 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/base.html
+-rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-27 08:10:38.000000 django-bulmacss-0.0.2/bulma/templates/registration/change-password.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     2796 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/email.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1143 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/email_confirm.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1565 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/index.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      540 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/login.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      838 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/logout.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      560 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/password_change.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      414 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/password_change_form.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      999 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/password_reset.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      554 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/password_reset_done.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1149 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/password_reset_from_key.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      343 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/password_reset_from_key_done.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      421 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/password_set.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1347 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/profile.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      849 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/settings.html
+-rw-r--r--   0 chen      (1000) chen      (1000)     1062 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/signup.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      264 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/signup_closed.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      437 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/verification_sent.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      797 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/registration/verified_email_required.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      274 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/render_boolean.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      331 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/search_bar.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      751 2023-04-13 08:56:56.000000 django-bulmacss-0.0.2/bulma/templates/sorting.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       60 2022-05-27 08:10:38.000000 django-bulmacss-0.0.2/bulma/tests.py
+-rw-r--r--   0 chen      (1000) chen      (1000)       63 2022-05-27 08:10:38.000000 django-bulmacss-0.0.2/bulma/views.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 05:54:17.247539 django-bulmacss-0.0.2/django_bulmacss.egg-info/
+-rw-r--r--   0 chen      (1000) chen      (1000)     1999 2023-04-14 05:54:17.000000 django-bulmacss-0.0.2/django_bulmacss.egg-info/PKG-INFO
+-rw-r--r--   0 chen      (1000) chen      (1000)     7096 2023-04-14 05:54:17.000000 django-bulmacss-0.0.2/django_bulmacss.egg-info/SOURCES.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)        1 2023-04-14 05:54:17.000000 django-bulmacss-0.0.2/django_bulmacss.egg-info/dependency_links.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       12 2023-04-14 05:54:17.000000 django-bulmacss-0.0.2/django_bulmacss.egg-info/requires.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)        6 2023-04-14 05:54:17.000000 django-bulmacss-0.0.2/django_bulmacss.egg-info/top_level.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)      100 2023-04-14 02:24:12.000000 django-bulmacss-0.0.2/pyproject.toml
+-rw-r--r--   0 chen      (1000) chen      (1000)      884 2023-04-14 05:54:17.247539 django-bulmacss-0.0.2/setup.cfg
+-rw-r--r--   0 chen      (1000) chen      (1000)       38 2023-04-14 02:03:27.000000 django-bulmacss-0.0.2/setup.py
```

### Comparing `django-bulmacss-0.0.1/LICENSE` & `django-bulmacss-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/static/bulma/bulma.min.css` & `django-bulmacss-0.0.2/bulma/static/bulma/bulma.min.css`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/static/bulma/feather.min.js` & `django-bulmacss-0.0.2/bulma/static/bulma/feather.min.js`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/static/bulma/feather.min.js.map` & `django-bulmacss-0.0.2/bulma/static/bulma/feather.min.js.map`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/static/bulma/jdenticon.min.js` & `django-bulmacss-0.0.2/bulma/static/bulma/jdenticon.min.js`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/static/bulma/jdenticon.min.js.map` & `django-bulmacss-0.0.2/bulma/static/bulma/jdenticon.min.js.map`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/account/base.html` & `django-bulmacss-0.0.2/bulma/templates/account/base.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/account/email/password_reset_key_message.txt` & `django-bulmacss-0.0.2/bulma/templates/account/email/password_reset_key_message.txt`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/account/email.html` & `django-bulmacss-0.0.2/bulma/templates/account/email.html`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,17 @@
       <p class="block"><strong>{% translate '提醒:'%}</strong> {% translate "您目前没有设置任何电子邮件地址。您确实应该添加一个电子邮件地址，以便接收通知、重置密码等。" %}</p>
     {% endif %}
 
     {% if can_add_email %}
       <h2 class="subtitle">{% translate "添加邮箱" %}</h2>
 
       <form method="post" action="{% url 'account_email' %}" class="add_email">
-				{% csrf_token %}
-				{% include "form_snippet.html" %}
-				<button class="button is-primary" name="action_add" type="submit">{% translate "保存" %}</button>
+	{% csrf_token %}
+	{{form}}
+	<button class="button is-primary" name="action_add" type="submit">{% translate "保存" %}</button>
       </form>
 
     {% endif %}
   </div>
 {% endblock %}
```

### Comparing `django-bulmacss-0.0.1/bulma/templates/account/email_confirm.html` & `django-bulmacss-0.0.2/bulma/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/account/index.html` & `django-bulmacss-0.0.2/bulma/templates/account/index.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/account/login.html` & `django-bulmacss-0.0.2/bulma/templates/account/login.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,71 @@
 {% extends "base.html" %}
-{% load static i18n thumbnail %}
+{% load static i18n %}
+{% load account %}
 
 {% block head_title %}{% trans "Sign In" %}{% endblock %}
 {% block navbar %}{% endblock %}
 {% block footer %}{% endblock %}
 {% block html_class %}{% endblock %}
 
 {% block extra_css %}
   <style>
-   #app {
-     background: linear-gradient(30deg, white 45%, transparent 15%, transparent 40%), linear-gradient(150deg, #1e47af 55%, white 45%);
+   html, body {
+     overflow: hidden;
    }
-   .container {
-     max-width: 460px !important;
-     background: white;
-     padding: 3rem;
-     border-radius: 5px;
-     box-shadow: 1px 2px 4px lightgrey;
+   #rightPanel {
+     background-image: url("/static/bulma/login_bg.jpg");
+     background-size: cover;
+     background-repeat: no-repeat;
+     background-position: center;
+     height: 100vh;
+     padding: 0;
    }
   </style>
 {% endblock %}
 
 {% block content %}
-  <section class="section">
-    <div class="has-text-centered my-6" style="margin-bottom:8vh !important;">
-      {% if request.site.setting.logo %}
-	<figure class="image is-inline-block">
-    {% comment %}
-	  {% thumbnail request.site.setting.logo "x120" as im %}
-	  <img src="{{im.url}}" />
-	  {% endthumbnail %}
-    {% endcomment %}
-    <img src="{{request.site.setting.logo.url}}" style="height:84px;" />
-	</figure>
-      {% else %}
-	<p class="title has-text-white">{{request.site.setting.site_name|default:'MDAI'}}</p>
-      {% endif %}
-    </div>
-    <div class="container">
-        <h1 class="title has-text-centered mb-6" style="letter-spacing:2px;">{% translate "Welcome back" %}</h1>
-
-      <form class="login" method="POST" action="{% url 'account_login' %}">
-	{% csrf_token %}
-	{% if form.non_field_errors %}
-	  <div class="notification is-danger is-light" >{{form.non_field_errors}}</div>
-	{% endif %}
-
-	<div class="field mb-5" >
-	  <div class="control has-icons-left" >
-          <input name="login" class="input is-medium" type="text" placeholder="{% translate "username or email address" %}" />
-	    <span class="icon is-small is-left" >
-	      <i data-feather="user"></i>
-	    </span>
+  <div class="columns">
+    <div class="column is-narrow">
+      <div class="is-flex is-justify-content-center" style="width:600px;max-width:100%;">
+	<div style="width:420px;max-width:100%;" class="py-6 px-5">
+	  {% if request.site.setting.logo %}
+	    <img class="mb-6" src="{{request.site.setting.logo.url}}" style="height:32px;" />
+	  {% endif %}
+	<h1 class="title">欢迎登录</h1>	
+	<form method="post">
+	  {% csrf_token %}
+	  {% if form.non_field_errors %}
+	    <div class="notification is-danger is-light" >{{form.non_field_errors.0}}</div>
+	  {% endif %}
+	  <div class="field">
+	    <label class="label">登录帐号</label>
+	    <input type="text" name="login" class="input" placeholder="用户名, {% if request.site.setting.enabled_phonenumber %}手机号码, {% endif %}邮箱地址" />
 	  </div>
-	</div>
-	<div class="field mb-5" >
-	  <div class="control has-icons-left" >
-          <input name="password" class="input is-medium" type="password" placeholder="{% translate "password" %}" />
-	    <span class="icon is-small is-left" >
-	      <i data-feather="lock"></i>
-	    </span>
+	  <div class="field">
+	    <label class="label">帐号密码</label>
+	    <input type="password" name="password" class="input" placeholder="登录密码" />
 	  </div>
-	</div>
-	{% comment %}
-	<p class="block has-text-right">
-	  <a href="/accounts/password/reset/" class="has-text-grey">{% trans "Forgot Password?" %}</a>
-	</p>
-	{% endcomment %}
-	{% if redirect_field_value %}
-	  <input type="hidden" name="{{ redirect_field_name }}" value="{{ redirect_field_value }}" />
-	{% endif %}
-	<div class="field" >
-	  <div class="control" >
-	    <button class="button is-primary is-fullwidth is-medium" type="submit">{% trans "Sign In" %}</button>
+	  <p class="has-text-right my-5"><a href="{% if request.site.setting.enabled_phonenumber %}/accounts/password/reset_by_phone/{% else %}/accounts/password/reset/{% endif %}" class="has-text-dark">{% trans "Forgot Password?" %}</a></p>
+	  {% if redirect_field_value %}
+	    <input type="hidden" name="{{ redirect_field_name }}" value="{{ redirect_field_value }}" />
+	  {% endif %}
+	  <div class="field" >
+	    <div class="control" >
+	      <button class="button is-primary is-fullwidth is-medium" type="submit">登  录</button>
+	    </div>
 	  </div>
+	  <p class="has-text-centered py-5">还没有帐号? 请先<a href="{{signup_url}}" class="has-text-primary">注册</a></p>
+	</form>
 	</div>
-      </form>
+      </div>
+    </div>
+    <div class="column is-hidden-mobile" id="rightPanel">
     </div>
-    {% comment %}
-      <p class="block has-text-centered py-5">还没有帐号? 请先<a href="{{signup_url}}">注册</a></p>
-    {% endcomment %}
-  </section>
+  </div>
 {% endblock %}
 
 {% block extra_js %}
   <script>
    document.querySelector("form").addEventListener("submit", event => {
      event.submitter.classList.add("is-loading")
    })
```

#### html2text {}

```diff
@@ -1,24 +1,19 @@
-{% extends "base.html" %} {% load static i18n thumbnail %} {% block head_title
-%}{% trans "Sign In" %}{% endblock %} {% block navbar %}{% endblock %} {% block
-footer %}{% endblock %} {% block html_class %}{% endblock %} {% block extra_css
-%}
+{% extends "base.html" %} {% load static i18n %} {% load account %} {% block
+head_title %}{% trans "Sign In" %}{% endblock %} {% block navbar %}{% endblock
+%} {% block footer %}{% endblock %} {% block html_class %}{% endblock %} {%
+block extra_css %}
  {% endblock %} {% block content %}
-{% if request.site.setting.logo %}  {% comment %} {% thumbnail
-request.site.setting.logo "x120" as im %} [{{im.url}}] {% endthumbnail %} {%
-endcomment %} [{{request.site.setting.logo.url}}]  {% else %}
-{{request.site.setting.site_name|default:'MDAI'}}
-{% endif %}
-****** {% translate "Welcome back" %} ******
+{% if request.site.setting.logo %} [{{request.site.setting.logo.url}}] {% endif
+%}
+****** æ¬¢è¿ç»å½ ******
 {% csrf_token %} {% if form.non_field_errors %}
-{{form.non_field_errors}}
+{{form.non_field_errors.0}}
 {% endif %}
- %}" />
- %}" />
-{% comment %}
+ç»å½å¸å· [login               ]
+å¸å·å¯ç  [********************]
 {%_trans_"Forgot_Password?"_%}
-{% endcomment %} {% if redirect_field_value %}  {% endif %}
-{% trans "Sign In" %}
-{% comment %}
+{% if redirect_field_value %}  {% endif %}
+ç» å½
 è¿æ²¡æå¸å·? è¯·åæ³¨å
-{% endcomment %}  {% endblock %} {% block extra_js %}
+{% endblock %} {% block extra_js %}
  {% endblock %}
```

### Comparing `django-bulmacss-0.0.1/bulma/templates/account/logout.html` & `django-bulmacss-0.0.2/bulma/templates/account/logout.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/account/password_reset.html` & `django-bulmacss-0.0.2/bulma/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/account/password_reset_done.html` & `django-bulmacss-0.0.2/bulma/templates/account/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/account/password_reset_from_key.html` & `django-bulmacss-0.0.2/bulma/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/account/settings.html` & `django-bulmacss-0.0.2/bulma/templates/account/settings.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/account/signup.html` & `django-bulmacss-0.0.2/bulma/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/account/verified_email_required.html` & `django-bulmacss-0.0.2/bulma/templates/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/accounts/login_by_invite.html` & `django-bulmacss-0.0.2/bulma/templates/accounts/login_by_invite.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/accounts/phone_change.html` & `django-bulmacss-0.0.2/bulma/templates/accounts/phone_change.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/accounts/set_password.html` & `django-bulmacss-0.0.2/bulma/templates/accounts/set_password.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/accounts/settings.html` & `django-bulmacss-0.0.2/bulma/templates/accounts/settings.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,116 +1,117 @@
 {% extends "base.html" %}
 {% load static thumbnail %}
 {% block extra_css %}
 {{block.super}}
 <style>
-  .tabs{
-    background:#faf8fb;
-    margin:auto;
-    border-radius:10px;
-  }
-  .tabs ul{
-    border:none;
-  }
-  .tabs li{
-    padding:5px 10px;
-    border-radius:10px;
-  }
-  .tabs a {
-    padding:0;
-    border-bottom:none;
-  }
-  .tabs a:hover {
-    color:#4258fe;
-  }
-  .tabs .is-active {
-    background:#fff;
-    color:#4258fe;
-  }
-  .avatar {
-    width:fit-content;
-    overflow:hidden;
-    border-radius:10px;
-    border: 3px solid rgba(255,255,255,0.6);
-  }
-  .avatar label {
-    position: absolute;
-    top: 0;
-    left: 0;
-    width: 100%;
-    height: 100%;
-    background: rgba(0,0,0,0.65);
-    display: none;
-    padding: 1rem;
-    align-items: center;
-    text-align: center;
-  }
-  .avatar:hover label {
-  display: inline-flex;
-  }
+.tabs-container {
+ padding: 0 1.5rem;
+}
+.tabs-container {
+ position: relative;
+}
+.tabs-container::before {
+ content: "";
+ display: block;
+ bottom: 0;
+ left: 0;
+ height: 1px;
+ width: 100%;
+ background: #dbdbdb;
+ position: absolute;
+}
+.tabs a {
+ padding: 0.5rem 0;
+ margin-right: 1.5rem;
+ color: white;
+ margin-bottom: 0;
+ border-color: #0073ea !important;
+ border-width: 2px;
+}
+.tabs a:hover {
+ color: white;
+ border-bottom-color: white !important;
+}
+.tabs .is-active a {
+ color: white !important;
+ border-bottom-color: white !important;
+}
+.avatar {
+ border: 3px solid rgba(255,255,255,0.6);
+}
+.avatar label {
+ position: absolute;
+ top: 0;
+ left: 0;
+ width: 100%;
+ height: 100%;
+ background: rgba(0,0,0,0.65);
+ display: none;
+ padding: 1rem;
+ align-items: center;
+ text-align: center;
+
+}
+.avatar:hover label {
+ display: inline-flex;
+}
+
 </style>
 {% endblock %}
 {% block content %}
-<section class="section pt-2">
-  <div class="container is-max-desktop">
-    <p class='title pt-6'>我的信息</p>
-  </div>
-  <div class="container is-max-desktop tabs is-centered is-text-black py-2 mt-5">
-    <ul>
-      <li class="m-1 {% if request.path == '/accounts/profile/' %}is-active{% endif %}"><a href="/accounts/profile/">基础信息</a></li>
-      {% if request.site.setting.enabled_phonenumber %}
-	<li class="m-1 {% if request.path == '/accounts/phone/change/' %}is-active{% endif %}"><a href="/accounts/phone/change/">修改手机号码</a></li>
-      {% endif %}
-      <li class="m-1 {% if request.path == '/accounts/email/' %}is-active{% endif %}"><a href="/accounts/email/">邮箱设置</a></li>
-      <li class="m-1 {% if request.path == '/accounts/password/set/' %}is-active{% endif %}"><a href="/accounts/password/change/">修改密码</a></li>
-    </ul>
-  </div>
+<section class="section p-0 has-background-link has-text-white" style="background:#0073ea !important;">
+  <div class="container has-text-centered pt-6 pb-3">
+    <figure class="avatar image is-128x128 mt-5 mb-2" style="border-radius:99px;overflow:hidden;margin:0 auto;">
+     {% if user.avatar %}
+     {% thumbnail user.avatar "128x128" crop="center" as im %}
+     <img src="{{im.url}}" />
+     {% endthumbnail %}
+     {% else %}
+     <svg width="128" height="128" class="has-background-white" data-jdenticon-value="{{user.email}}"></svg>
+     {% endif %}
+     <form method="post" enctype="multipart/form-data" action="/accounts/update_avatar/?redirect={{request.get_full_path}}">
+       {% csrf_token %}
+       <label for="id_avatar" style='justify-content:center;'><span>修改头像</span></label>
+       <input name="avatar" id="id_avatar" type="file" class="is-hidden" accept="image/*" />
+     </form>
+   </figure>
+   <div class="content">
+     <p class="is-size-3 has-text-light" >{{user.username|upper}}</p>
+   </div>
+ </div>
+ <div class="tabs is-centered">
+  <ul>
+   <li {% if request.path == "/accounts/profile/" %}class="is-active"{% endif %}><a href="/accounts/profile/">基础信息</a></li>
+   <li {% if request.path == "/accounts/email/" %}class="is-active"{% endif %}><a href="/accounts/email/">邮箱设置</a></li>
+   <li {% if request.path == "/accounts/password/set/" %}class="is-active"{% endif %}><a href="/accounts/password/change/">修改密码</a></li>
+ </ul>
+</div>
 </section>
 <section class="section pt-5" >
-  <div class="container" style="max-width:420px;">
+  <div class="container" style="max-width:600px;">
+    {#<h1 class="subtitle">{% block subtitle %}{{title}}{% endblock %}</h1>#}
     {% include "messages.html" %}
-    {% if request.path == '/accounts/profile/' %}
-      <div class='mb-2'>
-        <label class='label'>头像</label>
-        <div class="avatar">
-          <figure class="image is-64x64">
-            {% if user.avatar %}
-              {% thumbnail user.avatar "128x128" crop="center" as im %}<img src="{{im.url}}" />{% endthumbnail %}
-            {% else %}
-              <svg width="128" height="128" class="has-background-white" data-jdenticon-value="{{user.email}}"></svg>
-            {% endif %}
-            <form method="post" enctype="multipart/form-data" action="/accounts/update_avatar/?redirect={{request.get_full_path}}">
-              {% csrf_token %}
-              <label for="id_avatar" style='justify-content:center;color:#fff;'><span>编辑</span></label>
-              <input name="avatar" id="id_avatar" type="file" class="is-hidden" accept="image/*" />
-            </form>
-          </figure>
-        </div>
-      </div>
-    {% endif %}
     {% block inner %}
-      <form method="post" style="max-width:600px;">
-        {% csrf_token %}
-        {% include "form_snippet.html" %}
-        <div class="field is-grouped mt-6" >
-          <p class="control" >
-            <button type="submit" class="button is-primary" >保存</button>
-          </p>
-          <p class="control" >
-            <button data-goback class="button" >取消</button>
-          </p>
-        </div>
-      </form>
-    {% endblock %}
-  </div>
+    <form method="post" style="max-width:600px;">
+     {% csrf_token %}
+      {{form}}
+     <div class="field is-grouped mt-6" >
+       <p class="control" >
+         <button type="submit" class="button is-primary" >保存</button>
+       </p>
+       <p class="control" >
+         <button data-goback class="button" >取消</button>
+       </p>
+     </div>
+   </form>
+   {% endblock %}
+ </div>
 </section>
 {% endblock %}
 {% block extra_js %}
-  {{block.super}}
-  <script src="{% static 'server/js/cookies.js' %}"></script>
-  <script src="{% static 'server/js/sms.js' %}"></script>  
-  <script>
-    document.getElementById("id_avatar").addEventListener("change", (e) => {
-      e.target.closest("form").submit()
-    })
-  </script>
+{{block.super}}
+<script>
+document.getElementById("id_avatar").addEventListener("change", (e) => {
+ e.target.closest("form").submit()
+})
+</script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
 {% extends "base.html" %} {% load static thumbnail %} {% block extra_css %} {
 {block.super}}
  {% endblock %} {% block content %}
-æçä¿¡æ¯
-    * åºç¡ä¿¡æ¯
-    * {% if request.site.setting.enabled_phonenumber %}
-    * ä¿®æ¹ææºå·ç 
-    * {% endif %}
-    * é®ç®±è®¾ç½®
-    * ä¿®æ¹å¯ç 
-
-{% include "messages.html" %} {% if request.path == '/accounts/profile/' %}
-å¤´å
  {% if user.avatar %} {% thumbnail user.avatar "128x128" crop="center" as im %}
-[{{im.url}}]{% endthumbnail %} {% else %}  {% endif %}
-{% csrf_token %} ç¼è¾ [File]
-{% endif %} {% block inner %}
-{% csrf_token %} {% include "form_snippet.html" %}
+[{{im.url}}] {% endthumbnail %} {% else %}  {% endif %}
+{% csrf_token %} ä¿®æ¹å¤´å [File]
+{{user.username|upper}}
+    * % if request.path == "/accounts/profile/" %}class="is-active"{% endif
+      %}>åºç¡ä¿¡æ¯
+% if request.path == "/accounts/email/" %}class="is-active"{% endif
+%}>é®ç®±è®¾ç½®
+% if request.path == "/accounts/password/set/" %}class="is-active"{% endif
+%}>ä¿®æ¹å¯ç 
+
+{#
+****** {% block subtitle %}{{title}}{% endblock %} ******
+#} {% include "messages.html" %} {% block inner %}
+{% csrf_token %} {{form}}
 ä¿å­
 åæ¶
 {% endblock %}
  {% endblock %} {% block extra_js %} {{block.super}}
  {% endblock %}
```

### Comparing `django-bulmacss-0.0.1/bulma/templates/accounts/signup_by_invite.html` & `django-bulmacss-0.0.2/bulma/templates/accounts/signup_by_invite.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/accounts/user_confirm_delete.html` & `django-bulmacss-0.0.2/bulma/templates/accounts/user_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/accounts/user_form.html` & `django-bulmacss-0.0.2/bulma/templates/accounts/user_form.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/accounts/user_list.html` & `django-bulmacss-0.0.2/bulma/templates/accounts/user_list.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/accounts/user_tree_input.html` & `django-bulmacss-0.0.2/bulma/templates/accounts/user_tree_input.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/base.html` & `django-bulmacss-0.0.2/bulma/templates/base.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% load static %}
 
 <!DOCTYPE html>
 <html class="{% block html_class %}has-navbar-fixed-top{% endblock %}" lang="zh">
   <head>
     <meta charset="utf-8" />
     <title>
-      {% block title %}{{title|default:"MDAI"}}{% endblock %}
+      {% block title %}{{title|default:"Django-Bulmacss"}}{% endblock %}
     </title>
     <meta name="description" content="" />
     <meta name="viewport" content="width=device-width, initial-scale=1" />
     {#<link rel="shortcut icon" href="{% static 'server/img/favicon.ico' %}">#}
     
 
     {# Global stylesheets #}
```

### Comparing `django-bulmacss-0.0.1/bulma/templates/console.html` & `django-bulmacss-0.0.2/bulma/templates/console.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/dir_tree.html` & `django-bulmacss-0.0.2/bulma/templates/dir_tree.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/django/forms/default.html` & `django-bulmacss-0.0.2/bulma/templates/django/forms/default.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/django/forms/div.html` & `django-bulmacss-0.0.2/bulma/templates/django/forms/div.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/django/forms/p.html` & `django-bulmacss-0.0.2/bulma/templates/django/forms/p.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/django/forms/table.html` & `django-bulmacss-0.0.2/bulma/templates/django/forms/table.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/django/forms/ul.html` & `django-bulmacss-0.0.2/bulma/templates/django/forms/ul.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/field_horizontal.html` & `django-bulmacss-0.0.2/bulma/templates/field_horizontal.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/filters.html` & `django-bulmacss-0.0.2/bulma/templates/filters.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/form_display.html` & `django-bulmacss-0.0.2/bulma/templates/form_display.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/form_horizontal.html` & `django-bulmacss-0.0.2/bulma/templates/form_horizontal.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/index.html` & `django-bulmacss-0.0.2/bulma/templates/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 {% endblock %}
 {% block navbar %}
   {% include "navbar.html" %}
 {% endblock %}
 {% block content %}
     <div class="hero-body" >
       <div class="container" >
-	<p class="title mb-4 is-size-1" >MDAI</p>
-    <p class="subtitle mt-4 is-size-3" >MDAI is a new ai platform, <br>and one that is well suited to a wide range of purposes, <br>including business development, research, commercial projects, etc</p>
-	<a href="" class="button is-warning has-text-weight-bold">TRY NOW</a>
+	<p class="title mb-4 is-size-1" >Bulma Css</p>
+    <p class="subtitle mt-4 is-size-3" >Bulma is a simple and beautiful css framework, <br>Django-Bulmacss provide many common templates for multiple usage.<br>including allauth, basic form, flatpages, etc</p>
+	<a href="https://github.com/ChanMo/django-bulma/" class="button is-warning has-text-weight-bold">TRY NOW</a>
       </div>
     </div>
   </section>
   {% comment %}
   <section class="section" >
     <div class="container" style="max-width:900px;">
       <h3 class="title is-4 mb-6">功能特性</h3>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 {% extends "base.html" %} {% load static %} {% block extra_css %}
  {% endblock %} {% block navbar %} {% include "navbar.html" %} {% endblock %}
 {% block content %}
-MDAI
-MDAI is a new ai platform,
-and one that is well suited to a wide range of purposes,
-including business development, research, commercial projects, etc
-TRY NOW
+Bulma Css
+Bulma is a simple and beautiful css framework,
+Django-Bulmacss provide many common templates for multiple usage.
+including allauth, basic form, flatpages, etc
+TRY_NOW
  {% comment %}
 **** åè½ç¹æ§ ****
 
 mg/img1.png" %}" style="width:320px;" />
 *** æç®ä»£ç æ¶æ ***
 åªåå«å¿è¦åè½æ¨¡å, è®©å®å¶å¼åæ´å®¹æ
 *** ä½¿ç¨ææ°ææ¯ ***
```

### Comparing `django-bulmacss-0.0.1/bulma/templates/main_menu.html` & `django-bulmacss-0.0.2/bulma/templates/main_menu.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/menus.html` & `django-bulmacss-0.0.2/bulma/templates/menus.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/messages.html` & `django-bulmacss-0.0.2/bulma/templates/messages.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/modal.html` & `django-bulmacss-0.0.2/bulma/templates/modal.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/navbar.html` & `django-bulmacss-0.0.2/bulma/templates/navbar.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load static %}
 <nav class="navbar is-fixed-top is-link noprint">
   <div class="container">
     <div class="navbar-brand">
-      <a class="navbar-item has-text-weight-bold" href="/">MDAI</a>
+      <a class="navbar-item has-text-weight-bold" href="/">Django-BulmaCss</a>
       <span class="navbar-burger burger" data-target="navbarMenuHeroA">
         <span></span>
         <span></span>
         <span></span>
       </span>
     </div>
     <div id="navbarMenuHeroA" class="navbar-menu">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% load static %}
-MDAI
+Django-BulmaCss
 {% if not user.is_authenticated %}
 åè´¹æ³¨å ç»å½
 {% else %} {#
  in request.path %}is-active{% endif %}" href="{% url 'help:index'
 %}">å¸®å©ä¸­å¿
 #}
  {%_with_count=user.total_msg_%}_{%_if_count_%}_{{count}}_{%_endif_%}_{%
```

### Comparing `django-bulmacss-0.0.1/bulma/templates/pagination.html` & `django-bulmacss-0.0.2/bulma/templates/pagination.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/profile_menu.html` & `django-bulmacss-0.0.2/bulma/templates/profile_menu.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/registration/base.html` & `django-bulmacss-0.0.2/bulma/templates/registration/base.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/registration/email.html` & `django-bulmacss-0.0.2/bulma/templates/registration/email.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/registration/email_confirm.html` & `django-bulmacss-0.0.2/bulma/templates/registration/email_confirm.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/registration/index.html` & `django-bulmacss-0.0.2/bulma/templates/registration/index.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/registration/login.html` & `django-bulmacss-0.0.2/bulma/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/registration/logout.html` & `django-bulmacss-0.0.2/bulma/templates/registration/logout.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/registration/password_change.html` & `django-bulmacss-0.0.2/bulma/templates/registration/password_change.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/registration/password_reset.html` & `django-bulmacss-0.0.2/bulma/templates/registration/password_reset.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/registration/password_reset_done.html` & `django-bulmacss-0.0.2/bulma/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/registration/password_reset_from_key.html` & `django-bulmacss-0.0.2/bulma/templates/registration/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/registration/profile.html` & `django-bulmacss-0.0.2/bulma/templates/registration/profile.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/registration/settings.html` & `django-bulmacss-0.0.2/bulma/templates/registration/settings.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/registration/signup.html` & `django-bulmacss-0.0.2/bulma/templates/registration/signup.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/registration/verified_email_required.html` & `django-bulmacss-0.0.2/bulma/templates/registration/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/bulma/templates/sorting.html` & `django-bulmacss-0.0.2/bulma/templates/sorting.html`

 * *Files identical despite different names*

### Comparing `django-bulmacss-0.0.1/django_bulmacss.egg-info/SOURCES.txt` & `django-bulmacss-0.0.2/django_bulmacss.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 bulma/views.py
 bulma/migrations/__init__.py
 bulma/static/bulma/bulma.min.css
 bulma/static/bulma/feather.min.js
 bulma/static/bulma/feather.min.js.map
 bulma/static/bulma/jdenticon.min.js
 bulma/static/bulma/jdenticon.min.js.map
+bulma/static/bulma/login_bg.jpg
 bulma/templates/attrs.html
 bulma/templates/avatar.html
 bulma/templates/base.html
 bulma/templates/breadcrumb.html
 bulma/templates/console.html
 bulma/templates/dir_tree.html
 bulma/templates/empty.html
```

### Comparing `django-bulmacss-0.0.1/setup.cfg` & `django-bulmacss-0.0.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-bulmacss
-version = 0.0.1
+version = 0.0.2
 description = Some Django Templates Base On Bulma.css.
 long_description = file: README.rst
 url = https://github.com/ChanMo/django-bulma/
 author = ChanMo
 author_email = chan.mo@outlook.com
 license = MIT
 classifiers =
```

