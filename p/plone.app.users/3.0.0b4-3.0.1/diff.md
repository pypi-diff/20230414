# Comparing `tmp/plone.app.users-3.0.0b4.tar.gz` & `tmp/plone.app.users-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.users-3.0.0b4.tar", last modified: Tue Oct 11 20:58:10 2022, max compression
+gzip compressed data, was "plone.app.users-3.0.1.tar", last modified: Tue Mar 14 16:16:13 2023, max compression
```

## Comparing `plone.app.users-3.0.0b4.tar` & `plone.app.users-3.0.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:58:10.786562 plone.app.users-3.0.0b4/
--rw-r--r--   0 maurits    (501) staff       (20)    20055 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    23530 2022-10-11 20:58:10.786683 plone.app.users-3.0.0b4/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2560 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:58:10.770089 plone.app.users-3.0.0b4/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      677 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:58:10.770344 plone.app.users-3.0.0b4/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:58:10.772812 plone.app.users-3.0.0b4/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:58:10.775206 plone.app.users-3.0.0b4/plone/app/users/
--rw-r--r--   0 maurits    (501) staff       (20)      637 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/TODO.txt
--rw-r--r--   0 maurits    (501) staff       (20)       24 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:58:10.779898 plone.app.users-3.0.0b4/plone/app/users/browser/
--rw-r--r--   0 maurits    (501) staff       (20)       24 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1866 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/account-configlet.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1277 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/account-panel.pt
--rw-r--r--   0 maurits    (501) staff       (20)    11788 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/account.py
--rw-r--r--   0 maurits    (501) staff       (20)     3435 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2569 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     1524 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/memberregistration.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3715 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/membersearch.py
--rw-r--r--   0 maurits    (501) staff       (20)     4117 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/membersearch_form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1020 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/newuser_form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5683 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/passwordpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     3683 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/personalpreferences.py
--rw-r--r--   0 maurits    (501) staff       (20)    30914 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/register.py
--rw-r--r--   0 maurits    (501) staff       (20)     1586 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/register_form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4688 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/registered.pt
--rw-r--r--   0 maurits    (501) staff       (20)      598 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/registered.py
--rw-r--r--   0 maurits    (501) staff       (20)     2826 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/registersettingspanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     1710 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/schema_layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10199 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     4671 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/browser/userdatapanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     3017 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2173 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/field_extender.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:58:10.766892 plone.app.users-3.0.0b4/plone/app/users/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:58:10.780340 plone.app.users-3.0.0b4/plone/app/users/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)       70 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1977 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/profiles/default/userschema.xml
--rw-r--r--   0 maurits    (501) staff       (20)     5905 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/schema.py
--rw-r--r--   0 maurits    (501) staff       (20)      717 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1440 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:58:10.786150 plone.app.users-3.0.0b4/plone/app/users/tests/
--rw-r--r--   0 maurits    (501) staff       (20)       24 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:58:10.786367 plone.app.users-3.0.0b4/plone/app/users/tests/acceptance/
--rw-r--r--   0 maurits    (501) staff       (20)     9670 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/acceptance/test_edit_user_schema.robot
--rw-r--r--   0 maurits    (501) staff       (20)     5117 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     1997 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/duplicate_email.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4463 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/email_login.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7625 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/flexible_user_registration.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2712 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/forms_navigationroot.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3275 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/member_search.rst
--rw-r--r--   0 maurits    (501) staff       (20)      306 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/onepixel.jpg
--rw-r--r--   0 maurits    (501) staff       (20)     5282 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/password.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4060 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/personal_preferences.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3645 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/personal_preferences_prefs_user_details.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4246 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/plugins.rst
--rw-r--r--   0 maurits    (501) staff       (20)    15438 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/registration_forms.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1702 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/test_account.py
--rw-r--r--   0 maurits    (501) staff       (20)     1113 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)     8313 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/test_exportimport.py
--rw-r--r--   0 maurits    (501) staff       (20)     2423 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/test_loginname_generator.py
--rw-r--r--   0 maurits    (501) staff       (20)      559 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/test_member_search.py
--rw-r--r--   0 maurits    (501) staff       (20)     8587 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/test_new_user.py
--rw-r--r--   0 maurits    (501) staff       (20)     1828 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/test_pam.py
--rw-r--r--   0 maurits    (501) staff       (20)      753 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)     7620 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/test_schema_types.py
--rw-r--r--   0 maurits    (501) staff       (20)     1214 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/test_user_data_panel.py
--rw-r--r--   0 maurits    (501) staff       (20)     5218 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/test_userid_generator.py
--rw-r--r--   0 maurits    (501) staff       (20)     6049 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/userdata.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2730 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/tests/userdata_prefs_user_details.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3759 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)      684 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     4437 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/plone/app/users/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:58:10.772445 plone.app.users-3.0.0b4/plone.app.users.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    23530 2022-10-11 20:58:10.000000 plone.app.users-3.0.0b4/plone.app.users.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2836 2022-10-11 20:58:10.000000 plone.app.users-3.0.0b4/plone.app.users.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-10-11 20:58:10.000000 plone.app.users-3.0.0b4/plone.app.users.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2022-10-11 20:58:10.000000 plone.app.users-3.0.0b4/plone.app.users.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2022-10-11 20:58:10.000000 plone.app.users-3.0.0b4/plone.app.users.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-10-11 20:58:10.000000 plone.app.users-3.0.0b4/plone.app.users.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      366 2022-10-11 20:58:10.000000 plone.app.users-3.0.0b4/plone.app.users.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-10-11 20:58:10.000000 plone.app.users-3.0.0b4/plone.app.users.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       67 2022-10-11 20:58:10.787063 plone.app.users-3.0.0b4/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2143 2022-10-11 20:58:09.000000 plone.app.users-3.0.0b4/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:16:13.057855 plone.app.users-3.0.1/
+-rw-r--r--   0 maurits    (501) staff       (20)    20467 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    24014 2023-03-14 16:16:13.057997 plone.app.users-3.0.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2560 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:16:13.036503 plone.app.users-3.0.1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      677 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:16:13.036846 plone.app.users-3.0.1/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:16:13.039574 plone.app.users-3.0.1/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:16:13.042512 plone.app.users-3.0.1/plone/app/users/
+-rw-r--r--   0 maurits    (501) staff       (20)      637 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/TODO.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:16:13.048721 plone.app.users-3.0.1/plone/app/users/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1866 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/account-configlet.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1277 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/account-panel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    13616 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/account.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3435 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2569 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1524 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/memberregistration.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3715 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/membersearch.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4117 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/membersearch_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1020 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/newuser_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5683 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/passwordpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3683 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/personalpreferences.py
+-rw-r--r--   0 maurits    (501) staff       (20)    30400 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/register.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1586 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/register_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4688 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/registered.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      598 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/registered.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2826 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/registersettingspanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1710 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/schema_layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10199 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3889 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/browser/userdatapanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3017 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2173 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/field_extender.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:16:13.033409 plone.app.users-3.0.1/plone/app/users/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:16:13.049371 plone.app.users-3.0.1/plone/app/users/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1977 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/profiles/default/userschema.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     5905 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/schema.py
+-rw-r--r--   0 maurits    (501) staff       (20)      717 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1440 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:16:13.057306 plone.app.users-3.0.1/plone/app/users/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:16:13.057607 plone.app.users-3.0.1/plone/app/users/tests/acceptance/
+-rw-r--r--   0 maurits    (501) staff       (20)     9670 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/acceptance/test_edit_user_schema.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     5110 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1997 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/duplicate_email.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4463 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/email_login.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7625 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/flexible_user_registration.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2712 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/forms_navigationroot.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3275 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/member_search.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      306 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/onepixel.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)     5282 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/password.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4060 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/personal_preferences.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3645 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/personal_preferences_prefs_user_details.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4246 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/plugins.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    15438 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/registration_forms.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1702 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/test_account.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1113 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8313 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/test_exportimport.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2423 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/test_loginname_generator.py
+-rw-r--r--   0 maurits    (501) staff       (20)      559 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/test_member_search.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8587 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/test_new_user.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1828 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/test_pam.py
+-rw-r--r--   0 maurits    (501) staff       (20)      753 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12421 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/test_schema_types.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1214 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/test_user_data_panel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5218 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/test_userid_generator.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6049 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/userdata.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2730 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/tests/userdata_prefs_user_details.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3759 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)      684 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4437 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone/app/users/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 16:16:13.039288 plone.app.users-3.0.1/plone.app.users.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    24014 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone.app.users.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2836 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone.app.users.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone.app.users.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone.app.users.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone.app.users.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone.app.users.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      366 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone.app.users.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/plone.app.users.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      397 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       67 2023-03-14 16:16:13.058601 plone.app.users-3.0.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2220 2023-03-14 16:16:12.000000 plone.app.users-3.0.1/setup.py
```

### Comparing `plone.app.users-3.0.0b4/CHANGES.rst` & `plone.app.users-3.0.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,35 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.1 (2023-03-14)
+------------------
+
+Bug fixes:
+
+
+- Import more from plone.base. [maurits] (#1)
+
+
+3.0.0 (2022-11-11)
+------------------
+
+Bug fixes:
+
+
+- For user schemas use a volatile cache on the request instead of on the portal.
+  This prevents seeing an empty user profile when you have custom user schemas.
+  This fixes `issue 76 <https://github.com/plone/plone.app.users/issues/76>`_.
+  [maurits] (#76)
+
+
 3.0.0b4 (2022-10-11)
 --------------------
 
 Bug fixes:
 
 
 - Fix admin password in tests. [davisagli] (#113)
```

### Comparing `plone.app.users-3.0.0b4/PKG-INFO` & `plone.app.users-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.users
-Version: 3.0.0b4
+Version: 3.0.1
 Summary: A package for all things users and groups related (specific to plone)
 Home-page: https://pypi.org/project/plone.app.users
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Zope CMF Plone Users Groups
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,16 @@
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Introduction
 ============
 
 This package provides the registration form and the user profile form.
 It allows the site administrator to define the fields those forms will display.
@@ -91,14 +93,35 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.1 (2023-03-14)
+------------------
+
+Bug fixes:
+
+
+- Import more from plone.base. [maurits] (#1)
+
+
+3.0.0 (2022-11-11)
+------------------
+
+Bug fixes:
+
+
+- For user schemas use a volatile cache on the request instead of on the portal.
+  This prevents seeing an empty user profile when you have custom user schemas.
+  This fixes `issue 76 <https://github.com/plone/plone.app.users/issues/76>`_.
+  [maurits] (#76)
+
+
 3.0.0b4 (2022-10-11)
 --------------------
 
 Bug fixes:
 
 
 - Fix admin password in tests. [davisagli] (#113)
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: plone.app.users Version: 3.0.0b4 Summary: A package
+Metadata-Version: 2.1 Name: plone.app.users Version: 3.0.1 Summary: A package
 for all things users and groups related (specific to plone) Home-page: https://
 pypi.org/project/plone.app.users Author: Plone Foundation Author-email: plone-
 developers@lists.sourceforge.net License: GPL version 2 Keywords: Zope CMF
 Plone Users Groups Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 5 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Provides-Extra: test
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.8 Provides-Extra: test
 Introduction ============ This package provides the registration form and the
 user profile form. It allows the site administrator to define the fields those
 forms will display. Overriding / extending the default schema
 ========================================= Manipulating the user schema through
 the web -------------------------------------------- In Plone setup / Users and
 Groups / Member fields, we can add and modify the user fields using the
 `plone.schemaeditor`_ interface. Once a new field is added, we can access its
@@ -31,90 +32,96 @@
 ``portal_setup``. Note: the ``userschema.xml`` importation will automatically
 refresh the memberdata attributes, so the ``memberdata_properties.xml`` file is
 not needed. .. _plone.schemaeditor: https://github.com/plone/plone.schemaeditor
 .. _plone.supermodel: https://github.com/plone/plone.supermodel Changelog
 ========= .. You should *NOT* be adding new change log entries to this file.
 You should create a file in the news directory instead. For helpful
 instructions, please see: https://github.com/plone/plone.releaser/blob/master/
-ADD-A-NEWS-ITEM.rst .. towncrier release notes start 3.0.0b4 (2022-10-11) -----
---------------- Bug fixes: - Fix admin password in tests. [davisagli] (#113)
-3.0.0b3 (2022-10-02) -------------------- Bug fixes: - Use longer passwords in
-tests. [davisagli] (#112) 3.0.0b2 (2022-09-01) -------------------- Bug fixes:
-- Ensure that, when no timezone is selected, the value of the stored timezone
-is an empty string (#109) 3.0.0b1 (2022-07-19) -------------------- Bug fixes:
-- Change default msgids for translations [erral] (#108) 3.0.0a7 (2022-03-23) --
------------------- Bug fixes: - Fixed tests when run with ``zope.component``
-5+. [maurits] (#500) 3.0.0a6 (2022-02-24) -------------------- New features: -
-Show unfiltered member fields for manager in user profile page [MrTango] (#106)
-3.0.0a5 (2021-12-29) -------------------- Bug fixes: - Test fix: remove
-deprecated ustring handling, which is only needed on Python 2. [maurits]
-(#3305) 3.0.0a4 (2021-10-13) -------------------- Bug fixes: - Use registry API
-to access usergroup settings. Removes usages of deprecated API. [jensens]
-(#104) 3.0.0a3 (2021-09-15) -------------------- Bug fixes: - Remove cyclic
-dependency with Products.CMFPlone [sneridagh] (#102) 3.0.0a2 (2021-08-04) -----
---------------- Bug fixes: - Split up the chaotic navigation in users and
-groups into its parts. [jensens] (#1) 3.0.0a1 (2021-04-21) -------------------
-- Breaking changes: - Update for Plone 6 with Bootstrap markup Fix registration
-form test [petschki, jensens, agitator] (#98) - Update account-panel for Plone
-6 with Bootstrap markup [1letter] (#99) 2.6.6 (2021-01-08) -----------------
-- Bug fixes: - Fix setting "Use site default" for wysiwyg_editor. Fix https://
-github.com/plone/Products.CMFPlone/issues/3173 [pbauer] (#95) 2.6.5 (2020-07-
-17) ------------------ Bug fixes: - Remove unneeded arrow next to Site Setup
-button in "Edit Member Form Fields" controlpanel. [vincentfretin] (#93) 2.6.4
-(2020-05-06) ------------------ New features: - Doctest markup generalization
-[petschki] (#92) 2.6.3 (2020-04-20) ------------------ Bug fixes: - Minor
-packaging updates. (#1) 2.6.2 (2019-10-21) ------------------ Bug fixes: -
-Error happening during user add notification is logged. (#85) - User feedback
-if error happens during user add notification. (#86) - Fix default value for
-label_msgid. (#88) [erral] 2.6.1 (2019-08-23) ------------------ Bug fixes: -
-Fix many_groups usage in AddUserForm [tmassman] (#83) 2.6.0 (2019-06-27) ------
------------- New features: - Add support for Python 3.8 [pbauer] (#82) Bug
-fixes: - Fix missing i18n:translate calls [erral] (#80) 2.5.1 (2019-06-19) ----
--------------- Bug fixes: - Improve test assertion [ale-rt] (#78) 2.5.0 (2018-
-11-02) ------------------ New features: - Add support for Python 3. [pbauer]
-Bug fixes: - Remove dependency on plone.app.controlpanel. [jensens] - Fix
-browser test to use name of user/password field instead of label. [jensens] -
-Import ``activatePluginInterfaces`` from canonical location in PlonePAS.
-[maurits] - Move forgotten 'registered' template from Products.CMFPlone skins
-to here, were it belongs to. [jensens] - Don't depend on ZODB version directly.
-Rely on Zope dependency [tomgross] - Remove dependency on PloneTestCase
-[pbauer] 2.4.2 (2018-04-03) ------------------ Bug fixes: - Make
-``IUserDataSchema.email`` field ``description`` translatable. [jensens] 2.4.1
-(2018-02-05) ------------------ Bug fixes: - Provide the UserDataPanelAdapter
-for INavigationRoot, so @@personal-information is not broken with
-p.a.multilingual [ebrehault] - Fix tests to avoid using testbrowser internals.
-[davisagli] - Python 3 fixes. [pbauer] - Fix tests to avoid using testbrowser
-internals. [davisagli] 2.4 (2017-06-20) ---------------- New features: - Use
-``get_portal`` from Products.CMFPlone.utils instead of ``getSite``. For
-plone.app.users we always want the Plone portal object until this package is
-fixed to support individual subsite settings. This requires ``Products.CMFPlone
-5.1a2`` or higher. [thet] Bug fixes: - Remove dependency on ``zope.site``.
-[thet] - Code cleanup. [thet] 2.3.8 (2016-09-23) ------------------ Bug fixes:
-- Give a 404 when the user-information form is called with a not existing
-userid. [maurits] - Don't show unescaped user id in user-information form. This
-applies PloneHotfix20160830. [maurits] 2.3.7 (2016-08-18) -----------------
-- Bug fixes: - Use zope.interface decorator. [gforcada] 2.3.6 (2016-05-12) ----
--------------- Fixes: - Fixed KeyError email on personal preferences form. This
-could happen when email is used as login name. Fixes https://github.com/plone/
-plone.app.users/issues/56 and https://github.com/plone/Products.CMFPlone/
-issues/1146 [maurits] - Ensured partial searching utility for users in 'Search
-for users' page Fixes https://github.com/plone/Products.CMFPlone/issues/1499
-[kkhan] - Use ProtectedEmail for Email field factory [ebrehault] 2.3.5 (2016-
-02-11) ------------------ Fixes: - Fix bug when registering a user by adding a
-schema-setter to UserDataPanelAdapter. [pbauer] 2.3.4 (2015-11-28) ------------
------- Fixes: - Rerelease to fix problem on one of our testing servers.
-[maurits] 2.3.3 (2015-11-28) ------------------ Fixes: - Updated Site Setup
-link in all control panels. Fixes https://github.com/plone/Products.CMFPlone/
-issues/1255 [davilima6] 2.3.2 (2015-10-28) ------------------ Fixes: - Do not
-force "In User Profile" when importing a schema from a GS profile. [ebrehault]
-2.3.1 (2015-08-22) ------------------ - Gave upgrade step destination 1. With
-the previous destination '*' the upgrade step was always offered. [vanrees] -
-Cache schemas in volatile attributes on portal. [gotcha] - Package cleanup.
-[gotcha] - Disable toolbar buttons on personal preferences [vangheem] - Remove
-extra spaces in userschema.xml messages to avoid i18n extraction warnings.
+ADD-A-NEWS-ITEM.rst .. towncrier release notes start 3.0.1 (2023-03-14) -------
+----------- Bug fixes: - Import more from plone.base. [maurits] (#1) 3.0.0
+(2022-11-11) ------------------ Bug fixes: - For user schemas use a volatile
+cache on the request instead of on the portal. This prevents seeing an empty
+user profile when you have custom user schemas. This fixes `issue 76
+github.com/plone/plone.app.users/issues/76>`_. [maurits] (#76) 3.0.0b4 (2022-
+10-11) -------------------- Bug fixes: - Fix admin password in tests.
+[davisagli] (#113) 3.0.0b3 (2022-10-02) -------------------- Bug fixes: - Use
+longer passwords in tests. [davisagli] (#112) 3.0.0b2 (2022-09-01) ------------
+-------- Bug fixes: - Ensure that, when no timezone is selected, the value of
+the stored timezone is an empty string (#109) 3.0.0b1 (2022-07-19) ------------
+-------- Bug fixes: - Change default msgids for translations [erral] (#108)
+3.0.0a7 (2022-03-23) -------------------- Bug fixes: - Fixed tests when run
+with ``zope.component`` 5+. [maurits] (#500) 3.0.0a6 (2022-02-24) -------------
+------- New features: - Show unfiltered member fields for manager in user
+profile page [MrTango] (#106) 3.0.0a5 (2021-12-29) -------------------- Bug
+fixes: - Test fix: remove deprecated ustring handling, which is only needed on
+Python 2. [maurits] (#3305) 3.0.0a4 (2021-10-13) -------------------- Bug
+fixes: - Use registry API to access usergroup settings. Removes usages of
+deprecated API. [jensens] (#104) 3.0.0a3 (2021-09-15) -------------------- Bug
+fixes: - Remove cyclic dependency with Products.CMFPlone [sneridagh] (#102)
+3.0.0a2 (2021-08-04) -------------------- Bug fixes: - Split up the chaotic
+navigation in users and groups into its parts. [jensens] (#1) 3.0.0a1 (2021-04-
+21) -------------------- Breaking changes: - Update for Plone 6 with Bootstrap
+markup Fix registration form test [petschki, jensens, agitator] (#98) - Update
+account-panel for Plone 6 with Bootstrap markup [1letter] (#99) 2.6.6 (2021-01-
+08) ------------------ Bug fixes: - Fix setting "Use site default" for
+wysiwyg_editor. Fix https://github.com/plone/Products.CMFPlone/issues/3173
+[pbauer] (#95) 2.6.5 (2020-07-17) ------------------ Bug fixes: - Remove
+unneeded arrow next to Site Setup button in "Edit Member Form Fields"
+controlpanel. [vincentfretin] (#93) 2.6.4 (2020-05-06) ------------------ New
+features: - Doctest markup generalization [petschki] (#92) 2.6.3 (2020-04-20) -
+----------------- Bug fixes: - Minor packaging updates. (#1) 2.6.2 (2019-10-21)
+------------------ Bug fixes: - Error happening during user add notification is
+logged. (#85) - User feedback if error happens during user add notification.
+(#86) - Fix default value for label_msgid. (#88) [erral] 2.6.1 (2019-08-23) ---
+--------------- Bug fixes: - Fix many_groups usage in AddUserForm [tmassman]
+(#83) 2.6.0 (2019-06-27) ------------------ New features: - Add support for
+Python 3.8 [pbauer] (#82) Bug fixes: - Fix missing i18n:translate calls [erral]
+(#80) 2.5.1 (2019-06-19) ------------------ Bug fixes: - Improve test assertion
+[ale-rt] (#78) 2.5.0 (2018-11-02) ------------------ New features: - Add
+support for Python 3. [pbauer] Bug fixes: - Remove dependency on
+plone.app.controlpanel. [jensens] - Fix browser test to use name of user/
+password field instead of label. [jensens] - Import
+``activatePluginInterfaces`` from canonical location in PlonePAS. [maurits] -
+Move forgotten 'registered' template from Products.CMFPlone skins to here, were
+it belongs to. [jensens] - Don't depend on ZODB version directly. Rely on Zope
+dependency [tomgross] - Remove dependency on PloneTestCase [pbauer] 2.4.2
+(2018-04-03) ------------------ Bug fixes: - Make ``IUserDataSchema.email``
+field ``description`` translatable. [jensens] 2.4.1 (2018-02-05) --------------
+---- Bug fixes: - Provide the UserDataPanelAdapter for INavigationRoot, so
+@@personal-information is not broken with p.a.multilingual [ebrehault] - Fix
+tests to avoid using testbrowser internals. [davisagli] - Python 3 fixes.
+[pbauer] - Fix tests to avoid using testbrowser internals. [davisagli] 2.4
+(2017-06-20) ---------------- New features: - Use ``get_portal`` from
+Products.CMFPlone.utils instead of ``getSite``. For plone.app.users we always
+want the Plone portal object until this package is fixed to support individual
+subsite settings. This requires ``Products.CMFPlone 5.1a2`` or higher. [thet]
+Bug fixes: - Remove dependency on ``zope.site``. [thet] - Code cleanup. [thet]
+2.3.8 (2016-09-23) ------------------ Bug fixes: - Give a 404 when the user-
+information form is called with a not existing userid. [maurits] - Don't show
+unescaped user id in user-information form. This applies PloneHotfix20160830.
+[maurits] 2.3.7 (2016-08-18) ------------------ Bug fixes: - Use zope.interface
+decorator. [gforcada] 2.3.6 (2016-05-12) ------------------ Fixes: - Fixed
+KeyError email on personal preferences form. This could happen when email is
+used as login name. Fixes https://github.com/plone/plone.app.users/issues/56
+and https://github.com/plone/Products.CMFPlone/issues/1146 [maurits] - Ensured
+partial searching utility for users in 'Search for users' page Fixes https://
+github.com/plone/Products.CMFPlone/issues/1499 [kkhan] - Use ProtectedEmail for
+Email field factory [ebrehault] 2.3.5 (2016-02-11) ------------------ Fixes: -
+Fix bug when registering a user by adding a schema-setter to
+UserDataPanelAdapter. [pbauer] 2.3.4 (2015-11-28) ------------------ Fixes: -
+Rerelease to fix problem on one of our testing servers. [maurits] 2.3.3 (2015-
+11-28) ------------------ Fixes: - Updated Site Setup link in all control
+panels. Fixes https://github.com/plone/Products.CMFPlone/issues/1255
+[davilima6] 2.3.2 (2015-10-28) ------------------ Fixes: - Do not force "In
+User Profile" when importing a schema from a GS profile. [ebrehault] 2.3.1
+(2015-08-22) ------------------ - Gave upgrade step destination 1. With the
+previous destination '*' the upgrade step was always offered. [vanrees] - Cache
+schemas in volatile attributes on portal. [gotcha] - Package cleanup. [gotcha]
+- Disable toolbar buttons on personal preferences [vangheem] - Remove extra
+spaces in userschema.xml messages to avoid i18n extraction warnings.
 [vincentfretin] 2.3 (2015-07-18) ---------------- - Implement ttw editable
 schemas [ebrehault, kiorky] - Added upgrade step to move past Plone to user
 editable member schema. [ianderso] - Split personal information schema into
 required and ttw editable schemas [ianderso, ljb, stevem] - Updated tests to
 reflect current status of the product. [stevem] - Added ttw editable schema for
 personal information. [ianderso, ljb, stevem] - Removed ext_editor and
 visible_ids preferences. [davisagli] - Made save buttons "blue" [agitator]
```

### Comparing `plone.app.users-3.0.0b4/README.rst` & `plone.app.users-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/docs/LICENSE.GPL` & `plone.app.users-3.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/docs/LICENSE.txt` & `plone.app.users-3.0.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/TODO.txt` & `plone.app.users-3.0.1/plone/app/users/TODO.txt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/account-configlet.pt` & `plone.app.users-3.0.1/plone/app/users/browser/account-configlet.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/account-panel.pt` & `plone.app.users-3.0.1/plone/app/users/browser/account-panel.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/account.py` & `plone.app.users-3.0.1/plone/app/users/browser/account.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # -*- coding: utf-8 -*-
 from AccessControl import Unauthorized
 from Acquisition import aq_inner
+from plone.app.layout.navigation.interfaces import INavigationRoot
 from plone.app.users.browser.interfaces import IAccountPanelForm
+from plone.app.users.browser.schemaeditor import getFromBaseSchema
 from plone.app.users.utils import notifyWidgetActionExecutionError
 from plone.autoform.form import AutoExtensibleForm
 from plone.namedfile.file import NamedBlobImage
 from plone.protect import CheckAuthenticator
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone import PloneMessageFactory as _
 from Products.CMFPlone.controlpanel.events import ConfigurationChangedEvent
-from Products.CMFPlone.interfaces import ISecuritySchema
+from Products.CMFPlone.interfaces import IPloneSiteRoot
+from plone.base.interfaces import ISecuritySchema
 from Products.CMFPlone.utils import safe_unicode
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from Products.PlonePAS.tools.membership import default_portrait
 from Products.statusmessages.interfaces import IStatusMessage
 from z3c.form import button
 from z3c.form import form
 from zope import schema
 from zope.cachedescriptors.property import Lazy as lazy_property
 from zope.component import getMultiAdapter
 from zope.component import getUtility
+from zope.component import provideAdapter
 from zope.event import notify
+from zope.globalrequest import getRequest
 from zope.interface import implementer
 from ZTUtils import make_query
 
 
 MESSAGE_EMAIL_CANNOT_CHANGE = \
     _('message_email_cannot_change',
       default=(u"Sorry, you are not allowed to "
@@ -34,14 +39,52 @@
 MESSAGE_EMAIL_IN_USE = \
     _('message_email_in_use',
       default=(u"The email address you selected is "
                u"already in use or is not valid as login "
                u"name. Please choose another."))
 
 
+def getSchema(schema_interface, schema_adapter, form_name=None):
+    request = getRequest()
+    form_name_to_request_attr_name = {
+        "In User Profile": "_userdata_schema",
+        "On Registration": "_register_schema",
+        None: "_userdata_manager_schema",
+    }
+    request_attr_name = form_name_to_request_attr_name.pop(form_name, None)
+    if request_attr_name is not None:
+        schema = getattr(request, request_attr_name, None)
+    else:
+        schema = None
+    if schema is None:
+        schema = getFromBaseSchema(
+            schema_interface,
+            form_name=form_name
+        )
+        # Unset all request attr names.
+        # We do not want other caches to linger.
+        # See https://github.com/plone/plone.app.users/issues/76
+        # This is in the unlikely case that you visit both the add-user/register form
+        # and the user/personal-information form in one request,
+        # maybe during a migration.
+        for name in form_name_to_request_attr_name.values():
+            try:
+                delattr(request, name)
+            except AttributeError:
+                pass
+        if request_attr_name is not None:
+            setattr(request, request_attr_name, schema)
+        # As schema is a generated supermodel,
+        # needed adapters can only be registered at run time.
+        # Note that this overrides previous adapters for the same interfaces.
+        provideAdapter(schema_adapter, (IPloneSiteRoot,), schema)
+        provideAdapter(schema_adapter, (INavigationRoot,), schema)
+    return schema
+
+
 def isDefaultPortrait(value, portal):
     default_portrait_value = getattr(portal, default_portrait, None)
     return aq_inner(value) == aq_inner(default_portrait_value)
 
 
 class AccountPanelSchemaAdapter(object):
     """Data manager that gets and sets any property mentioned
```

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/configure.zcml` & `plone.app.users-3.0.1/plone/app/users/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/interfaces.py` & `plone.app.users-3.0.1/plone/app/users/browser/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/memberregistration.pt` & `plone.app.users-3.0.1/plone/app/users/browser/memberregistration.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/membersearch.py` & `plone.app.users-3.0.1/plone/app/users/browser/membersearch.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/membersearch_form.pt` & `plone.app.users-3.0.1/plone/app/users/browser/membersearch_form.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/newuser_form.pt` & `plone.app.users-3.0.1/plone/app/users/browser/newuser_form.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/passwordpanel.py` & `plone.app.users-3.0.1/plone/app/users/browser/passwordpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/personalpreferences.py` & `plone.app.users-3.0.1/plone/app/users/browser/personalpreferences.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/register.py` & `plone.app.users-3.0.1/plone/app/users/browser/register.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,66 +1,57 @@
 # -*- coding: utf-8 -*-
 from AccessControl import getSecurityManager
-from Acquisition import aq_inner
 from plone.app.users.browser.account import AccountPanelSchemaAdapter
+from plone.app.users.browser.account import getSchema
 from plone.app.users.browser.interfaces import ILoginNameGenerator
 from plone.app.users.browser.interfaces import IUserIdGenerator
-from plone.app.users.browser.schemaeditor import getFromBaseSchema
 from plone.app.users.schema import IAddUserSchema
 from plone.app.users.schema import ICombinedRegisterSchema
 from plone.app.users.schema import IRegisterSchema
 from plone.app.users.utils import notifyWidgetActionExecutionError
 from plone.app.users.utils import uuid_userid_generator
 from plone.autoform.form import AutoExtensibleForm
 from plone.protect import CheckAuthenticator
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.interfaces import ISiteRoot
 from Products.CMFCore.permissions import ManagePortal
 from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone import PloneMessageFactory as _
-from Products.CMFPlone.interfaces import IPloneSiteRoot
-from Products.CMFPlone.interfaces import ISecuritySchema
-from Products.CMFPlone.interfaces import IUserGroupsSettingsSchema
-from Products.CMFPlone.utils import get_portal
+from plone.base.interfaces import ISecuritySchema
+from plone.base.interfaces import IUserGroupsSettingsSchema
 from Products.CMFPlone.utils import normalizeString
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from Products.statusmessages.interfaces import IStatusMessage
 from z3c.form import button
 from z3c.form import field
 from z3c.form import form
 from z3c.form.browser.checkbox import CheckBoxFieldWidget
 from z3c.form.interfaces import DISPLAY_MODE
 from zExceptions import Forbidden
 from ZODB.POSException import ConflictError
 from zope.component import getAdapter
 from zope.component import getMultiAdapter
 from zope.component import getUtility
-from zope.component import provideAdapter
 from zope.component import queryUtility
 from zope.schema import getFieldNames
 
 import logging
 import six
 
 
 # Number of retries for creating a user id like bob-jones-42:
 RENAME_AFTER_CREATION_ATTEMPTS = 100
 
 
 def getRegisterSchema():
-    portal = get_portal()
-    schema = getattr(portal, '_v_register_schema', None)
-    if schema is None:
-        portal._v_register_schema = schema = getFromBaseSchema(
-            ICombinedRegisterSchema,
-            form_name=u'On Registration'
-        )
-        # as schema is a generated supermodel,
-        # needed adapters can only be registered at run time
-        provideAdapter(AccountPanelSchemaAdapter, (IPloneSiteRoot,), schema)
+    schema = getSchema(
+        ICombinedRegisterSchema,
+        AccountPanelSchemaAdapter,
+        form_name='On Registration',
+    )
     return schema
 
 
 class BaseRegistrationForm(AutoExtensibleForm, form.Form):
     """Form to be used as base for Register and Add User forms."""
     label = u""
     description = u""
@@ -718,8 +709,7 @@
             return
 
         IStatusMessage(self.request).addStatusMessage(
             _(u"User added."), type='info')
         self.request.response.redirect(
             self.context.absolute_url() +
             '/@@usergroup-userprefs?searchstring=' + user_id)
-
```

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/register_form.pt` & `plone.app.users-3.0.1/plone/app/users/browser/register_form.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/registered.pt` & `plone.app.users-3.0.1/plone/app/users/browser/registered.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/registered.py` & `plone.app.users-3.0.1/plone/app/users/browser/registered.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/registersettingspanel.py` & `plone.app.users-3.0.1/plone/app/users/browser/registersettingspanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/schema_layout.pt` & `plone.app.users-3.0.1/plone/app/users/browser/schema_layout.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/schemaeditor.py` & `plone.app.users-3.0.1/plone/app/users/browser/schemaeditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/browser/userdatapanel.py` & `plone.app.users-3.0.1/plone/app/users/browser/userdatapanel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # -*- coding: utf-8 -*-
 from AccessControl.SecurityManagement import getSecurityManager
-from plone.app.layout.navigation.interfaces import INavigationRoot
 from plone.app.users.browser.account import AccountPanelForm
 from plone.app.users.browser.account import AccountPanelSchemaAdapter
-from plone.app.users.browser.schemaeditor import getFromBaseSchema
+from plone.app.users.browser.account import getSchema
 from plone.app.users.schema import IUserDataSchema
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone import PloneMessageFactory as _
-from Products.CMFPlone.interfaces import IPloneSiteRoot
-from Products.CMFPlone.interfaces import ISecuritySchema
+from plone.base.interfaces import ISecuritySchema
 from Products.CMFPlone.utils import get_portal
 from Products.CMFPlone.utils import set_own_login_name
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from zExceptions import NotFound
 from zope.component import getUtility
-from zope.component import provideAdapter
 
 try:
     from html import escape
 except ImportError:
     from cgi import escape
 
 
@@ -99,32 +96,15 @@
 
 
 def getUserDataSchema():
     portal = get_portal()
     form_name = u'In User Profile'
     if getSecurityManager().checkPermission('Manage portal', portal):
         form_name = None
-    if form_name:
-        schema = getattr(portal, '_v_userdata_schema', None)
-    else:
-        schema = getattr(portal, '_v_userdata_manager_schema', None)
-    if schema is None:
-        schema = getFromBaseSchema(
-            IUserDataSchema,
-            form_name=form_name
-        )
-        if form_name:
-            portal._v_userdata_schema = schema
-        else:
-            portal._v_userdata_manager_schema = schema
-        # as schema is a generated supermodel,
-        # needed adapters can only be registered at run time
-        provideAdapter(UserDataPanelAdapter, (IPloneSiteRoot,), schema)
-        provideAdapter(UserDataPanelAdapter, (INavigationRoot,), schema)
+    schema = getSchema(IUserDataSchema, UserDataPanelAdapter, form_name=form_name)
     return schema
 
 
 class UserDataConfiglet(UserDataPanel):
     """Control panel version of the userdata panel"""
     template = ViewPageTemplateFile('account-configlet.pt')
     tab = "userdata"
-
```

### Comparing `plone.app.users-3.0.0b4/plone/app/users/configure.zcml` & `plone.app.users-3.0.1/plone/app/users/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/field_extender.py` & `plone.app.users-3.0.1/plone/app/users/field_extender.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/profiles/default/userschema.xml` & `plone.app.users-3.0.1/plone/app/users/profiles/default/userschema.xml`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/schema.py` & `plone.app.users-3.0.1/plone/app/users/schema.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/setuphandlers.py` & `plone.app.users-3.0.1/plone/app/users/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/testing.py` & `plone.app.users-3.0.1/plone/app/users/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/acceptance/test_edit_user_schema.robot` & `plone.app.users-3.0.1/plone/app/users/tests/acceptance/test_edit_user_schema.robot`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/base.py` & `plone.app.users-3.0.1/plone/app/users/tests/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from OFS.Cache import Cacheable
 from plone.app.testing import setRoles
 from plone.app.testing import login
 from plone.app.testing import TEST_USER_PASSWORD
 from plone.app.users.testing import PLONE_APP_USERS_FUNCTIONAL_TESTING
 from plone.registry.interfaces import IRegistry
 from plone.testing.z2 import Browser
-from Products.CMFPlone.interfaces import ISecuritySchema
+from plone.base.interfaces import ISecuritySchema
 from Products.CMFPlone.interfaces.controlpanel import IMailSchema
 from Products.CMFPlone.tests.utils import MockMailHost
 from Products.MailHost.interfaces import IMailHost
 from Products.PlonePAS.setuphandlers import activatePluginInterfaces
 from Products.PluggableAuthService.interfaces.plugins import IValidationPlugin
 from Products.PluggableAuthService.plugins.BasePlugin import BasePlugin
 from Products.PluggableAuthService.utils import classImplements
```

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/duplicate_email.rst` & `plone.app.users-3.0.1/plone/app/users/tests/duplicate_email.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/email_login.rst` & `plone.app.users-3.0.1/plone/app/users/tests/email_login.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/flexible_user_registration.rst` & `plone.app.users-3.0.1/plone/app/users/tests/flexible_user_registration.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/forms_navigationroot.rst` & `plone.app.users-3.0.1/plone/app/users/tests/forms_navigationroot.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/member_search.rst` & `plone.app.users-3.0.1/plone/app/users/tests/member_search.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/password.rst` & `plone.app.users-3.0.1/plone/app/users/tests/password.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/personal_preferences.rst` & `plone.app.users-3.0.1/plone/app/users/tests/personal_preferences.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/personal_preferences_prefs_user_details.rst` & `plone.app.users-3.0.1/plone/app/users/tests/personal_preferences_prefs_user_details.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/plugins.rst` & `plone.app.users-3.0.1/plone/app/users/tests/plugins.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/registration_forms.rst` & `plone.app.users-3.0.1/plone/app/users/tests/registration_forms.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/test_account.py` & `plone.app.users-3.0.1/plone/app/users/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/test_doctests.py` & `plone.app.users-3.0.1/plone/app/users/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/test_exportimport.py` & `plone.app.users-3.0.1/plone/app/users/tests/test_exportimport.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/test_loginname_generator.py` & `plone.app.users-3.0.1/plone/app/users/tests/test_loginname_generator.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/test_member_search.py` & `plone.app.users-3.0.1/plone/app/users/tests/test_member_search.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/test_new_user.py` & `plone.app.users-3.0.1/plone/app/users/tests/test_new_user.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/test_pam.py` & `plone.app.users-3.0.1/plone/app/users/tests/test_pam.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/test_robot.py` & `plone.app.users-3.0.1/plone/app/users/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/test_user_data_panel.py` & `plone.app.users-3.0.1/plone/app/users/tests/test_user_data_panel.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/test_userid_generator.py` & `plone.app.users-3.0.1/plone/app/users/tests/test_userid_generator.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/userdata.rst` & `plone.app.users-3.0.1/plone/app/users/tests/userdata.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/tests/userdata_prefs_user_details.rst` & `plone.app.users-3.0.1/plone/app/users/tests/userdata_prefs_user_details.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/upgrades.py` & `plone.app.users-3.0.1/plone/app/users/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/utils.py` & `plone.app.users-3.0.1/plone/app/users/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone/app/users/vocabularies.py` & `plone.app.users-3.0.1/plone/app/users/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/plone.app.users.egg-info/PKG-INFO` & `plone.app.users-3.0.1/plone.app.users.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.users
-Version: 3.0.0b4
+Version: 3.0.1
 Summary: A package for all things users and groups related (specific to plone)
 Home-page: https://pypi.org/project/plone.app.users
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Zope CMF Plone Users Groups
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,16 @@
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Introduction
 ============
 
 This package provides the registration form and the user profile form.
 It allows the site administrator to define the fields those forms will display.
@@ -91,14 +93,35 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.1 (2023-03-14)
+------------------
+
+Bug fixes:
+
+
+- Import more from plone.base. [maurits] (#1)
+
+
+3.0.0 (2022-11-11)
+------------------
+
+Bug fixes:
+
+
+- For user schemas use a volatile cache on the request instead of on the portal.
+  This prevents seeing an empty user profile when you have custom user schemas.
+  This fixes `issue 76 <https://github.com/plone/plone.app.users/issues/76>`_.
+  [maurits] (#76)
+
+
 3.0.0b4 (2022-10-11)
 --------------------
 
 Bug fixes:
 
 
 - Fix admin password in tests. [davisagli] (#113)
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: plone.app.users Version: 3.0.0b4 Summary: A package
+Metadata-Version: 2.1 Name: plone.app.users Version: 3.0.1 Summary: A package
 for all things users and groups related (specific to plone) Home-page: https://
 pypi.org/project/plone.app.users Author: Plone Foundation Author-email: plone-
 developers@lists.sourceforge.net License: GPL version 2 Keywords: Zope CMF
 Plone Users Groups Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 5 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Provides-Extra: test
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.8 Provides-Extra: test
 Introduction ============ This package provides the registration form and the
 user profile form. It allows the site administrator to define the fields those
 forms will display. Overriding / extending the default schema
 ========================================= Manipulating the user schema through
 the web -------------------------------------------- In Plone setup / Users and
 Groups / Member fields, we can add and modify the user fields using the
 `plone.schemaeditor`_ interface. Once a new field is added, we can access its
@@ -31,90 +32,96 @@
 ``portal_setup``. Note: the ``userschema.xml`` importation will automatically
 refresh the memberdata attributes, so the ``memberdata_properties.xml`` file is
 not needed. .. _plone.schemaeditor: https://github.com/plone/plone.schemaeditor
 .. _plone.supermodel: https://github.com/plone/plone.supermodel Changelog
 ========= .. You should *NOT* be adding new change log entries to this file.
 You should create a file in the news directory instead. For helpful
 instructions, please see: https://github.com/plone/plone.releaser/blob/master/
-ADD-A-NEWS-ITEM.rst .. towncrier release notes start 3.0.0b4 (2022-10-11) -----
---------------- Bug fixes: - Fix admin password in tests. [davisagli] (#113)
-3.0.0b3 (2022-10-02) -------------------- Bug fixes: - Use longer passwords in
-tests. [davisagli] (#112) 3.0.0b2 (2022-09-01) -------------------- Bug fixes:
-- Ensure that, when no timezone is selected, the value of the stored timezone
-is an empty string (#109) 3.0.0b1 (2022-07-19) -------------------- Bug fixes:
-- Change default msgids for translations [erral] (#108) 3.0.0a7 (2022-03-23) --
------------------- Bug fixes: - Fixed tests when run with ``zope.component``
-5+. [maurits] (#500) 3.0.0a6 (2022-02-24) -------------------- New features: -
-Show unfiltered member fields for manager in user profile page [MrTango] (#106)
-3.0.0a5 (2021-12-29) -------------------- Bug fixes: - Test fix: remove
-deprecated ustring handling, which is only needed on Python 2. [maurits]
-(#3305) 3.0.0a4 (2021-10-13) -------------------- Bug fixes: - Use registry API
-to access usergroup settings. Removes usages of deprecated API. [jensens]
-(#104) 3.0.0a3 (2021-09-15) -------------------- Bug fixes: - Remove cyclic
-dependency with Products.CMFPlone [sneridagh] (#102) 3.0.0a2 (2021-08-04) -----
---------------- Bug fixes: - Split up the chaotic navigation in users and
-groups into its parts. [jensens] (#1) 3.0.0a1 (2021-04-21) -------------------
-- Breaking changes: - Update for Plone 6 with Bootstrap markup Fix registration
-form test [petschki, jensens, agitator] (#98) - Update account-panel for Plone
-6 with Bootstrap markup [1letter] (#99) 2.6.6 (2021-01-08) -----------------
-- Bug fixes: - Fix setting "Use site default" for wysiwyg_editor. Fix https://
-github.com/plone/Products.CMFPlone/issues/3173 [pbauer] (#95) 2.6.5 (2020-07-
-17) ------------------ Bug fixes: - Remove unneeded arrow next to Site Setup
-button in "Edit Member Form Fields" controlpanel. [vincentfretin] (#93) 2.6.4
-(2020-05-06) ------------------ New features: - Doctest markup generalization
-[petschki] (#92) 2.6.3 (2020-04-20) ------------------ Bug fixes: - Minor
-packaging updates. (#1) 2.6.2 (2019-10-21) ------------------ Bug fixes: -
-Error happening during user add notification is logged. (#85) - User feedback
-if error happens during user add notification. (#86) - Fix default value for
-label_msgid. (#88) [erral] 2.6.1 (2019-08-23) ------------------ Bug fixes: -
-Fix many_groups usage in AddUserForm [tmassman] (#83) 2.6.0 (2019-06-27) ------
------------- New features: - Add support for Python 3.8 [pbauer] (#82) Bug
-fixes: - Fix missing i18n:translate calls [erral] (#80) 2.5.1 (2019-06-19) ----
--------------- Bug fixes: - Improve test assertion [ale-rt] (#78) 2.5.0 (2018-
-11-02) ------------------ New features: - Add support for Python 3. [pbauer]
-Bug fixes: - Remove dependency on plone.app.controlpanel. [jensens] - Fix
-browser test to use name of user/password field instead of label. [jensens] -
-Import ``activatePluginInterfaces`` from canonical location in PlonePAS.
-[maurits] - Move forgotten 'registered' template from Products.CMFPlone skins
-to here, were it belongs to. [jensens] - Don't depend on ZODB version directly.
-Rely on Zope dependency [tomgross] - Remove dependency on PloneTestCase
-[pbauer] 2.4.2 (2018-04-03) ------------------ Bug fixes: - Make
-``IUserDataSchema.email`` field ``description`` translatable. [jensens] 2.4.1
-(2018-02-05) ------------------ Bug fixes: - Provide the UserDataPanelAdapter
-for INavigationRoot, so @@personal-information is not broken with
-p.a.multilingual [ebrehault] - Fix tests to avoid using testbrowser internals.
-[davisagli] - Python 3 fixes. [pbauer] - Fix tests to avoid using testbrowser
-internals. [davisagli] 2.4 (2017-06-20) ---------------- New features: - Use
-``get_portal`` from Products.CMFPlone.utils instead of ``getSite``. For
-plone.app.users we always want the Plone portal object until this package is
-fixed to support individual subsite settings. This requires ``Products.CMFPlone
-5.1a2`` or higher. [thet] Bug fixes: - Remove dependency on ``zope.site``.
-[thet] - Code cleanup. [thet] 2.3.8 (2016-09-23) ------------------ Bug fixes:
-- Give a 404 when the user-information form is called with a not existing
-userid. [maurits] - Don't show unescaped user id in user-information form. This
-applies PloneHotfix20160830. [maurits] 2.3.7 (2016-08-18) -----------------
-- Bug fixes: - Use zope.interface decorator. [gforcada] 2.3.6 (2016-05-12) ----
--------------- Fixes: - Fixed KeyError email on personal preferences form. This
-could happen when email is used as login name. Fixes https://github.com/plone/
-plone.app.users/issues/56 and https://github.com/plone/Products.CMFPlone/
-issues/1146 [maurits] - Ensured partial searching utility for users in 'Search
-for users' page Fixes https://github.com/plone/Products.CMFPlone/issues/1499
-[kkhan] - Use ProtectedEmail for Email field factory [ebrehault] 2.3.5 (2016-
-02-11) ------------------ Fixes: - Fix bug when registering a user by adding a
-schema-setter to UserDataPanelAdapter. [pbauer] 2.3.4 (2015-11-28) ------------
------- Fixes: - Rerelease to fix problem on one of our testing servers.
-[maurits] 2.3.3 (2015-11-28) ------------------ Fixes: - Updated Site Setup
-link in all control panels. Fixes https://github.com/plone/Products.CMFPlone/
-issues/1255 [davilima6] 2.3.2 (2015-10-28) ------------------ Fixes: - Do not
-force "In User Profile" when importing a schema from a GS profile. [ebrehault]
-2.3.1 (2015-08-22) ------------------ - Gave upgrade step destination 1. With
-the previous destination '*' the upgrade step was always offered. [vanrees] -
-Cache schemas in volatile attributes on portal. [gotcha] - Package cleanup.
-[gotcha] - Disable toolbar buttons on personal preferences [vangheem] - Remove
-extra spaces in userschema.xml messages to avoid i18n extraction warnings.
+ADD-A-NEWS-ITEM.rst .. towncrier release notes start 3.0.1 (2023-03-14) -------
+----------- Bug fixes: - Import more from plone.base. [maurits] (#1) 3.0.0
+(2022-11-11) ------------------ Bug fixes: - For user schemas use a volatile
+cache on the request instead of on the portal. This prevents seeing an empty
+user profile when you have custom user schemas. This fixes `issue 76
+github.com/plone/plone.app.users/issues/76>`_. [maurits] (#76) 3.0.0b4 (2022-
+10-11) -------------------- Bug fixes: - Fix admin password in tests.
+[davisagli] (#113) 3.0.0b3 (2022-10-02) -------------------- Bug fixes: - Use
+longer passwords in tests. [davisagli] (#112) 3.0.0b2 (2022-09-01) ------------
+-------- Bug fixes: - Ensure that, when no timezone is selected, the value of
+the stored timezone is an empty string (#109) 3.0.0b1 (2022-07-19) ------------
+-------- Bug fixes: - Change default msgids for translations [erral] (#108)
+3.0.0a7 (2022-03-23) -------------------- Bug fixes: - Fixed tests when run
+with ``zope.component`` 5+. [maurits] (#500) 3.0.0a6 (2022-02-24) -------------
+------- New features: - Show unfiltered member fields for manager in user
+profile page [MrTango] (#106) 3.0.0a5 (2021-12-29) -------------------- Bug
+fixes: - Test fix: remove deprecated ustring handling, which is only needed on
+Python 2. [maurits] (#3305) 3.0.0a4 (2021-10-13) -------------------- Bug
+fixes: - Use registry API to access usergroup settings. Removes usages of
+deprecated API. [jensens] (#104) 3.0.0a3 (2021-09-15) -------------------- Bug
+fixes: - Remove cyclic dependency with Products.CMFPlone [sneridagh] (#102)
+3.0.0a2 (2021-08-04) -------------------- Bug fixes: - Split up the chaotic
+navigation in users and groups into its parts. [jensens] (#1) 3.0.0a1 (2021-04-
+21) -------------------- Breaking changes: - Update for Plone 6 with Bootstrap
+markup Fix registration form test [petschki, jensens, agitator] (#98) - Update
+account-panel for Plone 6 with Bootstrap markup [1letter] (#99) 2.6.6 (2021-01-
+08) ------------------ Bug fixes: - Fix setting "Use site default" for
+wysiwyg_editor. Fix https://github.com/plone/Products.CMFPlone/issues/3173
+[pbauer] (#95) 2.6.5 (2020-07-17) ------------------ Bug fixes: - Remove
+unneeded arrow next to Site Setup button in "Edit Member Form Fields"
+controlpanel. [vincentfretin] (#93) 2.6.4 (2020-05-06) ------------------ New
+features: - Doctest markup generalization [petschki] (#92) 2.6.3 (2020-04-20) -
+----------------- Bug fixes: - Minor packaging updates. (#1) 2.6.2 (2019-10-21)
+------------------ Bug fixes: - Error happening during user add notification is
+logged. (#85) - User feedback if error happens during user add notification.
+(#86) - Fix default value for label_msgid. (#88) [erral] 2.6.1 (2019-08-23) ---
+--------------- Bug fixes: - Fix many_groups usage in AddUserForm [tmassman]
+(#83) 2.6.0 (2019-06-27) ------------------ New features: - Add support for
+Python 3.8 [pbauer] (#82) Bug fixes: - Fix missing i18n:translate calls [erral]
+(#80) 2.5.1 (2019-06-19) ------------------ Bug fixes: - Improve test assertion
+[ale-rt] (#78) 2.5.0 (2018-11-02) ------------------ New features: - Add
+support for Python 3. [pbauer] Bug fixes: - Remove dependency on
+plone.app.controlpanel. [jensens] - Fix browser test to use name of user/
+password field instead of label. [jensens] - Import
+``activatePluginInterfaces`` from canonical location in PlonePAS. [maurits] -
+Move forgotten 'registered' template from Products.CMFPlone skins to here, were
+it belongs to. [jensens] - Don't depend on ZODB version directly. Rely on Zope
+dependency [tomgross] - Remove dependency on PloneTestCase [pbauer] 2.4.2
+(2018-04-03) ------------------ Bug fixes: - Make ``IUserDataSchema.email``
+field ``description`` translatable. [jensens] 2.4.1 (2018-02-05) --------------
+---- Bug fixes: - Provide the UserDataPanelAdapter for INavigationRoot, so
+@@personal-information is not broken with p.a.multilingual [ebrehault] - Fix
+tests to avoid using testbrowser internals. [davisagli] - Python 3 fixes.
+[pbauer] - Fix tests to avoid using testbrowser internals. [davisagli] 2.4
+(2017-06-20) ---------------- New features: - Use ``get_portal`` from
+Products.CMFPlone.utils instead of ``getSite``. For plone.app.users we always
+want the Plone portal object until this package is fixed to support individual
+subsite settings. This requires ``Products.CMFPlone 5.1a2`` or higher. [thet]
+Bug fixes: - Remove dependency on ``zope.site``. [thet] - Code cleanup. [thet]
+2.3.8 (2016-09-23) ------------------ Bug fixes: - Give a 404 when the user-
+information form is called with a not existing userid. [maurits] - Don't show
+unescaped user id in user-information form. This applies PloneHotfix20160830.
+[maurits] 2.3.7 (2016-08-18) ------------------ Bug fixes: - Use zope.interface
+decorator. [gforcada] 2.3.6 (2016-05-12) ------------------ Fixes: - Fixed
+KeyError email on personal preferences form. This could happen when email is
+used as login name. Fixes https://github.com/plone/plone.app.users/issues/56
+and https://github.com/plone/Products.CMFPlone/issues/1146 [maurits] - Ensured
+partial searching utility for users in 'Search for users' page Fixes https://
+github.com/plone/Products.CMFPlone/issues/1499 [kkhan] - Use ProtectedEmail for
+Email field factory [ebrehault] 2.3.5 (2016-02-11) ------------------ Fixes: -
+Fix bug when registering a user by adding a schema-setter to
+UserDataPanelAdapter. [pbauer] 2.3.4 (2015-11-28) ------------------ Fixes: -
+Rerelease to fix problem on one of our testing servers. [maurits] 2.3.3 (2015-
+11-28) ------------------ Fixes: - Updated Site Setup link in all control
+panels. Fixes https://github.com/plone/Products.CMFPlone/issues/1255
+[davilima6] 2.3.2 (2015-10-28) ------------------ Fixes: - Do not force "In
+User Profile" when importing a schema from a GS profile. [ebrehault] 2.3.1
+(2015-08-22) ------------------ - Gave upgrade step destination 1. With the
+previous destination '*' the upgrade step was always offered. [vanrees] - Cache
+schemas in volatile attributes on portal. [gotcha] - Package cleanup. [gotcha]
+- Disable toolbar buttons on personal preferences [vangheem] - Remove extra
+spaces in userschema.xml messages to avoid i18n extraction warnings.
 [vincentfretin] 2.3 (2015-07-18) ---------------- - Implement ttw editable
 schemas [ebrehault, kiorky] - Added upgrade step to move past Plone to user
 editable member schema. [ianderso] - Split personal information schema into
 required and ttw editable schemas [ianderso, ljb, stevem] - Updated tests to
 reflect current status of the product. [stevem] - Added ttw editable schema for
 personal information. [ianderso, ljb, stevem] - Removed ext_editor and
 visible_ids preferences. [davisagli] - Made save buttons "blue" [agitator]
```

### Comparing `plone.app.users-3.0.0b4/plone.app.users.egg-info/SOURCES.txt` & `plone.app.users-3.0.1/plone.app.users.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.0b4/setup.py` & `plone.app.users-3.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
-version = '3.0.0b4'
+version = '3.0.1'
 
 long_description = u'{0}\n\n{1}'.format(
     open('README.rst').read(),
     open('CHANGES.rst').read()
 )
 
 extras_require = {
@@ -32,24 +32,26 @@
         "Framework :: Zope :: 5",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords='Zope CMF Plone Users Groups',
     author='Plone Foundation',
     author_email='plone-developers@lists.sourceforge.net',
     url='https://pypi.org/project/plone.app.users',
     license='GPL version 2',
     packages=find_packages(),
     namespace_packages=['plone', 'plone.app'],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     extras_require=extras_require,
     install_requires=[
         'AccessControl',
         'Acquisition',
         'Products.CMFCore',
         'Products.PlonePAS >= 5.0.1',
         'Products.statusmessages',
```

