# Comparing `tmp/plone.app.discussion-4.0.0b3.tar.gz` & `tmp/plone.app.discussion-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.discussion-4.0.0b3.tar", last modified: Tue Oct 11 20:53:44 2022, max compression
+gzip compressed data, was "plone.app.discussion-4.0.1.tar", last modified: Thu Apr 13 23:08:24 2023, max compression
```

## Comparing `plone.app.discussion-4.0.0b3.tar` & `plone.app.discussion-4.0.1.tar`

### file list

```diff
@@ -1,147 +1,126 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.155750 plone.app.discussion-4.0.0b3/
--rw-r--r--   0 maurits    (501) staff       (20)    44332 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      122 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    46958 2022-10-11 20:53:44.155891 plone.app.discussion-4.0.0b3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1736 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.124831 plone.app.discussion-4.0.0b3/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      726 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      106 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/README.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.126577 plone.app.discussion-4.0.0b3/docs/source/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.127414 plone.app.discussion-4.0.0b3/docs/source/api/
--rw-r--r--   0 maurits    (501) staff       (20)       54 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/api/comment.txt
--rw-r--r--   0 maurits    (501) staff       (20)       59 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/api/conversation.txt
--rw-r--r--   0 maurits    (501) staff       (20)      599 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/api/index.txt
--rw-r--r--   0 maurits    (501) staff       (20)       56 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/architecture.txt
--rw-r--r--   0 maurits    (501) staff       (20)       59 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/captcha.txt
--rw-r--r--   0 maurits    (501) staff       (20)     6729 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)       50 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/design.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2148 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/email-notification.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.129459 plone.app.discussion-4.0.0b3/docs/source/howtos/
--rw-r--r--   0 maurits    (501) staff       (20)     5493 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/howtos/howto_extend_the_comment_form.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1242 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/howtos/howto_make_pad_work_with_a_dexterity_content_type.txt
--rw-r--r--   0 maurits    (501) staff       (20)     5116 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/howtos/howto_override_comments_viewlet.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2526 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/howtos/howto_override_enable_conversation.txt
--rw-r--r--   0 maurits    (501) staff       (20)     5038 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/howtos/howto_set_discussion_settings_with_generic_setup.txt
--rw-r--r--   0 maurits    (501) staff       (20)      301 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/howtos/howto_write_a_custom_email_notification.txt
--rw-r--r--   0 maurits    (501) staff       (20)      330 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/howtos/index.txt
--rw-r--r--   0 maurits    (501) staff       (20)      629 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/index.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3670 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/docs/source/workflow.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.129852 plone.app.discussion-4.0.0b3/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.132495 plone.app.discussion-4.0.0b3/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.138235 plone.app.discussion-4.0.0b3/plone/app/discussion/
--rw-r--r--   0 maurits    (501) staff       (20)     3064 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/TODO.txt
--rw-r--r--   0 maurits    (501) staff       (20)       76 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2562 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/architecture.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.141787 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2592 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/captcha.py
--rw-r--r--   0 maurits    (501) staff       (20)     3641 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/captcha.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1267 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/captcha.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4036 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/comment.py
--rw-r--r--   0 maurits    (501) staff       (20)    12326 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/comments.pt
--rw-r--r--   0 maurits    (501) staff       (20)    21238 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/comments.py
--rw-r--r--   0 maurits    (501) staff       (20)     5020 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      747 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9705 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     5496 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/conversation.py
--rw-r--r--   0 maurits    (501) staff       (20)    12989 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/moderation.pt
--rw-r--r--   0 maurits    (501) staff       (20)    15099 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/moderation.py
--rw-r--r--   0 maurits    (501) staff       (20)     1421 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/traversal.py
--rw-r--r--   0 maurits    (501) staff       (20)     2025 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/browser/validator.py
--rw-r--r--   0 maurits    (501) staff       (20)     4460 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)    14871 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/comment.py
--rw-r--r--   0 maurits    (501) staff       (20)      394 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/comment.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4062 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2310 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/contentrules.py
--rw-r--r--   0 maurits    (501) staff       (20)     3435 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/contentrules.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    13840 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/conversation.py
--rw-r--r--   0 maurits    (501) staff       (20)      192 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/conversation.txt
--rw-r--r--   0 maurits    (501) staff       (20)     6886 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/design.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2452 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/events.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.146627 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/
--rw-r--r--   0 maurits    (501) staff       (20)     3497 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-ca.po
--rw-r--r--   0 maurits    (501) staff       (20)     3514 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-cs.po
--rw-r--r--   0 maurits    (501) staff       (20)     3500 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-da.po
--rw-r--r--   0 maurits    (501) staff       (20)     3615 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-de.po
--rw-r--r--   0 maurits    (501) staff       (20)     3813 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-el.po
--rw-r--r--   0 maurits    (501) staff       (20)     3770 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-es.po
--rw-r--r--   0 maurits    (501) staff       (20)     3505 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-eu.po
--rw-r--r--   0 maurits    (501) staff       (20)     3583 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-fr.po
--rw-r--r--   0 maurits    (501) staff       (20)     3408 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-it.po
--rw-r--r--   0 maurits    (501) staff       (20)     3613 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-ja.po
--rw-r--r--   0 maurits    (501) staff       (20)      511 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-manual.pot
--rw-r--r--   0 maurits    (501) staff       (20)     3563 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-nl.po
--rw-r--r--   0 maurits    (501) staff       (20)     2846 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-no.po
--rw-r--r--   0 maurits    (501) staff       (20)     3563 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-pt_BR.po
--rw-r--r--   0 maurits    (501) staff       (20)     4219 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-ru.po
--rw-r--r--   0 maurits    (501) staff       (20)     2873 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-sk.po
--rw-r--r--   0 maurits    (501) staff       (20)     4080 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-uk.po
--rw-r--r--   0 maurits    (501) staff       (20)     3371 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-zh_CN.po
--rw-r--r--   0 maurits    (501) staff       (20)     3410 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone-zh_TW.po
--rw-r--r--   0 maurits    (501) staff       (20)     2873 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/i18n/plone.pot
--rw-r--r--   0 maurits    (501) staff       (20)    13956 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      496 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/notifications.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      688 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.121430 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.149683 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      853 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      145 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      487 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      572 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      201 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1139 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/portal_atct.xml
--rw-r--r--   0 maurits    (501) staff       (20)      244 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1178 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.149947 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)     1039 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/types/Discussion_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)      165 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.121893 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/workflows/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.150173 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/
--rw-r--r--   0 maurits    (501) staff       (20)     2628 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/definition.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.150398 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/workflows/comment_review_workflow/
--rw-r--r--   0 maurits    (501) staff       (20)     7835 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/workflows/comment_review_workflow/definition.xml
--rw-r--r--   0 maurits    (501) staff       (20)      369 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/workflows.xml
--rw-r--r--   0 maurits    (501) staff       (20)      306 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/subscribers.py
--rw-r--r--   0 maurits    (501) staff       (20)     2657 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/subscribers.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4039 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.155042 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3965 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/collection-integration-test.txt
--rw-r--r--   0 maurits    (501) staff       (20)     8931 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/functional_test_comment_review_workflow.txt
--rw-r--r--   0 maurits    (501) staff       (20)    17850 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/functional_test_comments.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.155562 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)     2490 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/robot/test_discussion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2580 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/robot/test_moderation.robot
--rw-r--r--   0 maurits    (501) staff       (20)    20193 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)    19218 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_comment.py
--rw-r--r--   0 maurits    (501) staff       (20)    28427 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_comments_viewlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     5457 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_contentrules.py
--rw-r--r--   0 maurits    (501) staff       (20)     8119 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)    32288 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_conversation.py
--rw-r--r--   0 maurits    (501) staff       (20)     7052 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_events.py
--rw-r--r--   0 maurits    (501) staff       (20)      985 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     7238 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_indexers.py
--rw-r--r--   0 maurits    (501) staff       (20)     4814 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_moderation_multiple_state_view.py
--rw-r--r--   0 maurits    (501) staff       (20)     7623 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_moderation_view.py
--rw-r--r--   0 maurits    (501) staff       (20)    12006 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_notifications.py
--rw-r--r--   0 maurits    (501) staff       (20)      879 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)    12711 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_workflow.py
--rw-r--r--   0 maurits    (501) staff       (20)     2598 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/tool.py
--rw-r--r--   0 maurits    (501) staff       (20)     3021 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     3259 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/upgrades.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2149 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone/app/discussion/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-10-11 20:53:44.132270 plone.app.discussion-4.0.0b3/plone.app.discussion.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    46958 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone.app.discussion.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     5123 2022-10-11 20:53:44.000000 plone.app.discussion-4.0.0b3/plone.app.discussion.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone.app.discussion.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone.app.discussion.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone.app.discussion.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      276 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone.app.discussion.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/plone.app.discussion.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      284 2022-10-11 20:53:44.156978 plone.app.discussion-4.0.0b3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1753 2022-10-11 20:53:43.000000 plone.app.discussion-4.0.0b3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.104374 plone.app.discussion-4.0.1/
+-rw-r--r--   0 maurits    (501) staff       (20)    44676 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    47374 2023-04-13 23:08:24.104516 plone.app.discussion-4.0.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1736 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.074598 plone.app.discussion-4.0.1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      726 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      106 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/README.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.076502 plone.app.discussion-4.0.1/docs/source/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.077516 plone.app.discussion-4.0.1/docs/source/api/
+-rw-r--r--   0 maurits    (501) staff       (20)       54 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/api/comment.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       59 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/api/conversation.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      599 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/api/index.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/architecture.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       59 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/captcha.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     6706 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)       50 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/design.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2148 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/email-notification.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.080272 plone.app.discussion-4.0.1/docs/source/howtos/
+-rw-r--r--   0 maurits    (501) staff       (20)     5493 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/howtos/howto_extend_the_comment_form.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1242 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/howtos/howto_make_pad_work_with_a_dexterity_content_type.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     5116 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/howtos/howto_override_comments_viewlet.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2526 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/howtos/howto_override_enable_conversation.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     5038 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/howtos/howto_set_discussion_settings_with_generic_setup.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      301 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/howtos/howto_write_a_custom_email_notification.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      330 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/howtos/index.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      629 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/index.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3670 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/docs/source/workflow.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.080580 plone.app.discussion-4.0.1/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.082947 plone.app.discussion-4.0.1/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.089297 plone.app.discussion-4.0.1/plone/app/discussion/
+-rw-r--r--   0 maurits    (501) staff       (20)     3064 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/TODO.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       76 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2563 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/architecture.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.093698 plone.app.discussion-4.0.1/plone/app/discussion/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2592 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/captcha.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3641 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/captcha.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1216 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/captcha.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4035 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/comment.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12326 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/comments.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    21248 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/comments.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4789 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      892 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/controlpanel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9705 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2407 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/conversation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15336 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/moderation.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    15100 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/moderation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1420 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/traversal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2025 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/browser/validator.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3786 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15442 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/comment.py
+-rw-r--r--   0 maurits    (501) staff       (20)      394 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/comment.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4253 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2310 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/contentrules.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3554 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/contentrules.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    13839 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/conversation.py
+-rw-r--r--   0 maurits    (501) staff       (20)      192 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/conversation.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     6886 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/design.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2452 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13956 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      501 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/notifications.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      651 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.070852 plone.app.discussion-4.0.1/plone/app/discussion/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.096599 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)     1002 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      170 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      504 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      621 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      247 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1104 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/portal_atct.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      261 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1189 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.096833 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     1182 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/types/Discussion_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      205 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.071342 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.097075 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)     3068 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/definition.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.097350 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/comment_review_workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)     7060 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/comment_review_workflow/definition.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      421 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      255 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/subscribers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2534 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/subscribers.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4037 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.103505 plone.app.discussion-4.0.1/plone/app/discussion/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3965 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/collection-integration-test.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     8931 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/functional_test_comment_review_workflow.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    17844 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/functional_test_comments.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.104058 plone.app.discussion-4.0.1/plone/app/discussion/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)     2490 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/robot/test_discussion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2580 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/robot/test_moderation.robot
+-rw-r--r--   0 maurits    (501) staff       (20)    20481 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)    19247 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_comment.py
+-rw-r--r--   0 maurits    (501) staff       (20)    28444 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_comments_viewlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5457 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_contentrules.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8117 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)    34617 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_conversation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7051 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_events.py
+-rw-r--r--   0 maurits    (501) staff       (20)      985 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8558 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_indexers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4544 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_moderation_multiple_state_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7620 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_moderation_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12004 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_notifications.py
+-rw-r--r--   0 maurits    (501) staff       (20)      879 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12733 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tests/test_workflow.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2597 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/tool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3909 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3685 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/upgrades.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2149 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone/app/discussion/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:08:24.082475 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    47374 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4351 2023-04-13 23:08:24.000000 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      535 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/plone.app.discussion.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1965 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-13 23:08:24.104990 plone.app.discussion-4.0.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2256 2023-04-13 23:08:23.000000 plone.app.discussion-4.0.1/setup.py
```

### Comparing `plone.app.discussion-4.0.0b3/CHANGES.rst` & `plone.app.discussion-4.0.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,36 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.1 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Remove translations folder,
+  for ages they are coming from p.a.locales.
+  [gforcada] (#1)
+- Update configuration files.
+  [plone devs] (#47959565)
+
+
+4.0.0 (2022-11-11)
+------------------
+
+Bug fixes:
+
+
+- Set timezones for creation and modification dates of comments [instification] (#204)
+
+
 4.0.0b3 (2022-10-11)
 --------------------
 
 Bug fixes:
 
 
 - Fix password used in tests.  [davisagli] (#203)
@@ -177,15 +199,15 @@
 
 3.4.0 (2020-04-20)
 ------------------
 
 New features:
 
 
-- Extended existing review workflow by stati ``rejected`` and ``spam``
+- Extended existing review workflow by state ``rejected`` and ``spam``
   Moderation view extended to handle four workflow states.
   [ksuess and precious input of agitator] (#164)
 
 
 Bug fixes:
 
 
@@ -735,15 +757,15 @@
   [toutpt]
 
 
 2.2.10 (2013-09-24)
 -------------------
 
 - Revert "Refactor tests to use the PLONE_APP_CONTENTTYPES_FIXTURE instead of
-  the PLONE_FIXTURE." that has been accidentially introduced into the 2.2.9
+  the PLONE_FIXTURE." that has been accidentally introduced into the 2.2.9
   release.
   [timo]
 
 
 2.2.9 (2013-09-24)
 ------------------
 
@@ -1063,15 +1085,15 @@
 - Remove one_state_workflow customizations.
   [timo]
 
 
 2.0.9 (2011-07-25)
 ------------------
 
-- Make sure the creator index always stores utf-8 encoded stings and not
+- Make sure the creator index always stores utf-8 encoded strings and not
   unicode.
   [timo]
 
 
 2.0.8 (2011-07-25)
 ------------------
```

### Comparing `plone.app.discussion-4.0.0b3/PKG-INFO` & `plone.app.discussion-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.discussion
-Version: 4.0.0b3
+Version: 4.0.1
 Summary: Enhanced discussion support for Plone
 Home-page: https://pypi.org/project/plone.app.discussion
 Author: Timo Stollenwerk - Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: plone discussion
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
 
 
 plone.app.discussion is the commenting system used since Plone 4.1.
@@ -86,14 +88,36 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.1 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Remove translations folder,
+  for ages they are coming from p.a.locales.
+  [gforcada] (#1)
+- Update configuration files.
+  [plone devs] (#47959565)
+
+
+4.0.0 (2022-11-11)
+------------------
+
+Bug fixes:
+
+
+- Set timezones for creation and modification dates of comments [instification] (#204)
+
+
 4.0.0b3 (2022-10-11)
 --------------------
 
 Bug fixes:
 
 
 - Fix password used in tests.  [davisagli] (#203)
@@ -259,15 +283,15 @@
 
 3.4.0 (2020-04-20)
 ------------------
 
 New features:
 
 
-- Extended existing review workflow by stati ``rejected`` and ``spam``
+- Extended existing review workflow by state ``rejected`` and ``spam``
   Moderation view extended to handle four workflow states.
   [ksuess and precious input of agitator] (#164)
 
 
 Bug fixes:
 
 
@@ -817,15 +841,15 @@
   [toutpt]
 
 
 2.2.10 (2013-09-24)
 -------------------
 
 - Revert "Refactor tests to use the PLONE_APP_CONTENTTYPES_FIXTURE instead of
-  the PLONE_FIXTURE." that has been accidentially introduced into the 2.2.9
+  the PLONE_FIXTURE." that has been accidentally introduced into the 2.2.9
   release.
   [timo]
 
 
 2.2.9 (2013-09-24)
 ------------------
 
@@ -1145,15 +1169,15 @@
 - Remove one_state_workflow customizations.
   [timo]
 
 
 2.0.9 (2011-07-25)
 ------------------
 
-- Make sure the creator index always stores utf-8 encoded stings and not
+- Make sure the creator index always stores utf-8 encoded strings and not
   unicode.
   [timo]
 
 
 2.0.8 (2011-07-25)
 ------------------
```

### Comparing `plone.app.discussion-4.0.0b3/README.rst` & `plone.app.discussion-4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/docs/LICENSE.GPL` & `plone.app.discussion-4.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/docs/LICENSE.txt` & `plone.app.discussion-4.0.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/docs/source/api/index.txt` & `plone.app.discussion-4.0.1/docs/source/api/index.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 The conversation is responsible for storing all comments. It provides a
 dict-like API for accessing comments, where keys are integers and values
 are IComment objects. It also provides features for finding comments quickly.
 
 The IReplies adapter provides an API for finding and manipulating the comments
 directly in reply to a particular comment (implemented by the CommentReplies
-adpater) or at the top level of the conversation (implemented by the
+adapter) or at the top level of the conversation (implemented by the
 ConversationReplies adapter).
 
 
 .. toctree::
    :maxdepth: 1
 
    conversation.txt
```

### Comparing `plone.app.discussion-4.0.0b3/docs/source/conf.py` & `plone.app.discussion-4.0.1/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,14 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import os
-import sys
-
-
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 # sys.path.append(os.path.abspath('.'))
 
 # -- General configuration ----------------------------------------------------
```

### Comparing `plone.app.discussion-4.0.0b3/docs/source/email-notification.txt` & `plone.app.discussion-4.0.1/docs/source/email-notification.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/docs/source/howtos/howto_extend_the_comment_form.txt` & `plone.app.discussion-4.0.1/docs/source/howtos/howto_extend_the_comment_form.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/docs/source/howtos/howto_make_pad_work_with_a_dexterity_content_type.txt` & `plone.app.discussion-4.0.1/docs/source/howtos/howto_make_pad_work_with_a_dexterity_content_type.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/docs/source/howtos/howto_override_comments_viewlet.txt` & `plone.app.discussion-4.0.1/docs/source/howtos/howto_override_comments_viewlet.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/docs/source/howtos/howto_override_enable_conversation.txt` & `plone.app.discussion-4.0.1/docs/source/howtos/howto_override_enable_conversation.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/docs/source/howtos/howto_set_discussion_settings_with_generic_setup.txt` & `plone.app.discussion-4.0.1/docs/source/howtos/howto_set_discussion_settings_with_generic_setup.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/docs/source/index.txt` & `plone.app.discussion-4.0.1/docs/source/index.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/docs/source/workflow.txt` & `plone.app.discussion-4.0.1/docs/source/workflow.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/TODO.txt` & `plone.app.discussion-4.0.1/plone/app/discussion/TODO.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/architecture.txt` & `plone.app.discussion-4.0.1/plone/app/discussion/architecture.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   **Discussion items are light weight objects**
     Discussion item objects are as light weight as possible. Ideally, a
     discussion item should be as lightweight as a catalog brain. This may mean
     that we forego convenience base classes and re-implement certain interfaces.
     Comments should not provide the full set of dublin core metadata, though
     custom indexers can be used to provide values for standard catalog indexes.
 
-  **Optimise for retrival speed**
+  **Optimise for retrieval speed**
     HTML filtering and other processing should happen on save, not on render,
     to make rendering quick.
 
   **Settings are stored using plone.registry**
     Any global setting should be stored in plone.registry records.
 
   **Forms are constructed using extensible z3c.form forms**
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/browser/captcha.py` & `plone.app.discussion-4.0.1/plone/app/discussion/browser/captcha.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/browser/captcha.txt` & `plone.app.discussion-4.0.1/plone/app/discussion/browser/captcha.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/browser/captcha.zcml` & `plone.app.discussion-4.0.1/plone/app/discussion/browser/captcha.zcml`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:meta="http://namespaces.zope.org/meta"
     xmlns:zcml="http://namespaces.zope.org/zcml"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
-    <!-- Captcha comment form extender -->
-    <configure zcml:condition="have plone.app.discussion-captcha">
-        <!--
+  <!-- Captcha comment form extender -->
+  <configure zcml:condition="have plone.app.discussion-captcha">
+    <!--
           Register the Captcha form extender and validator only if there are
           plugins installed that declare to implement a Captcha solution for
           plone.app.discussion (e.g. plone.formwidget.captcha and
           plone.formwidget.recaptcha).
         -->
-        <adapter
-            factory=".captcha.Captcha"
-            provides="plone.app.discussion.interfaces.ICaptcha" />
-        <adapter
-            factory=".captcha.CaptchaExtender"
-            provides="plone.z3cform.fieldsets.interfaces.IFormExtender" />
-        <adapter
-            factory=".validator.CaptchaValidator"
-            provides="z3c.form.interfaces.IValidator"
-            />
-    </configure>
+    <adapter
+        factory=".captcha.Captcha"
+        provides="plone.app.discussion.interfaces.ICaptcha"
+        />
+    <adapter
+        factory=".captcha.CaptchaExtender"
+        provides="plone.z3cform.fieldsets.interfaces.IFormExtender"
+        />
+    <adapter
+        factory=".validator.CaptchaValidator"
+        provides="z3c.form.interfaces.IValidator"
+        />
+  </configure>
 
-    <!-- Akismet Validator -->
-    <configure zcml:condition="installed collective.akismet">
-        <adapter
-            factory="collective.akismet.validator.AkismetValidator"
-            provides="z3c.form.interfaces.IValidator"
-            />
-    </configure>
+  <!-- Akismet Validator -->
+  <configure zcml:condition="installed collective.akismet">
+    <adapter
+        factory="collective.akismet.validator.AkismetValidator"
+        provides="z3c.form.interfaces.IValidator"
+        />
+  </configure>
 
 </configure>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/browser/comment.py` & `plone.app.discussion-4.0.1/plone/app/discussion/browser/comment.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,14 @@
                 (self.context, self.request), name="plone_portal_state"
             )
             target = portal_state.portal_url()
         self.request.response.redirect(target)
 
     @button.buttonAndHandler(_("label_save", default="Save"), name="comment")
     def handleComment(self, action):
-
         # Validate form
         data, errors = self.extractData()
         if errors:
             return
 
         # Check permissions
         can_edit = getSecurityManager().checkPermission("Edit comments", self.context)
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/browser/comments.pt` & `plone.app.discussion-4.0.1/plone/app/discussion/browser/comments.pt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/browser/comments.py` & `plone.app.discussion-4.0.1/plone/app/discussion/browser/comments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from AccessControl import getSecurityManager
 from AccessControl import Unauthorized
 from Acquisition import aq_inner
-from datetime import datetime
 from DateTime import DateTime
 from plone.app.discussion import _
 from plone.app.discussion.browser.validator import CaptchaValidator
 from plone.app.discussion.interfaces import ICaptcha
 from plone.app.discussion.interfaces import IComment
 from plone.app.discussion.interfaces import IConversation
 from plone.app.discussion.interfaces import IDiscussionSettings
 from plone.app.discussion.interfaces import IReplies
+from plone.app.event.base import localized_now
 from plone.app.layout.viewlets.common import ViewletBase
 from plone.base.utils import safe_text
 from plone.registry.interfaces import IRegistry
 from plone.z3cform import z2
 from plone.z3cform.fieldsets import extensible
 from plone.z3cform.interfaces import IWrappedForm
 from Products.CMFCore.utils import getToolByName
@@ -56,15 +56,14 @@
 COMMENT_DESCRIPTION_MODERATION_ENABLED = _(
     "comment_description_moderation_enabled",
     default="Comments are moderated.",
 )
 
 
 class CommentForm(extensible.ExtensibleForm, form.Form):
-
     ignoreContext = True  # don't use context to get widget data
     id = None
     label = _("Add a comment")
     fields = field.Fields(IComment).omit(
         "portal_type",
         "__parent__",
         "__name__",
@@ -188,16 +187,16 @@
         comment.mime_type = settings.text_transform
 
         # Set comment attributes (including extended comment form attributes)
         for attribute in self.fields.keys():
             setattr(comment, attribute, data[attribute])
 
         # Set dates
-        comment.creation_date = datetime.utcnow()
-        comment.modification_date = datetime.utcnow()
+        comment.creation_date = localized_now()
+        comment.modification_date = localized_now()
 
         # Get author name and email
         comment.author_name, comment.author_email = self.get_author(data)
 
         # Set comment author properties for anonymous users or members
         portal_membership = getToolByName(context, "portal_membership")
         anon = portal_membership.isAnonymousUser()
@@ -297,15 +296,14 @@
     def handleCancel(self, action):
         # This method should never be called, it's only there to show
         # a cancel button that is handled by a jQuery method.
         pass  # pragma: no cover
 
 
 class CommentsViewlet(ViewletBase):
-
     form = CommentForm
     index = ViewPageTemplateFile("comments.pt")
 
     def update(self):
         super().update()
         discussion_allowed = self.is_discussion_allowed()
         anonymous_allowed_or_can_reply = (
@@ -479,15 +477,14 @@
     def get_commenter_home_url(self, username=None):
         if username is None:
             return None
         else:
             return f"{self.context.portal_url()}/author/{username}"
 
     def get_commenter_portrait(self, username=None):
-
         if username is None:
             # return the default user image if no username is given
             return "defaultUser.png"
         else:
             portal_membership = getToolByName(self.context, "portal_membership", None)
             return portal_membership.getPersonalPortrait(username).absolute_url()
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/browser/configure.zcml` & `plone.app.discussion-4.0.1/plone/app/discussion/browser/configure.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -1,156 +1,160 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
     xmlns:plone="http://namespaces.plone.org/plone"
     xmlns:zcml="http://namespaces.zope.org/zcml"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
-    <include package="plone.app.registry" />
+  <include package="plone.app.registry" />
 
-    <include file="captcha.zcml" />
+  <include file="captcha.zcml" />
 
-    <!-- Traversal adapter -->
-    <adapter factory=".traversal.ConversationNamespace" name="conversation" />
+  <!-- Traversal adapter -->
+  <adapter
+      factory=".traversal.ConversationNamespace"
+      name="conversation"
+      />
+
+  <!-- Moderation view -->
+  <browser:page
+      name="moderate-comments"
+      for="Products.CMFCore.interfaces.ISiteRoot"
+      class=".moderation.View"
+      permission="plone.app.discussion.ReviewComments"
+      layer="..interfaces.IDiscussionLayer"
+      />
+
+  <browser:page
+      name="moderate-comments"
+      for="plone.app.layout.navigation.interfaces.INavigationRoot"
+      class=".moderation.View"
+      permission="plone.app.discussion.ReviewComments"
+      layer="..interfaces.IDiscussionLayer"
+      />
+
+  <!-- Moderation bulk actions view -->
+  <browser:page
+      name="bulk-actions"
+      for="Products.CMFCore.interfaces.ISiteRoot"
+      class=".moderation.BulkActionsView"
+      permission="plone.app.discussion.ReviewComments"
+      layer="..interfaces.IDiscussionLayer"
+      />
+
+  <browser:page
+      name="bulk-actions"
+      for="plone.app.layout.navigation.interfaces.INavigationRoot"
+      class=".moderation.BulkActionsView"
+      permission="plone.app.discussion.ReviewComments"
+      layer="..interfaces.IDiscussionLayer"
+      />
+
+  <!-- Moderate comments enabled view -->
+  <browser:page
+      name="moderate-comments-enabled"
+      for="plone.base.interfaces.IPloneSiteRoot"
+      class=".moderation.ModerateCommentsEnabled"
+      permission="zope2.View"
+      layer="..interfaces.IDiscussionLayer"
+      />
+
+  <browser:page
+      name="moderate-comments-enabled"
+      for="plone.app.layout.navigation.interfaces.INavigationRoot"
+      class=".moderation.ModerateCommentsEnabled"
+      permission="zope2.View"
+      layer="..interfaces.IDiscussionLayer"
+      />
+
+  <!-- Edit comment view -->
+  <browser:page
+      name="edit-comment"
+      for="plone.app.discussion.interfaces.IComment"
+      class=".comment.EditComment"
+      permission="plone.app.discussion.EditComments"
+      layer="..interfaces.IDiscussionLayer"
+      />
 
-    <!-- Moderation view -->
-    <browser:page
-        for="Products.CMFCore.interfaces.ISiteRoot"
-        name="moderate-comments"
-        layer="..interfaces.IDiscussionLayer"
-        class=".moderation.View"
-        permission="plone.app.discussion.ReviewComments"
-        />
-
-    <browser:page
-        for="plone.app.layout.navigation.interfaces.INavigationRoot"
-        name="moderate-comments"
-        layer="..interfaces.IDiscussionLayer"
-        class=".moderation.View"
-        permission="plone.app.discussion.ReviewComments"
-        />
-
-    <!-- Moderation bulk actions view -->
-    <browser:page
-        for="Products.CMFCore.interfaces.ISiteRoot"
-        name="bulk-actions"
-        layer="..interfaces.IDiscussionLayer"
-        class=".moderation.BulkActionsView"
-        permission="plone.app.discussion.ReviewComments"
-        />
-
-    <browser:page
-        for="plone.app.layout.navigation.interfaces.INavigationRoot"
-        name="bulk-actions"
-        layer="..interfaces.IDiscussionLayer"
-        class=".moderation.BulkActionsView"
-        permission="plone.app.discussion.ReviewComments"
-        />
-
-    <!-- Moderate comments enabled view -->
-    <browser:page
-        for="plone.base.interfaces.IPloneSiteRoot"
-        name="moderate-comments-enabled"
-        layer="..interfaces.IDiscussionLayer"
-        class=".moderation.ModerateCommentsEnabled"
-        permission="zope2.View"
-        />
-
-    <browser:page
-        for="plone.app.layout.navigation.interfaces.INavigationRoot"
-        name="moderate-comments-enabled"
-        layer="..interfaces.IDiscussionLayer"
-        class=".moderation.ModerateCommentsEnabled"
-        permission="zope2.View"
-        />
-
-    <!-- Edit comment view -->
-    <browser:page
-        for="plone.app.discussion.interfaces.IComment"
-        name="edit-comment"
-        layer="..interfaces.IDiscussionLayer"
-        class=".comment.EditComment"
-        permission="plone.app.discussion.EditComments"
-        />
-
-    <!-- Delete comment views
+  <!-- Delete comment views
          has conditional security dependent on controlpanel settings.
     -->
-    <browser:page
-        for="plone.app.discussion.interfaces.IComment"
-        name="moderate-delete-comment"
-        layer="..interfaces.IDiscussionLayer"
-        class=".moderation.DeleteComment"
-        permission="plone.app.discussion.DeleteComments"
-        />
-
-    <browser:page
-        for="plone.app.discussion.interfaces.IComment"
-        name="delete-own-comment"
-        layer="..interfaces.IDiscussionLayer"
-        class=".moderation.DeleteOwnComment"
-        permission="plone.app.discussion.DeleteOwnComments"
-        />
-
-    <!-- Comment Transition -->
-    <browser:page
-        for="plone.app.discussion.interfaces.IComment"
-        name="transmit-comment"
-        layer="..interfaces.IDiscussionLayer"
-        class=".moderation.CommentTransition"
-        permission="plone.app.discussion.ReviewComments"
-        />
-
-    <browser:page
-        for="*"
-        name="translationhelper"
-        layer="..interfaces.IDiscussionLayer"
-        class=".moderation.TranslationHelper"
-        permission="plone.app.discussion.ReviewComments"
-        />
-
-
-    <!-- Comments viewlet -->
-    <browser:viewlet
-        name="plone.comments"
-        for="Products.CMFCore.interfaces.IContentish"
-        layer="..interfaces.IDiscussionLayer"
-        manager="plone.app.layout.viewlets.interfaces.IBelowContent"
-        view="plone.app.layout.globals.interfaces.IViewView"
-        class=".comments.CommentsViewlet"
-        permission="plone.app.discussion.ViewComments"
-        />
-
-    <!-- Conversation view -->
-    <browser:page
-        name="conversation_view"
-        for="Products.CMFCore.interfaces.IContentish"
-        layer="..interfaces.IDiscussionLayer"
-        class=".conversation.ConversationView"
-        permission="zope2.View"
-        />
-
-    <!-- Comment view -->
-    <browser:view
-        name="view"
-        for="plone.app.discussion.interfaces.IComment"
-        layer="..interfaces.IDiscussionLayer"
-        class=".comment.View"
-        permission="zope2.View"
-        />
-
-    <!-- Control panel -->
-    <browser:page
-        name="discussion-controlpanel"
-        for="plone.base.interfaces.IPloneSiteRoot"
-        class=".controlpanel.DiscussionSettingsControlPanel"
-        permission="cmf.ManagePortal"
-        />
-    <!-- Deprecated controlpanel url -->
-    <browser:page
-        name="discussion-settings"
-        for="plone.base.interfaces.IPloneSiteRoot"
-        class=".controlpanel.DiscussionSettingsControlPanel"
-        permission="cmf.ManagePortal"
-        />
+  <browser:page
+      name="moderate-delete-comment"
+      for="plone.app.discussion.interfaces.IComment"
+      class=".moderation.DeleteComment"
+      permission="plone.app.discussion.DeleteComments"
+      layer="..interfaces.IDiscussionLayer"
+      />
+
+  <browser:page
+      name="delete-own-comment"
+      for="plone.app.discussion.interfaces.IComment"
+      class=".moderation.DeleteOwnComment"
+      permission="plone.app.discussion.DeleteOwnComments"
+      layer="..interfaces.IDiscussionLayer"
+      />
+
+  <!-- Comment Transition -->
+  <browser:page
+      name="transmit-comment"
+      for="plone.app.discussion.interfaces.IComment"
+      class=".moderation.CommentTransition"
+      permission="plone.app.discussion.ReviewComments"
+      layer="..interfaces.IDiscussionLayer"
+      />
+
+  <browser:page
+      name="translationhelper"
+      for="*"
+      class=".moderation.TranslationHelper"
+      permission="plone.app.discussion.ReviewComments"
+      layer="..interfaces.IDiscussionLayer"
+      />
+
+
+  <!-- Comments viewlet -->
+  <browser:viewlet
+      name="plone.comments"
+      for="Products.CMFCore.interfaces.IContentish"
+      view="plone.app.layout.globals.interfaces.IViewView"
+      manager="plone.app.layout.viewlets.interfaces.IBelowContent"
+      class=".comments.CommentsViewlet"
+      permission="plone.app.discussion.ViewComments"
+      layer="..interfaces.IDiscussionLayer"
+      />
+
+  <!-- Conversation view -->
+  <browser:page
+      name="conversation_view"
+      for="Products.CMFCore.interfaces.IContentish"
+      class=".conversation.ConversationView"
+      permission="zope2.View"
+      layer="..interfaces.IDiscussionLayer"
+      />
+
+  <!-- Comment view -->
+  <browser:view
+      name="view"
+      for="plone.app.discussion.interfaces.IComment"
+      class=".comment.View"
+      permission="zope2.View"
+      layer="..interfaces.IDiscussionLayer"
+      />
+
+  <!-- Control panel -->
+  <browser:page
+      name="discussion-controlpanel"
+      for="plone.base.interfaces.IPloneSiteRoot"
+      class=".controlpanel.DiscussionSettingsControlPanel"
+      permission="cmf.ManagePortal"
+      />
+  <!-- Deprecated controlpanel url -->
+  <browser:page
+      name="discussion-settings"
+      for="plone.base.interfaces.IPloneSiteRoot"
+      class=".controlpanel.DiscussionSettingsControlPanel"
+      permission="cmf.ManagePortal"
+      />
 
 </configure>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/browser/controlpanel.pt` & `plone.app.discussion-4.0.1/plone/app/discussion/browser/controlpanel.pt`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,36 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
       lang="en"
       metal:use-macro="here/prefs_main_template/macros/master"
-      i18n:domain="plone">
-<body>
+      xml:lang="en"
+      i18n:domain="plone"
+>
+  <body>
 
-<metal:main metal:fill-slot="prefs_configlet_main" i18n:domain="plone">
+    <metal:main metal:fill-slot="prefs_configlet_main"
+                i18n:domain="plone"
+    >
 
-    <header>
-      <h1 class="documentFirstHeading" tal:content="view/label">View Title</h1>
-      <p class="lead" tal:content="view/description">Description</p>
-    </header>
+      <header>
+        <h1 class="documentFirstHeading"
+            tal:content="view/label"
+        >View Title</h1>
+        <p class="lead"
+           tal:content="view/description"
+        >Description</p>
+      </header>
 
-    <div id="content-core" tal:attributes="class view/settings">
-      <span tal:replace="structure view/contents" />
-    </div>
+      <div id="content-core"
+           tal:attributes="
+             class view/settings;
+           "
+      >
+        <span tal:replace="structure view/contents"></span>
+      </div>
 
-</metal:main>
+    </metal:main>
 
-</body>
+  </body>
 </html>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/browser/controlpanel.py` & `plone.app.discussion-4.0.1/plone/app/discussion/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/browser/moderation.pt` & `plone.app.discussion-4.0.1/plone/app/discussion/browser/moderation.pt`

 * *Files 13% similar despite different names*

```diff
@@ -1,263 +1,346 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
-  xml:lang="en"
-  xmlns:tal="http://xml.zope.org/namespaces/tal"
-  xmlns:metal="http://xml.zope.org/namespaces/metal"
-  xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-  lang="en"
-  metal:use-macro="context/main_template/macros/master"
-  i18n:domain="plone">
+      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
+      metal:use-macro="context/main_template/macros/master"
+      xml:lang="en"
+      i18n:domain="plone"
+>
   <body>
 
     <metal:override fill-slot="top_slot"
-      tal:define="disable_column_one python:request.set('disable_plone.leftcolumn',1);
-                disable_column_two python:request.set('disable_plone.rightcolumn',1);" />
+                    tal:define="
+                      disable_column_one python:request.set('disable_plone.leftcolumn',1);
+                      disable_column_two python:request.set('disable_plone.rightcolumn',1);
+                    "
+    />
 
     <metal:main fill-slot="main">
       <tal:main-macro metal:define-macro="main"
-        tal:define="toLocalizedTime nocall:context/@@plone/toLocalizedTime;
-                    items view/comments;
-                    filter request/review_state|nothing;
-                    Batch python:modules['Products.CMFPlone'].Batch;
-                    b_size python:30;
-                    b_start python:0;
-                    b_start request/b_start | b_start;
-                    moderation_enabled view/moderation_enabled;
-                    colorclass python:lambda x: 'state-private' if x=='rejected' else ('state-internal' if x=='spam' else 'state-'+x);
-                    translationhelper nocall:context/@@translationhelper;
-                    ">
+                      tal:define="
+                        toLocalizedTime nocall:context/@@plone/toLocalizedTime;
+                        items view/comments;
+                        filter request/review_state|nothing;
+                        Batch python:modules['Products.CMFPlone'].Batch;
+                        b_size python:30;
+                        b_start python:0;
+                        b_start request/b_start | b_start;
+                        moderation_enabled view/moderation_enabled;
+                        colorclass python:lambda x: 'state-private' if x=='rejected' else ('state-internal' if x=='spam' else 'state-'+x);
+                        translationhelper nocall:context/@@translationhelper;
+                      "
+      >
         <style>
             #review-comments th label {
                 margin-right: 1em;
             }
         </style>
 
         <h1 i18n:translate="heading_moderate_comments">
             Moderate comments
         </h1>
         <div class="alert alert-info"
-          role="status"
-          tal:condition="python: not moderation_enabled">
+             role="status"
+             tal:condition="python: not moderation_enabled"
+        >
           <strong>Info</strong>
           <div i18n:translate="message_moderation_disabled">Moderation workflow is disabled. You have to
-            <a i18n:name="enable_comment_workflow"
-              i18n:translate="message_enable_comment_workflow"
-              href=""
-              tal:attributes="href string:${context/portal_url}/@@content-controlpanel?type_id=Discussion Item">
+            <a href=""
+               tal:attributes="
+                 href string:${context/portal_url}/@@content-controlpanel?type_id=Discussion Item;
+               "
+               i18n:name="enable_comment_workflow"
+               i18n:translate="message_enable_comment_workflow"
+            >
             enable the 'Comment Review Workflow' for the Comment content
-            type</a> before you can moderate comments here.</div>
+              type</a>
+            before you can moderate comments here.</div>
         </div>
 
         <form class="mb-3"
-          method="post"
-          action="#"
-          tal:condition="moderation_enabled"
-          tal:attributes="action string:${context/absolute_url}/@@bulk-actions"
-          tal:define="batch python:Batch(items, b_size, int(b_start), orphan=1);">
-          <fieldset id="fieldset-moderate-comments"
-            class="formPanel">
+              action="#"
+              method="post"
+              tal:define="
+                batch python:Batch(items, b_size, int(b_start), orphan=1);
+              "
+              tal:condition="moderation_enabled"
+              tal:attributes="
+                action string:${context/absolute_url}/@@bulk-actions;
+              "
+        >
+          <fieldset class="formPanel"
+                    id="fieldset-moderate-comments"
+          >
 
-            <div metal:use-macro="here/batch_macros/macros/navigation" />
+            <div metal:use-macro="here/batch_macros/macros/navigation"></div>
             <div id="review-comments">
 
               <div class="row row-cols-lg-auto g-3 align-items-center mb-2 mt-2"
-                id="bulkactions">
+                   id="bulkactions"
+              >
                 <tal:bulk condition="items">
                   <div class="col-auto">
                     <select class="form-select"
-                      name="form.select.BulkAction">
+                            name="form.select.BulkAction"
+                    >
                       <option selected="selected"
-                        value="-1"
-                        i18n:translate="title_bulkactions">Bulk Actions</option>
-                      <tal:comment tal:replace="nothing"></tal:comment>
+                              value="-1"
+                              i18n:translate="title_bulkactions"
+                      >Bulk Actions</option>
+                      <tal:comment tal:replace="nothing" />
                       <option value="publish"
-                        i18n:translate="bulkactions_publish"
-                        tal:condition="python: filter != 'published'">Approve</option>
+                              tal:condition="python: filter != 'published'"
+                              i18n:translate="bulkactions_publish"
+                      >Approve</option>
                       <option value="mark_as_spam"
-                        i18n:translate="bulkactions_spam"
-                        tal:condition="python: filter != 'spam'">Spam</option>
+                              tal:condition="python: filter != 'spam'"
+                              i18n:translate="bulkactions_spam"
+                      >Spam</option>
                       <option value="delete"
-                        i18n:translate="bulkactions_delete">Delete</option>
+                              i18n:translate="bulkactions_delete"
+                      >Delete</option>
                     </select>
                   </div>
                   <div class="col-auto">
-                    <input type="hidden"
-                      name="filter"
-                      tal:attributes="value filter" />
+                    <input name="filter"
+                           type="hidden"
+                           tal:attributes="
+                             value filter;
+                           "
+                    />
                     <button class="standalone allowMultiSubmit btn btn-primary"
-                      id="dobulkaction"
-                      type="submit"
-                      value="Apply"
-                      name="form.button.BulkAction"
-                      i18n:attributes="value label_apply;"
-                      i18n:translate="label_apply">Apply</button>
+                            id="dobulkaction"
+                            name="form.button.BulkAction"
+                            type="submit"
+                            value="Apply"
+                            i18n:attributes="value label_apply;"
+                            i18n:translate="label_apply"
+                    >Apply</button>
                   </div>
                 </tal:bulk>
 
                 <div class="flex-grow-1">
                   <div class="row row-cols-lg-auto g-3 align-items-center justify-content-end"
-                    tal:condition="view/moderation_multiple_state_enabled">
+                       tal:condition="view/moderation_multiple_state_enabled"
+                  >
                     <label i18n:translate="filter_by_state">Filter by state:</label>
                     <div>
                       <input class="form-check-input"
-                        type="radio"
-                        id="all"
-                        name="review_state"
-                        value="all"
-                        tal:attributes="checked python:request.review_state=='all'" />
+                             id="all"
+                             name="review_state"
+                             type="radio"
+                             value="all"
+                             tal:attributes="
+                               checked python:request.review_state=='all';
+                             "
+                      />
                       <label class="form-check-label"
-                        for="all"
-                        i18n:translate="">all</label>
+                             for="all"
+                             i18n:translate=""
+                      >all</label>
                     </div>
                     <tal:states tal:repeat="review_state python:['pending', 'published', 'rejected', 'spam']">
                       <div>
                         <input class="form-check-input"
-                          type="radio"
-                          name="review_state"
-                          tal:attributes="
-                                value review_state;
-                                id review_state;
-                                checked python:request.review_state==review_state" />
+                               name="review_state"
+                               type="radio"
+                               tal:attributes="
+                                 value review_state;
+                                 id review_state;
+                                 checked python:request.review_state==review_state;
+                               "
+                        />
                         <label class="form-check-label"
-                          tal:attributes="for review_state">
+                               tal:attributes="
+                                 for review_state;
+                               "
+                        >
                           <span tal:content="python:translationhelper.translate_comment_review_state(review_state)">review_state</span>
                         </label>
                       </div>
                     </tal:states>
                   </div>
                 </div>
 
 
               </div>
               <table class="table table-bordered table-striped">
                 <thead>
                   <tr tal:condition="items">
-                    <th scope="col"
-                      class="nosort">
+                    <th class="nosort"
+                        scope="col"
+                    >
                       <input name="check_all"
-                        type="checkbox"
-                        value="0" />
+                             type="checkbox"
+                             value="0"
+                      />
                     </th>
-                    <th scope="col"
-                      class="nosort"
-                      i18n:translate="heading_commenter">Commenter</th>
-                    <th scope="col"
-                      class="nosort"
-                      i18n:translate="heading_date">Date</th>
-                    <th scope="col"
-                      class="nosort"
-                      i18n:translate="heading_in_reponse_to">In Response To</th>
-                    <th scope="col"
-                      class="nosort"
-                      i18n:translate="heading_comment">Comment</th>
-                    <th scope="col"
-                      class="nosort"
-                      i18n:translate="heading_changedby">Last Action</th>
+                    <th class="nosort"
+                        scope="col"
+                        i18n:translate="heading_commenter"
+                    >Commenter</th>
+                    <th class="nosort"
+                        scope="col"
+                        i18n:translate="heading_date"
+                    >Date</th>
+                    <th class="nosort"
+                        scope="col"
+                        i18n:translate="heading_in_reponse_to"
+                    >In Response To</th>
+                    <th class="nosort"
+                        scope="col"
+                        i18n:translate="heading_comment"
+                    >Comment</th>
+                    <th class="nosort"
+                        scope="col"
+                        i18n:translate="heading_changedby"
+                    >Last Action</th>
                   </tr>
                 </thead>
                 <tbody>
-                  <tal:block repeat="item batch"
-                    tal:condition="items">
+                  <tal:block tal:condition="items"
+                             repeat="item batch"
+                  >
                     <tr class="commentrow"
-                      tal:define="even repeat/item/even;
-                                          item_obj item/getObject;
-                                          email item_obj/author_email;
-                                          item_url item/getURL;"
-                      tal:attributes="class python: even and 'odd' or 'even'">
+                        tal:define="
+                          even repeat/item/even;
+                          item_obj item/getObject;
+                          email item_obj/author_email;
+                          item_url item/getURL;
+                        "
+                        tal:attributes="
+                          class python: even and 'odd' or 'even';
+                        "
+                    >
                       <td class="notDraggable">
-                        <input type="checkbox"
-                          class="noborder"
-                          name="paths:list"
-                          id="#"
-                          value="#"
-                          tal:attributes="value   item/getPath;
-                                                         id      string:cb_${item/id};
-                                                         checked item/checked|nothing;
-                                                         alt     string:Select ${item/Title};
-                                                         title   string:Select ${item/Title}" />
-                        <input type="hidden"
-                          name="selected_obj_paths:list"
-                          value="#"
-                          tal:attributes="value item/getURL" />
+                        <input class="noborder"
+                               id="#"
+                               name="paths:list"
+                               type="checkbox"
+                               value="#"
+                               tal:attributes="
+                                 value   item/getPath;
+                                 id      string:cb_${item/id};
+                                 checked item/checked|nothing;
+                                 alt     string:Select ${item/Title};
+                                 title   string:Select ${item/Title};
+                               "
+                        />
+                        <input name="selected_obj_paths:list"
+                               type="hidden"
+                               value="#"
+                               tal:attributes="
+                                 value item/getURL;
+                               "
+                        />
                       </td>
                       <td>
                         <span tal:content="python:item.author_name or item.Creator">Name</span>
                         <tal:email tal:condition="email">
                           <br />
-                          <a tal:attributes="href string:mailto:$email;"
-                            tal:content="email">Email
+                          <a tal:content="email"
+                             tal:attributes="
+                               href string:mailto:$email;
+                             "
+                          >Email
                           </a>
                         </tal:email>
                       </td>
                       <td style="white-space: nowrap;"
-                        tal:content="python:toLocalizedTime(item.created, long_format=1)" />
+                          tal:content="python:toLocalizedTime(item.created, long_format=1)"
+                      ></td>
                       <td>
-                        <a tal:attributes="href item_url"
-                          target="_blank"
-                          tal:content="item/in_response_to" />
+                        <a target="_blank"
+                           tal:content="item/in_response_to"
+                           tal:attributes="
+                             href item_url;
+                           "
+                        ></a>
                       </td>
-                      <td tal:attributes="class  python:colorclass(item.review_state)">
+                      <td tal:attributes="
+                            class  python:colorclass(item.review_state);
+                          ">
                         <div class="mb-2">
-                          <span tal:replace="item/Description" />
-                          <a href=""
-                            tal:attributes="href string:$item_url/getText"
-                            tal:condition="python:item.Description.endswith('[...]')"
-                            i18n:translate="label_show_full_comment_text"
-                            class="show-full-comment-text">show full comment text</a>
+                          <span tal:replace="item/Description"></span>
+                          <a class="show-full-comment-text"
+                             href=""
+                             tal:condition="python:item.Description.endswith('[...]')"
+                             tal:attributes="
+                               href string:$item_url/getText;
+                             "
+                             i18n:translate="label_show_full_comment_text"
+                          >show full comment text</a>
                         </div>
                         <div class="actions input-group-addon">
-                          <input type="hidden"
-                            name="selected_obj_paths:list"
-                            value="#"
-                            tal:attributes="value item/getURL" />
+                          <input name="selected_obj_paths:list"
+                                 type="hidden"
+                                 value="#"
+                                 tal:attributes="
+                                   value item/getURL;
+                                 "
+                          />
                           <!-- delete -->
-                          <button id=""
-                            class="destructive comment-delete-button btn btn-sm btn-danger"
-                            type="submit"
-                            value="Delete"
-                            name="form.button.moderation.DeleteComment"
-                            i18n:attributes="value label_delete;"
-                            tal:attributes="id item/id"
-                            i18n:translate="label_delete">Delete</button>
+                          <button class="destructive comment-delete-button btn btn-sm btn-danger"
+                                  id=""
+                                  name="form.button.moderation.DeleteComment"
+                                  type="submit"
+                                  value="Delete"
+                                  tal:attributes="
+                                    id item/id;
+                                  "
+                                  i18n:attributes="value label_delete;"
+                                  i18n:translate="label_delete"
+                          >Delete</button>
                           <!-- edit -->
                           <a class="pat-plone-modal context btn btn-sm btn-primary"
-                            href="#"
-                            i18n:translate="label_edit"
-                            tal:attributes="href python:item_url+'/@@edit-comment?review_state=' + item.review_state">Edit</a>
+                             href="#"
+                             tal:attributes="
+                               href python:item_url+'/@@edit-comment?review_state=' + item.review_state;
+                             "
+                             i18n:translate="label_edit"
+                          >Edit</a>
 
                           <!-- workflow actions -->
                           <tal:transitions tal:define="
-                                            transitions python:view.allowed_transitions(item_obj)">
-                            <button name="form.button.moderation.TransmitComment"
-                              tal:repeat="transition transitions"
-                              class="context btn btn-sm btn-primary"
-                              type="submit"
-                              value="Label"
-                              tal:content="python:translationhelper.translate(transition['title'])"
-                              tal:attributes="id string:${item/id}_${transition/id};
-                                                    data-transition transition/id;
-                                                    value python:translationhelper.translate(transition['title']);
-                                                    style python:transition['id']=='publish' and 'background-color: #5cb85c;; border-color: #4cae4c;;' or '';
-                                                    ">Label</button>
+                                             transitions python:view.allowed_transitions(item_obj);
+                                           ">
+                            <button class="context btn btn-sm btn-primary"
+                                    name="form.button.moderation.TransmitComment"
+                                    type="submit"
+                                    value="Label"
+                                    tal:repeat="transition transitions"
+                                    tal:content="python:translationhelper.translate(transition['title'])"
+                                    tal:attributes="
+                                      id string:${item/id}_${transition/id};
+                                      data-transition transition/id;
+                                      value python:translationhelper.translate(transition['title']);
+                                      style python:transition['id']=='publish' and 'background-color: #5cb85c;; border-color: #4cae4c;;' or '';
+                                    "
+                            >Label</button>
                           </tal:transitions>
                         </div>
                       </td>
                       <td>
                         <span class="last-history-entry"
-                          tal:attributes="data-href string:$item_url/@@contenthistorypopup"
-                          i18n:translate="">
+                              tal:attributes="
+                                data-href string:$item_url/@@contenthistorypopup;
+                              "
+                              i18n:translate=""
+                        >
                                       last history entry
                         </span>
                       </td>
                     </tr>
                   </tal:block>
                 </tbody>
               </table>
             </div>
-            <div metal:use-macro="here/batch_macros/macros/navigation" />
+            <div metal:use-macro="here/batch_macros/macros/navigation"></div>
           </fieldset>
         </form>
 
 
       </tal:main-macro>
     </metal:main>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/browser/moderation.py` & `plone.app.discussion-4.0.1/plone/app/discussion/browser/moderation.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         return False
 
     @property
     def moderation_multiple_state_enabled(self):
         """Return true if a 'review multiple state workflow' is enabled on
         'Discussion Item' content type.
 
-        A 'review multipe state workflow' is characterized by implementing
+        A 'review multiple state workflow' is characterized by implementing
         a 'rejected' workflow state and a 'spam' workflow state.
         """
         workflows = self.workflowTool.getChainForPortalType("Discussion Item")
         if workflows:
             comment_workflow = self.workflowTool[workflows[0]]
             if "spam" in comment_workflow.states:
                 return True
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/browser/traversal.py` & `plone.app.discussion-4.0.1/plone/app/discussion/browser/traversal.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     """
 
     def __init__(self, context, request=None):
         self.context = context
         self.request = request
 
     def traverse(self, name, ignore):
-
         if name == "default":
             name = ""
 
         conversation = queryAdapter(self.context, IConversation, name=name)
         if conversation is None:
             raise TraversalError(name)  # pragma: no cover
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/browser/validator.py` & `plone.app.discussion-4.0.1/plone/app/discussion/browser/validator.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/comment.py` & `plone.app.discussion-4.0.1/plone/app/discussion/comment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """The default comment class and factory.
 """
 from AccessControl import ClassSecurityInfo
 from AccessControl.SecurityManagement import getSecurityManager
 from Acquisition import aq_base
 from Acquisition import aq_parent
 from Acquisition import Implicit
-from datetime import datetime
+from datetime import timezone
 from OFS.owner import Owned
 from OFS.role import RoleManager
 from OFS.Traversable import Traversable
 from persistent import Persistent
 from plone.app.discussion import _
 from plone.app.discussion.events import CommentAddedEvent
 from plone.app.discussion.events import CommentModifiedEvent
 from plone.app.discussion.events import CommentRemovedEvent
 from plone.app.discussion.events import ReplyAddedEvent
 from plone.app.discussion.events import ReplyModifiedEvent
 from plone.app.discussion.events import ReplyRemovedEvent
 from plone.app.discussion.interfaces import IComment
 from plone.app.discussion.interfaces import IConversation
 from plone.app.discussion.interfaces import IDiscussionSettings
+from plone.app.event.base import localized_now
 from plone.base.interfaces.controlpanel import IMailSchema
 from plone.base.utils import safe_text
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore import permissions
 from Products.CMFCore.CMFCatalogAware import CatalogAware
 from Products.CMFCore.CMFCatalogAware import WorkflowAware
 from Products.CMFCore.DynamicType import DynamicType
@@ -115,28 +116,39 @@
     user_notification = None
 
     # Note: we want to use zope.component.createObject() to instantiate
     # comments as far as possible. comment_id and __parent__ are set via
     # IConversation.addComment().
 
     def __init__(self):
-        self.creation_date = self.modification_date = datetime.utcnow()
+        self.creation_date = self.modification_date = localized_now()
         self.mime_type = "text/plain"
 
         user = getSecurityManager().getUser()
         if user and user.getId():
             aclpath = [x for x in user.getPhysicalPath() if x]
             self._owner = (
                 aclpath,
                 user.getId(),
             )
             self.__ac_local_roles__ = {
                 user.getId(): ["Owner"],
             }
 
+    def __getattribute__(self, attr):
+        # In older versions of the add-on dates were set timezone naive.
+        # In tz aware versions, the value is stored as self._creation_date
+        if attr in ["creation_date", "modification_date"]:
+            old_date = super().__getattribute__(attr)
+            if old_date.tzinfo is None:
+                # Naive dates were always stored utc
+                return old_date.replace(tzinfo=timezone.utc)
+            return old_date
+        return super().__getattribute__(attr)
+
     @property
     def __name__(self):
         return self.comment_id and str(self.comment_id) or None
 
     @property
     def id(self):
         return self.comment_id and str(self.comment_id) or None
@@ -298,15 +310,15 @@
     ):
         return
 
     # This method is also called for sublocations of moved objects. We
     # therefore can't assume that event.object == obj and event.
     # {old,new}{Parent,Name} may refer to the actually moved object further up
     # in the object hierarchy. The object is already moved at this point. so
-    # obj.getPhysicalPath retruns the new path get the part of the path that
+    # obj.getPhysicalPath returns the new path get the part of the path that
     # was moved.
     moved_path = obj.getPhysicalPath()[len(event.newParent.getPhysicalPath()) + 1 :]
 
     # Remove comments at the old location from catalog
     catalog = getToolByName(obj, "portal_catalog")
     old_path = "/".join(
         event.oldParent.getPhysicalPath() + (event.oldName,) + moved_path,
@@ -338,15 +350,15 @@
 
     # Check if user notification is enabled
     registry = queryUtility(IRegistry)
     settings = registry.forInterface(IDiscussionSettings, check=False)
     if not settings.user_notification_enabled:
         return
 
-    # Get informations that are necessary to send an email
+    # Get information that are necessary to send an email
     mail_host = getToolByName(obj, "MailHost")
     registry = getUtility(IRegistry)
     mail_settings = registry.forInterface(IMailSchema, prefix="plone")
     sender = mail_settings.email_from_address
 
     # Check if a sender address is available
     if not sender:
@@ -414,15 +426,15 @@
     """
     # Check if moderator notification is enabled
     registry = queryUtility(IRegistry)
     settings = registry.forInterface(IDiscussionSettings, check=False)
     if not settings.moderator_notification_enabled:
         return
 
-    # Get informations that are necessary to send an email
+    # Get information that are necessary to send an email
     mail_host = getToolByName(obj, "MailHost")
     registry = getUtility(IRegistry)
     mail_settings = registry.forInterface(IMailSchema, prefix="plone")
     sender = mail_settings.email_from_address
 
     if settings.moderator_email:
         mto = settings.moderator_email
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/configure.zcml` & `plone.app.discussion-4.0.1/plone/app/discussion/configure.zcml`

 * *Files 16% similar despite different names*

```diff
@@ -1,102 +1,161 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
+    xmlns:five="http://namespaces.zope.org/five"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     xmlns:i18n="http://namespaces.zope.org/i18n"
     xmlns:zcml="http://namespaces.zope.org/zcml"
-    xmlns:five="http://namespaces.zope.org/five"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
-    <five:registerPackage package="." />
+  <five:registerPackage package="." />
 
-    <include package="plone.indexer" />
-    <include package="plone.app.registry" />
-    <include package="plone.resource" />
-    <include package="plone.uuid" />
-    <include package="plone.app.uuid" />
-
-    <include file="contentrules.zcml" />
-    <include file="permissions.zcml" />
-    <include file="notifications.zcml" />
-    <include file="subscribers.zcml" />
-    <include file="upgrades.zcml" />
-
-    <!-- load captch before browser -->
-    <configure zcml:condition="installed plone.formwidget.captcha">
-      <include package="plone.formwidget.captcha" />
-    </configure>
-    <configure zcml:condition="installed plone.formwidget.recaptcha">
-      <include package="plone.formwidget.recaptcha" />
-    </configure>
-    <configure zcml:condition="installed collective.z3cform.norobots">
-      <include package="collective.z3cform.norobots" />
-    </configure>
-    <include package=".browser" />
-
-    <!-- Register the installation GenericSetup extension profile -->
-    <genericsetup:registerProfile
-        name="default"
-        title="Plone Discussions"
-        description="Commenting infrastructure for Plone"
-        directory="profiles/default"
-        provides="Products.GenericSetup.interfaces.EXTENSION"
-        for="plone.base.interfaces.IPloneSiteRoot"
+  <include package="plone.indexer" />
+  <include package="plone.app.registry" />
+  <include package="plone.resource" />
+  <include package="plone.uuid" />
+  <include package="plone.app.uuid" />
+
+  <include file="contentrules.zcml" />
+  <include file="permissions.zcml" />
+  <include file="notifications.zcml" />
+  <include file="subscribers.zcml" />
+  <include file="upgrades.zcml" />
+
+  <!-- load captch before browser -->
+  <configure zcml:condition="installed plone.formwidget.captcha">
+    <include package="plone.formwidget.captcha" />
+  </configure>
+  <configure zcml:condition="installed plone.formwidget.recaptcha">
+    <include package="plone.formwidget.recaptcha" />
+  </configure>
+  <configure zcml:condition="installed collective.z3cform.norobots">
+    <include package="collective.z3cform.norobots" />
+  </configure>
+  <include package=".browser" />
+
+  <!-- Register the installation GenericSetup extension profile -->
+  <genericsetup:registerProfile
+      name="default"
+      title="Plone Discussions"
+      description="Commenting infrastructure for Plone"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      for="plone.base.interfaces.IPloneSiteRoot"
+      directory="profiles/default"
+      />
+  <!-- For upgrade steps see upgrades.zcml. -->
+
+  <!-- Comments -->
+
+  <class class=".comment.Comment">
+    <require
+        permission="zope2.View"
+        interface=".interfaces.IComment"
         />
-    <!-- For upgrade steps see upgrades.zcml. -->
-
-    <!-- Comments -->
+    <require
+        permission="zope2.View"
+        attributes="Title Creator getId getText"
+        />
+  </class>
 
-    <class class=".comment.Comment">
-        <require interface=".interfaces.IComment" permission="zope2.View" />
-        <require attributes="Title Creator getId getText" permission="zope2.View" />
-    </class>
-
-    <class class=".comment.Comment">
-        <implements interface="plone.uuid.interfaces.IAttributeUUID" />
-    </class>
-
-    <utility
-        component=".comment.CommentFactory"
-        name="plone.Comment"
+  <class class=".comment.Comment">
+    <implements interface="plone.uuid.interfaces.IAttributeUUID" />
+  </class>
+
+  <utility
+      name="plone.Comment"
+      component=".comment.CommentFactory"
+      />
+
+  <!-- Conversations -->
+
+  <class class=".conversation.Conversation">
+    <require
+        permission="zope2.View"
+        interface=".interfaces.IConversation"
         />
+  </class>
+
+  <adapter factory=".conversation.conversationAdapterFactory" />
 
-    <!-- Conversations -->
+  <adapter factory=".conversation.ConversationReplies" />
+  <adapter factory=".conversation.CommentReplies" />
 
-    <class class=".conversation.Conversation">
-        <require interface=".interfaces.IConversation" permission="zope2.View" />
-    </class>
-
-    <adapter factory=".conversation.conversationAdapterFactory" />
-
-    <adapter factory=".conversation.ConversationReplies" />
-    <adapter factory=".conversation.CommentReplies" />
-
-    <!-- Captcha Vocabulary -->
-    <utility component=".vocabularies.captcha_vocabulary"
-             name="plone.app.discussion.vocabularies.CaptchaVocabulary"
-             provides="zope.schema.interfaces.IVocabularyFactory" />
-
-    <!-- Text Transform Vocabulary -->
-    <utility component=".vocabularies.text_transform_vocabulary"
-             name="plone.app.discussion.vocabularies.TextTransformVocabulary"
-             provides="zope.schema.interfaces.IVocabularyFactory" />
-
-    <!-- Conversation indexes -->
-    <adapter name="total_comments" factory=".catalog.total_comments" />
-    <adapter name="last_comment_date" factory=".catalog.last_comment_date" />
-    <adapter name="commentators" factory=".catalog.commentators" />
-    <adapter name="in_response_to" factory=".catalog.in_response_to" />
-
-    <!-- Comment indexes -->
-    <adapter name="UID" factory=".catalog.UID" />
-    <adapter name="Title" factory=".catalog.title" />
-    <adapter name="Creator" factory=".catalog.creator" />
-    <adapter name="Description" factory=".catalog.description" />
-    <adapter name="SearchableText" factory=".catalog.searchable_text" />
-    <adapter name="effective" factory=".catalog.effective" />
-    <adapter name="created" factory=".catalog.created" />
-    <adapter name="modified" factory=".catalog.modified" />
-    <adapter name="total_comments" factory=".catalog.comments_total_comments" />
-    <adapter name="last_comment_date" factory=".catalog.comments_last_comment_date" />
-    <adapter name="commentators" factory=".catalog.comments_commentators" />
+  <!-- Captcha Vocabulary -->
+  <utility
+      provides="zope.schema.interfaces.IVocabularyFactory"
+      name="plone.app.discussion.vocabularies.CaptchaVocabulary"
+      component=".vocabularies.captcha_vocabulary"
+      />
+
+  <!-- Text Transform Vocabulary -->
+  <utility
+      provides="zope.schema.interfaces.IVocabularyFactory"
+      name="plone.app.discussion.vocabularies.TextTransformVocabulary"
+      component=".vocabularies.text_transform_vocabulary"
+      />
+
+  <!-- Conversation indexes -->
+  <adapter
+      factory=".catalog.total_comments"
+      name="total_comments"
+      />
+  <adapter
+      factory=".catalog.last_comment_date"
+      name="last_comment_date"
+      />
+  <adapter
+      factory=".catalog.commentators"
+      name="commentators"
+      />
+  <adapter
+      factory=".catalog.in_response_to"
+      name="in_response_to"
+      />
+
+  <!-- Comment indexes -->
+  <adapter
+      factory=".catalog.UID"
+      name="UID"
+      />
+  <adapter
+      factory=".catalog.title"
+      name="Title"
+      />
+  <adapter
+      factory=".catalog.creator"
+      name="Creator"
+      />
+  <adapter
+      factory=".catalog.description"
+      name="Description"
+      />
+  <adapter
+      factory=".catalog.searchable_text"
+      name="SearchableText"
+      />
+  <adapter
+      factory=".catalog.effective"
+      name="effective"
+      />
+  <adapter
+      factory=".catalog.created"
+      name="created"
+      />
+  <adapter
+      factory=".catalog.modified"
+      name="modified"
+      />
+  <adapter
+      factory=".catalog.comments_total_comments"
+      name="total_comments"
+      />
+  <adapter
+      factory=".catalog.comments_last_comment_date"
+      name="last_comment_date"
+      />
+  <adapter
+      factory=".catalog.comments_commentators"
+      name="commentators"
+      />
 
 </configure>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/contentrules.py` & `plone.app.discussion-4.0.1/plone/app/discussion/contentrules.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/contentrules.zcml` & `plone.app.discussion-4.0.1/plone/app/discussion/contentrules.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -1,120 +1,121 @@
 <configure
-  xmlns="http://namespaces.zope.org/zope"
-  xmlns:zcml="http://namespaces.zope.org/zcml">
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    >
 
   <!-- Content Rules events -->
   <configure zcml:condition="installed plone.contentrules">
 
     <interface
-      interface="plone.app.discussion.interfaces.ICommentAddedEvent"
-      type="plone.contentrules.rule.interfaces.IRuleEventType"
-      name="Comment added"
-      />
-
-    <interface
-      interface="plone.app.discussion.interfaces.ICommentRemovedEvent"
-      type="plone.contentrules.rule.interfaces.IRuleEventType"
-      name="Comment removed"
-      />
-
-    <interface
-      interface="plone.app.discussion.interfaces.IReplyAddedEvent"
-      type="plone.contentrules.rule.interfaces.IRuleEventType"
-      name="Comment reply added"
-      />
-
-    <interface
-      interface="plone.app.discussion.interfaces.IReplyRemovedEvent"
-      type="plone.contentrules.rule.interfaces.IRuleEventType"
-      name="Comment reply removed"
-      />
-      
-    <interface
-      interface="plone.app.discussion.interfaces.ICommentPublishedEvent"
-      type="plone.contentrules.rule.interfaces.IRuleEventType"
-      name="Notify user on comment publication"
-      />
-      
-    <interface
-      interface="plone.app.discussion.interfaces.ICommentDeletedEvent"
-      type="plone.contentrules.rule.interfaces.IRuleEventType"
-      name="Notify user on comment delete"
-      />
+        interface="plone.app.discussion.interfaces.ICommentAddedEvent"
+        type="plone.contentrules.rule.interfaces.IRuleEventType"
+        name="Comment added"
+        />
+
+    <interface
+        interface="plone.app.discussion.interfaces.ICommentRemovedEvent"
+        type="plone.contentrules.rule.interfaces.IRuleEventType"
+        name="Comment removed"
+        />
+
+    <interface
+        interface="plone.app.discussion.interfaces.IReplyAddedEvent"
+        type="plone.contentrules.rule.interfaces.IRuleEventType"
+        name="Comment reply added"
+        />
+
+    <interface
+        interface="plone.app.discussion.interfaces.IReplyRemovedEvent"
+        type="plone.contentrules.rule.interfaces.IRuleEventType"
+        name="Comment reply removed"
+        />
+
+    <interface
+        interface="plone.app.discussion.interfaces.ICommentPublishedEvent"
+        type="plone.contentrules.rule.interfaces.IRuleEventType"
+        name="Notify user on comment publication"
+        />
+
+    <interface
+        interface="plone.app.discussion.interfaces.ICommentDeletedEvent"
+        type="plone.contentrules.rule.interfaces.IRuleEventType"
+        name="Notify user on comment delete"
+        />
 
   </configure>
 
 
   <!-- Content rules subscribers -->
   <configure zcml:condition="installed plone.app.contentrules">
 
     <subscriber
-      for="plone.app.discussion.interfaces.ICommentAddedEvent"
-      handler=".contentrules.execute_comment"
-      />
+        for="plone.app.discussion.interfaces.ICommentAddedEvent"
+        handler=".contentrules.execute_comment"
+        />
 
     <subscriber
-      for="plone.app.discussion.interfaces.ICommentRemovedEvent"
-      handler=".contentrules.execute_comment"
-      />
+        for="plone.app.discussion.interfaces.ICommentRemovedEvent"
+        handler=".contentrules.execute_comment"
+        />
 
     <subscriber
-      for="plone.app.discussion.interfaces.IReplyAddedEvent"
-      handler=".contentrules.execute_comment"
-      />
+        for="plone.app.discussion.interfaces.IReplyAddedEvent"
+        handler=".contentrules.execute_comment"
+        />
 
     <subscriber
-      for="plone.app.discussion.interfaces.IReplyRemovedEvent"
-      handler=".contentrules.execute_comment"
-      />
-      
+        for="plone.app.discussion.interfaces.IReplyRemovedEvent"
+        handler=".contentrules.execute_comment"
+        />
+
     <subscriber
-      for="plone.app.discussion.interfaces.ICommentDeletedEvent"
-      handler=".contentrules.execute_comment"
-      />
-      
+        for="plone.app.discussion.interfaces.ICommentDeletedEvent"
+        handler=".contentrules.execute_comment"
+        />
+
     <subscriber
-      for="plone.app.discussion.interfaces.ICommentPublishedEvent"
-      handler=".contentrules.execute_comment"
-      />
+        for="plone.app.discussion.interfaces.ICommentPublishedEvent"
+        handler=".contentrules.execute_comment"
+        />
 
   </configure>
 
   <!-- Content rules strings -->
   <configure zcml:condition="installed plone.stringinterp">
     <adapter
-      for="zope.interface.Interface"
-      provides="plone.stringinterp.interfaces.IStringSubstitution"
-      factory=".contentrules.Id"
-      name="comment_id"
-      />
+        factory=".contentrules.Id"
+        provides="plone.stringinterp.interfaces.IStringSubstitution"
+        for="zope.interface.Interface"
+        name="comment_id"
+        />
 
     <adapter
-      for="zope.interface.Interface"
-      provides="plone.stringinterp.interfaces.IStringSubstitution"
-      factory=".contentrules.Text"
-      name="comment_text"
-      />
+        factory=".contentrules.Text"
+        provides="plone.stringinterp.interfaces.IStringSubstitution"
+        for="zope.interface.Interface"
+        name="comment_text"
+        />
 
     <adapter
-      for="zope.interface.Interface"
-      provides="plone.stringinterp.interfaces.IStringSubstitution"
-      factory=".contentrules.AuthorUserName"
-      name="comment_user_id"
-      />
+        factory=".contentrules.AuthorUserName"
+        provides="plone.stringinterp.interfaces.IStringSubstitution"
+        for="zope.interface.Interface"
+        name="comment_user_id"
+        />
 
     <adapter
-      for="zope.interface.Interface"
-      provides="plone.stringinterp.interfaces.IStringSubstitution"
-      factory=".contentrules.AuthorFullName"
-      name="comment_user_fullname"
-      />
+        factory=".contentrules.AuthorFullName"
+        provides="plone.stringinterp.interfaces.IStringSubstitution"
+        for="zope.interface.Interface"
+        name="comment_user_fullname"
+        />
 
     <adapter
-      for="zope.interface.Interface"
-      provides="plone.stringinterp.interfaces.IStringSubstitution"
-      factory=".contentrules.AuthorEmail"
-      name="comment_user_email"
-      />
+        factory=".contentrules.AuthorEmail"
+        provides="plone.stringinterp.interfaces.IStringSubstitution"
+        for="zope.interface.Interface"
+        name="comment_user_email"
+        />
   </configure>
 
 </configure>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/conversation.py` & `plone.app.discussion-4.0.1/plone/app/discussion/conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,14 @@
                         yield from recurse(child_id, d + 1)
 
         # Find top level threads
         comments = self._children.get(root, None)
         if comments is not None:
             count = 0
             for comment_id in comments.keys(min=start):
-
                 # Abort if we have found all the threads we want
                 count += 1
                 if size and count > size:
                     return
 
                 # Let the closure recurse
                 yield from recurse(comment_id)
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/design.txt` & `plone.app.discussion-4.0.1/plone/app/discussion/design.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/events.py` & `plone.app.discussion-4.0.1/plone/app/discussion/events.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/interfaces.py` & `plone.app.discussion-4.0.1/plone/app/discussion/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/permissions.zcml` & `plone.app.discussion-4.0.1/plone/app/discussion/permissions.zcml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
-    <!-- custom permissions are defined here -->
+  <!-- custom permissions are defined here -->
 
-    <permission
-        id="plone.app.discussion.ViewComments"
-        title="View comments"
-        />
-
-    <permission
-        id="plone.app.discussion.ReviewComments"
-        title="Review comments"
-        />
-
-    <permission
-        id="plone.app.discussion.EditComments"
-        title="Edit comments"
-        />
-
-    <permission
-        id="plone.app.discussion.DeleteOwnComments"
-        title="Delete own comments"
-        />
-
-    <permission
-        id="plone.app.discussion.DeleteComments"
-        title="Delete comments"
-        />
+  <permission
+      id="plone.app.discussion.ViewComments"
+      title="View comments"
+      />
+
+  <permission
+      id="plone.app.discussion.ReviewComments"
+      title="Review comments"
+      />
+
+  <permission
+      id="plone.app.discussion.EditComments"
+      title="Edit comments"
+      />
+
+  <permission
+      id="plone.app.discussion.DeleteOwnComments"
+      title="Delete own comments"
+      />
+
+  <permission
+      id="plone.app.discussion.DeleteComments"
+      title="Delete comments"
+      />
 
 </configure>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/actions.xml` & `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/actions.xml`

 * *Files 17% similar despite different names*

#### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/actions.xml` & `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/actions.xml`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="portal_actions">
-  <object name="user" meta_type="CMF Action Category">
-    <object name="review-comments" meta_type="CMF Action" i18n:domain="plone" insert-before="logout">
+  <object meta_type="CMF Action Category" name="user">
+    <object insert-before="logout" meta_type="CMF Action" name="review-comments" i18n:domain="plone">
       <property name="title" i18n:translate="">Moderate comments</property>
       <property name="description" i18n:translate=""/>
       <property name="url_expr">string:${globals_view/navigationRootUrl}/@@moderate-comments</property>
       <property name="icon_expr">string:${globals_view/navigationRootUrl}/discussionitem_icon.png</property>
       <property name="available_expr">portal/@@moderate-comments-enabled|nothing</property>
       <property name="permissions">
         <element value="Review comments"/>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/controlpanel.xml` & `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/controlpanel.xml`

 * *Files 15% similar despite different names*

#### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/controlpanel.xml` & `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/controlpanel.xml`

```diff
@@ -1,6 +1,6 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="portal_controlpanel" i18n:domain="plone" purge="False">
-  <configlet title="Discussion" action_id="discussion" appId="plone.app.discussion" category="plone-general" condition_expr="" icon_expr="string:chat-square-dots" url_expr="string:${portal_url}/@@discussion-controlpanel" visible="True" i18n:attributes="title">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="portal_controlpanel" purge="False" i18n:domain="plone">
+  <configlet action_id="discussion" appId="plone.app.discussion" category="plone-general" condition_expr="" icon_expr="string:chat-square-dots" title="Discussion" url_expr="string:${portal_url}/@@discussion-controlpanel" visible="True" i18n:attributes="title">
     <permission>Manage portal</permission>
   </configlet>
 </object>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/portal_atct.xml` & `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/portal_atct.xml`

 * *Files 21% similar despite different names*

#### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/portal_atct.xml` & `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/portal_atct.xml`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <atcttool xmlns:i18n="http://xml.zope.org/namespaces/i18n">
   <topic_indexes i18n:domain="plone">
-    <index name="commentators" friendlyName="Commentators" description="Users who have commented on the item" enabled="True" i18n:attributes="description; friendlyName">
+    <index description="Users who have commented on the item" enabled="True" friendlyName="Commentators" name="commentators" i18n:attributes="description; friendlyName">
       <criteria>ATCurrentAuthorCriterion</criteria>
       <criteria>ATSimpleStringCriterion</criteria>
       <criteria>ATListCriterion</criteria>
     </index>
-    <index name="total_comments" enabled="False" friendlyName="Total number of comments" description="Total number of comments on this item." i18n:attributes="description; friendlyName">
+    <index description="Total number of comments on this item." enabled="False" friendlyName="Total number of comments" name="total_comments" i18n:attributes="description; friendlyName">
       <criteria>ATSimpleIntCriterion</criteria>
     </index>
   </topic_indexes>
   <topic_metadata i18n:domain="plone">
-    <metadata name="total_comments" enabled="True" friendlyName="Total number of comments" description="Total number of comments on this item."/>
+    <metadata description="Total number of comments on this item." enabled="True" friendlyName="Total number of comments" name="total_comments"/>
   </topic_metadata>
 </atcttool>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/types/Discussion_Item.xml` & `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/types/Discussion_Item.xml`

 * *Files 18% similar despite different names*

#### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/types/Discussion_Item.xml` & `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/types/Discussion_Item.xml`

```diff
@@ -1,19 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="Discussion Item" meta_type="Factory-based Type Information" i18n:domain="plone">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Factory-based Type Information" name="Discussion Item" i18n:domain="plone">
   <property name="title" i18n:translate="">Comment</property>
   <property name="description" i18n:translate="">Comments added to a content item.</property>
   <property name="content_icon">discussionitem_icon.png</property>
   <property name="content_meta_type">Discussion Item</property>
   <property name="product"/>
   <property name="factory">plone.Comment</property>
   <property name="immediate_view"/>
   <property name="global_allow">False</property>
   <property name="filter_content_types">True</property>
   <property name="allowed_content_types"/>
   <property name="allow_discussion">True</property>
   <alias from="(Default)" to="@@view"/>
   <alias from="view" to="@@view"/>
-  <action title="View" action_id="view" category="object" condition_expr="" url_expr="string:${object_url}/@@view" visible="True">
+  <action action_id="view" category="object" condition_expr="" title="View" url_expr="string:${object_url}/@@view" visible="True">
     <permission value="View"/>
   </action>
 </object>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/definition.xml` & `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/definition.xml`

 * *Files 26% similar despite different names*

#### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/definition.xml` & `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/comment_one_state_workflow/definition.xml`

```diff
@@ -1,57 +1,57 @@
 <?xml version="1.0" encoding="utf-8"?>
-<dc-workflow workflow_id="comment_one_state_workflow" title="Single State Workflow" description="- Essentially a workflow with no transitions, but has a Published state, so portlets and applications that expect that state will continue to work." state_variable="review_state" initial_state="published" manager_bypass="False">
+<dc-workflow description="- Essentially a workflow with no transitions, but has a Published state, so portlets and applications that expect that state will continue to work." initial_state="published" manager_bypass="False" state_variable="review_state" title="Single State Workflow" workflow_id="comment_one_state_workflow">
   <permission>Access contents information</permission>
   <permission>Modify portal content</permission>
   <permission>View</permission>
   <state state_id="published" title="Published">
     <description>Visible to everyone, editable by the owner.</description>
-    <permission-map name="Access contents information" acquired="False">
+    <permission-map acquired="False" name="Access contents information">
       <permission-role>Anonymous</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
+    <permission-map acquired="False" name="Modify portal content">
       <permission-role>Manager</permission-role>
       <permission-role>Owner</permission-role>
       <permission-role>Editor</permission-role>
       <permission-role>Site Administrator</permission-role>
     </permission-map>
-    <permission-map name="View" acquired="True"/>
+    <permission-map acquired="True" name="View"/>
   </state>
-  <variable variable_id="action" for_catalog="False" for_status="True" update_always="True">
+  <variable for_catalog="False" for_status="True" update_always="True" variable_id="action">
     <description>Previous transition</description>
     <default>
       <expression>transition/getId|nothing</expression>
     </default>
     <guard/>
   </variable>
-  <variable variable_id="actor" for_catalog="False" for_status="True" update_always="True">
+  <variable for_catalog="False" for_status="True" update_always="True" variable_id="actor">
     <description>The ID of the user who performed the previous transition</description>
     <default>
       <expression>user/getId</expression>
     </default>
     <guard/>
   </variable>
-  <variable variable_id="comments" for_catalog="False" for_status="True" update_always="True">
+  <variable for_catalog="False" for_status="True" update_always="True" variable_id="comments">
     <description>Comment about the last transition</description>
     <default>
       <expression>python:state_change.kwargs.get('comment', '')</expression>
     </default>
     <guard/>
   </variable>
-  <variable variable_id="review_history" for_catalog="False" for_status="False" update_always="False">
+  <variable for_catalog="False" for_status="False" update_always="False" variable_id="review_history">
     <description>Provides access to workflow history</description>
     <default>
       <expression>state_change/getHistory</expression>
     </default>
     <guard>
       <guard-permission>Request review</guard-permission>
       <guard-permission>Review portal content</guard-permission>
     </guard>
   </variable>
-  <variable variable_id="time" for_catalog="False" for_status="True" update_always="True">
+  <variable for_catalog="False" for_status="True" update_always="True" variable_id="time">
     <description>When the previous transition was performed</description>
     <default>
       <expression>state_change/getDateTime</expression>
     </default>
     <guard/>
   </variable>
 </dc-workflow>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/workflows/comment_review_workflow/definition.xml` & `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/comment_review_workflow/definition.xml`

 * *Files 16% similar despite different names*

#### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/profiles/default/workflows/comment_review_workflow/definition.xml` & `plone.app.discussion-4.0.1/plone/app/discussion/profiles/default/workflows/comment_review_workflow/definition.xml`

```diff
@@ -1,120 +1,120 @@
 <?xml version="1.0" encoding="utf-8"?>
-<dc-workflow xmlns:i18n="http://xml.zope.org/namespaces/i18n" i18n:domain="plone" workflow_id="comment_review_workflow" title="Comment Review Workflow" description="A simple review workflow for comments" state_variable="review_state" initial_state="pending" i18n:attributes="title; description">
+<dc-workflow xmlns:i18n="http://xml.zope.org/namespaces/i18n" description="A simple review workflow for comments" initial_state="pending" state_variable="review_state" title="Comment Review Workflow" workflow_id="comment_review_workflow" i18n:attributes="title; description" i18n:domain="plone">
   <permission>Access contents information</permission>
   <permission>Modify portal content</permission>
   <permission>Reply to item</permission>
   <permission>View</permission>
   <state state_id="pending" title="Pending">
     <description>Submitted, pending review.</description>
     <exit-transition transition_id="mark_as_spam"/>
     <exit-transition transition_id="publish"/>
     <exit-transition transition_id="reject"/>
-    <permission-map name="Access contents information" acquired="False">
+    <permission-map acquired="False" name="Access contents information">
       <permission-role>Manager</permission-role>
       <permission-role>Owner</permission-role>
       <permission-role>Reviewer</permission-role>
       <permission-role>Site Administrator</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
+    <permission-map acquired="False" name="Modify portal content">
       <permission-role>Manager</permission-role>
       <permission-role>Owner</permission-role>
       <permission-role>Reviewer</permission-role>
       <permission-role>Site Administrator</permission-role>
     </permission-map>
-    <permission-map name="Reply to item" acquired="False"/>
-    <permission-map name="View" acquired="False">
+    <permission-map acquired="False" name="Reply to item"/>
+    <permission-map acquired="False" name="View">
       <permission-role>Manager</permission-role>
       <permission-role>Owner</permission-role>
       <permission-role>Reviewer</permission-role>
       <permission-role>Site Administrator</permission-role>
     </permission-map>
   </state>
   <state state_id="published" title="Published">
     <description>Visible to everyone, non-editable.</description>
     <exit-transition transition_id="mark_as_spam"/>
     <exit-transition transition_id="recall"/>
     <exit-transition transition_id="reject"/>
-    <permission-map name="Access contents information" acquired="True"/>
-    <permission-map name="Modify portal content" acquired="False">
+    <permission-map acquired="True" name="Access contents information"/>
+    <permission-map acquired="False" name="Modify portal content">
       <permission-role>Manager</permission-role>
       <permission-role>Site Administrator</permission-role>
     </permission-map>
-    <permission-map name="Reply to item" acquired="True"/>
-    <permission-map name="View" acquired="True"/>
+    <permission-map acquired="True" name="Reply to item"/>
+    <permission-map acquired="True" name="View"/>
   </state>
   <state state_id="rejected" title="Rejected">
     <exit-transition transition_id="mark_as_spam"/>
     <exit-transition transition_id="publish"/>
     <exit-transition transition_id="recall"/>
   </state>
   <state state_id="spam" title="Spam">
     <exit-transition transition_id="publish"/>
     <exit-transition transition_id="recall"/>
     <exit-transition transition_id="reject"/>
   </state>
-  <transition transition_id="mark_as_spam" title="Mark as spam" new_state="spam" trigger="USER" before_script="" after_script="">
+  <transition after_script="" before_script="" new_state="spam" title="Mark as spam" transition_id="mark_as_spam" trigger="USER">
     <description>Spam comments are invisible to other users.</description>
-    <action url="%(content_url)s/content_status_modify?workflow_action=mark_as_spam" category="workflow" icon="">Spam</action>
+    <action category="workflow" icon="" url="%(content_url)s/content_status_modify?workflow_action=mark_as_spam">Spam</action>
     <guard>
       <guard-permission>Review comments</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="publish" title="Reviewer approves content" new_state="published" trigger="USER" before_script="" after_script="">
+  <transition after_script="" before_script="" new_state="published" title="Reviewer approves content" transition_id="publish" trigger="USER">
     <description>Approving the comment makes it visible to other users.</description>
-    <action url="%(content_url)s/content_status_modify?workflow_action=publish" category="workflow" icon="">Approve</action>
+    <action category="workflow" icon="" url="%(content_url)s/content_status_modify?workflow_action=publish">Approve</action>
     <guard>
       <guard-permission>Review comments</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="recall" title="Reviewer recalls comment back to pending state" new_state="pending" trigger="USER" before_script="" after_script="">
-    <action url="%(content_url)s/content_status_modify?workflow_action=recall" category="workflow" icon="">Recall</action>
+  <transition after_script="" before_script="" new_state="pending" title="Reviewer recalls comment back to pending state" transition_id="recall" trigger="USER">
+    <action category="workflow" icon="" url="%(content_url)s/content_status_modify?workflow_action=recall">Recall</action>
     <guard>
       <guard-permission>Review comments</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="reject" title="Reviewer rejects comment" new_state="rejected" trigger="USER" before_script="" after_script="">
+  <transition after_script="" before_script="" new_state="rejected" title="Reviewer rejects comment" transition_id="reject" trigger="USER">
     <description>Rejected comments are invisible to other users.</description>
-    <action url="%(content_url)s/content_status_modify?workflow_action=reject" category="workflow" icon="">Reject</action>
+    <action category="workflow" icon="" url="%(content_url)s/content_status_modify?workflow_action=reject">Reject</action>
     <guard>
       <guard-permission>Review comments</guard-permission>
     </guard>
   </transition>
-  <variable variable_id="action" for_catalog="False" for_status="True" update_always="True">
+  <variable for_catalog="False" for_status="True" update_always="True" variable_id="action">
     <description>Previous transition</description>
     <default>
       <expression>transition/getId|nothing</expression>
     </default>
     <guard/>
   </variable>
-  <variable variable_id="actor" for_catalog="False" for_status="True" update_always="True">
+  <variable for_catalog="False" for_status="True" update_always="True" variable_id="actor">
     <description>The ID of the user who performed the previous transition</description>
     <default>
       <expression>user/getUserName</expression>
     </default>
     <guard/>
   </variable>
-  <variable variable_id="comments" for_catalog="False" for_status="True" update_always="True">
+  <variable for_catalog="False" for_status="True" update_always="True" variable_id="comments">
     <description>Comment about the last transition</description>
     <default>
       <expression>python:state_change.kwargs.get('comment', '')</expression>
     </default>
     <guard/>
   </variable>
-  <variable variable_id="review_history" for_catalog="False" for_status="False" update_always="False">
+  <variable for_catalog="False" for_status="False" update_always="False" variable_id="review_history">
     <description>Provides access to workflow history</description>
     <default>
       <expression>state_change/getHistory</expression>
     </default>
     <guard>
       <guard-permission>Request review</guard-permission>
       <guard-permission>Review portal content</guard-permission>
     </guard>
   </variable>
-  <variable variable_id="time" for_catalog="False" for_status="True" update_always="True">
+  <variable for_catalog="False" for_status="True" update_always="True" variable_id="time">
     <description>When the previous transition was performed</description>
     <default>
       <expression>state_change/getDateTime</expression>
     </default>
     <guard/>
   </variable>
 </dc-workflow>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/subscribers.zcml` & `plone.app.discussion-4.0.1/plone/app/discussion/subscribers.zcml`

 * *Files 5% similar despite different names*

```diff
@@ -1,84 +1,85 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:zcml="http://namespaces.zope.org/zcml"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
-    <subscriber
-        for="plone.app.discussion.interfaces.IComment
-             zope.lifecycleevent.interfaces.IObjectAddedEvent"
-        handler=".comment.notify_workflow"
-        />
-
-    <subscriber
-        for="plone.app.discussion.interfaces.IComment
-             zope.lifecycleevent.interfaces.IObjectModifiedEvent"
-        handler=".comment.notify_comment_modified"
-        />
-
-    <subscriber
-        for="plone.app.discussion.interfaces.IComment
-             zope.lifecycleevent.interfaces.IObjectAddedEvent"
-        handler=".comment.notify_content_object"
-        />
-
-    <subscriber
-        for="plone.app.discussion.interfaces.IComment
-             zope.lifecycleevent.interfaces.IObjectAddedEvent"
-        handler=".comment.notify_comment_added"
-        />
-
-    <subscriber
-        for="plone.app.discussion.interfaces.IComment
-             zope.lifecycleevent.interfaces.IObjectRemovedEvent"
-        handler=".comment.notify_content_object"
-        />
-
-    <subscriber
-        for="plone.app.discussion.interfaces.IComment
-             zope.lifecycleevent.interfaces.IObjectRemovedEvent"
-        handler=".comment.notify_comment_removed"
-        />
-
-    <subscriber
-        for="plone.app.discussion.interfaces.IComment
-             zope.lifecycleevent.interfaces.IObjectAddedEvent"
-        handler=".subscribers.index_object"
-        />
-
-    <subscriber
-        for="plone.app.discussion.interfaces.IComment
-             zope.lifecycleevent.interfaces.IObjectModifiedEvent"
-        handler=".subscribers.index_object"
-        />
-
-    <subscriber
-        for="plone.app.discussion.interfaces.IComment
-             zope.lifecycleevent.interfaces.IObjectRemovedEvent"
-        handler=".subscribers.unindex_object"
-        />
-
-    <subscriber
-        for="Products.CMFCore.interfaces.IContentish
-             zope.lifecycleevent.interfaces.IObjectRemovedEvent"
-        handler=".comment.notify_content_object_deleted"
-        />
-
-    <subscriber
-        for="Products.CMFCore.interfaces.IContentish
-             zope.lifecycleevent.interfaces.IObjectMovedEvent"
-        handler=".comment.notify_content_object_moved"
-        />
-
-    <!-- Control panel event subscribers -->
-
-    <subscriber
-        for="plone.base.interfaces.events.IConfigurationChangedEvent"
-        handler=".browser.controlpanel.notify_configuration_changed"
-        />
-
-    <subscriber
-        for="plone.registry.interfaces.IRecordModifiedEvent"
-        handler=".browser.controlpanel.notify_configuration_changed"
-        />
+  <subscriber
+      for="plone.app.discussion.interfaces.IComment
+           zope.lifecycleevent.interfaces.IObjectAddedEvent"
+      handler=".comment.notify_workflow"
+      />
+
+  <subscriber
+      for="plone.app.discussion.interfaces.IComment
+           zope.lifecycleevent.interfaces.IObjectModifiedEvent"
+      handler=".comment.notify_comment_modified"
+      />
+
+  <subscriber
+      for="plone.app.discussion.interfaces.IComment
+           zope.lifecycleevent.interfaces.IObjectAddedEvent"
+      handler=".comment.notify_content_object"
+      />
+
+  <subscriber
+      for="plone.app.discussion.interfaces.IComment
+           zope.lifecycleevent.interfaces.IObjectAddedEvent"
+      handler=".comment.notify_comment_added"
+      />
+
+  <subscriber
+      for="plone.app.discussion.interfaces.IComment
+           zope.lifecycleevent.interfaces.IObjectRemovedEvent"
+      handler=".comment.notify_content_object"
+      />
+
+  <subscriber
+      for="plone.app.discussion.interfaces.IComment
+           zope.lifecycleevent.interfaces.IObjectRemovedEvent"
+      handler=".comment.notify_comment_removed"
+      />
+
+  <subscriber
+      for="plone.app.discussion.interfaces.IComment
+           zope.lifecycleevent.interfaces.IObjectAddedEvent"
+      handler=".subscribers.index_object"
+      />
+
+  <subscriber
+      for="plone.app.discussion.interfaces.IComment
+           zope.lifecycleevent.interfaces.IObjectModifiedEvent"
+      handler=".subscribers.index_object"
+      />
+
+  <subscriber
+      for="plone.app.discussion.interfaces.IComment
+           zope.lifecycleevent.interfaces.IObjectRemovedEvent"
+      handler=".subscribers.unindex_object"
+      />
+
+  <subscriber
+      for="Products.CMFCore.interfaces.IContentish
+           zope.lifecycleevent.interfaces.IObjectRemovedEvent"
+      handler=".comment.notify_content_object_deleted"
+      />
+
+  <subscriber
+      for="Products.CMFCore.interfaces.IContentish
+           zope.lifecycleevent.interfaces.IObjectMovedEvent"
+      handler=".comment.notify_content_object_moved"
+      />
+
+  <!-- Control panel event subscribers -->
+
+  <subscriber
+      for="plone.base.interfaces.events.IConfigurationChangedEvent"
+      handler=".browser.controlpanel.notify_configuration_changed"
+      />
+
+  <subscriber
+      for="plone.registry.interfaces.IRecordModifiedEvent"
+      handler=".browser.controlpanel.notify_configuration_changed"
+      />
 
 </configure>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/testing.py` & `plone.app.discussion-4.0.1/plone/app/discussion/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
     COLLECTION_TYPE = "Collection"
 except ImportError:
     COLLECTION_TYPE = "Topic"
 
 
 class PloneAppDiscussion(PloneSandboxLayer):
-
     defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     USER_NAME = "johndoe"
     USER_PASSWORD = TEST_USER_PASSWORD
     MEMBER_NAME = "janedoe"
     MEMBER_PASSWORD = TEST_USER_PASSWORD
     USER_WITH_FULLNAME_NAME = "jim"
@@ -97,15 +96,14 @@
             id="doc1",
             title="Document 1",
             type_name="Document",
         )
 
 
 class PloneAppDiscussionRobot(PloneAppDiscussion):
-
     defaultBases = (
         PLONE_APP_CONTENTTYPES_FIXTURE,
         REMOTE_LIBRARY_ROBOT_TESTING,
     )
 
     def setUpPloneSite(self, portal):
         registry = queryUtility(IRegistry)
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/collection-integration-test.txt` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/collection-integration-test.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/functional_test_comment_review_workflow.txt` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/functional_test_comment_review_workflow.txt`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/functional_test_comments.txt` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/functional_test_comments.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 This is a functional test for the plone.app.discussion comments viewlet.
 
 We use zope.testbrowser to simulate browser interaction in order to show how
 the plone.app.discussion commenting works.
 
 
-Setting up and loggin in
-------------------------
+Setting up and log in
+---------------------
 
 First we have to set up some things and login.
 
     >>> app = layer['app']
     >>> from plone.testing.z2 import Browser
     >>> from plone.app.testing import SITE_OWNER_PASSWORD
     >>> from plone.app.testing import TEST_USER_PASSWORD
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 ====================== plone.app.discussion ====================== This is a
 functional test for the plone.app.discussion comments viewlet. We use
 zope.testbrowser to simulate browser interaction in order to show how the
-plone.app.discussion commenting works. Setting up and loggin in ---------------
---------- First we have to set up some things and login. >>> app = layer['app']
->>> from plone.testing.z2 import Browser >>> from plone.app.testing import
+plone.app.discussion commenting works. Setting up and log in ------------------
+--- First we have to set up some things and login. >>> app = layer['app'] >>>
+from plone.testing.z2 import Browser >>> from plone.app.testing import
 SITE_OWNER_PASSWORD >>> from plone.app.testing import TEST_USER_PASSWORD >>>
 browser = Browser(app) >>> browser.handleErrors = False >>> browser.addHeader
 ('Authorization', f'Basic admin:{SITE_OWNER_PASSWORD}') >>> portal = layer
 ['portal'] >>> portal_url = 'http://nohost/plone' By default, only HTTP error
 codes (e.g. 500 Server Side Error) are shown when an error occurs on the
 server. To see more details, set handleErrors to False: >>>
 browser.handleErrors = False We also keep another testbrowser handy for testing
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/robot/test_discussion.robot` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/robot/test_discussion.robot`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/robot/test_moderation.robot` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/robot/test_moderation.robot`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_catalog.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_catalog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Test the plone.app.discussion catalog indexes
 """
 from datetime import datetime
+from datetime import timezone
 from plone.app.discussion.interfaces import IConversation
 from plone.app.discussion.testing import (  # noqa
     PLONE_APP_DISCUSSION_INTEGRATION_TESTING,
 )
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from Products.CMFCore.utils import getToolByName
@@ -14,15 +15,14 @@
 from zope.lifecycleevent import ObjectModifiedEvent
 
 import transaction
 import unittest
 
 
 class CatalogSetupTest(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
 
     def test_catalog_installed(self):
         self.assertTrue(
@@ -46,15 +46,14 @@
             self.portal.portal_atct.getIndex("total_comments")
             self.portal.portal_atct.getMetadata("total_comments")
         except AttributeError:
             self.fail()
 
 
 class ConversationCatalogTest(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
 
         workflow = self.portal.portal_workflow
@@ -63,16 +62,20 @@
         self.catalog = getToolByName(self.portal, "portal_catalog")
         conversation = IConversation(self.portal.doc1)
         comment1 = createObject("plone.Comment")
         comment1.title = "Comment 1"
         comment1.text = "Comment text"
         comment1.creator = "jim"
         comment1.author_username = "Jim"
-        comment1.creation_date = datetime(2006, 9, 17, 14, 18, 12)
-        comment1.modification_date = datetime(2006, 9, 17, 14, 18, 12)
+        comment1.creation_date = datetime(2006, 9, 17, 14, 18, 12).astimezone(
+            timezone.utc
+        )
+        comment1.modification_date = datetime(2006, 9, 17, 14, 18, 12).astimezone(
+            timezone.utc
+        )
 
         new_comment1_id = conversation.addComment(comment1)
         self.comment_id = new_comment1_id
 
         brains = self.catalog.searchResults(
             dict(
                 path={
@@ -111,23 +114,27 @@
         doc1_brain = brains[0]
         self.assertEqual(doc1_brain.total_comments, 2)
 
     def test_last_comment_date(self):
         self.assertTrue("last_comment_date" in self.doc1_brain)
         self.assertEqual(
             self.doc1_brain.last_comment_date,
-            datetime(2006, 9, 17, 14, 18, 12),
+            datetime(2006, 9, 17, 14, 18, 12).astimezone(timezone.utc),
         )
 
         # Add another comment and check if last comment date is updated.
         comment2 = createObject("plone.Comment")
         comment2.title = "Comment 2"
         comment2.text = "Comment text"
-        comment2.creation_date = datetime(2009, 9, 17, 14, 18, 12)
-        comment2.modification_date = datetime(2009, 9, 17, 14, 18, 12)
+        comment2.creation_date = datetime(2009, 9, 17, 14, 18, 12).astimezone(
+            timezone.utc
+        )
+        comment2.modification_date = datetime(2009, 9, 17, 14, 18, 12).astimezone(
+            timezone.utc
+        )
         new_comment2_id = self.conversation.addComment(comment2)
 
         comment2 = self.portal.doc1.restrictedTraverse(
             f"++conversation++default/{new_comment2_id}",
         )
         comment2.reindexObject()
         brains = self.catalog.searchResults(
@@ -137,15 +144,15 @@
                 },
                 portal_type="Document",
             ),
         )
         doc1_brain = brains[0]
         self.assertEqual(
             doc1_brain.last_comment_date,
-            datetime(2009, 9, 17, 14, 18, 12),
+            datetime(2009, 9, 17, 14, 18, 12).astimezone(timezone.utc),
         )
 
         # Remove the comment again
         del self.conversation[new_comment2_id]
 
         brains = self.catalog.searchResults(
             dict(
@@ -154,15 +161,15 @@
                 },
                 portal_type="Document",
             ),
         )
         doc1_brain = brains[0]
         self.assertEqual(
             doc1_brain.last_comment_date,
-            datetime(2006, 9, 17, 14, 18, 12),
+            datetime(2006, 9, 17, 14, 18, 12).astimezone(timezone.utc),
         )
 
         # remove all comments
         del self.conversation[self.new_comment1_id]
         brains = self.catalog.searchResults(
             dict(
                 path={
@@ -258,15 +265,14 @@
             ),
         )
         doc1_brain = brains[0]
         self.assertEqual(doc1_brain.commentators, ())
 
 
 class CommentCatalogTest(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.catalog = getToolByName(self.portal, "portal_catalog")
 
@@ -505,15 +511,14 @@
         self.assertEqual(comment_brain.Title, "Jim on Document 1")
         self.assertEqual(
             comment_brain.getPath(),
             "/plone/doc1/++conversation++default/" + str(self.comment_id),
         )
 
     def test_clear_and_rebuild_catalog_for_nested_comments(self):
-
         # Create a nested comment structure:
         #
         # Conversation
         # +- Comment 1
         #    +- Comment 1_1
         #    |  +- Comment 1_1_1
         #    +- Comment 1_2
@@ -562,15 +567,14 @@
         # Check if comments are still there
         brains = self.catalog.searchResults({"portal_type": "Discussion Item"})
         self.assertTrue(brains)
         self.assertEqual(len(brains), 6)
 
 
 class NoConversationCatalogTest(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
 
         self.catalog = getToolByName(self.portal, "portal_catalog")
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_comment.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_comment.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         ):
             line = " " + line
         lines.append(line)
     return "".join(lines).strip()
 
 
 class CommentTest(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
 
         workflow = self.portal.portal_workflow
@@ -59,15 +58,15 @@
         if utc_to_local_diff < 60:
             logger.warning(
                 "Your computer is living in a timezone where local "
                 "time equals utc time. Some potential errors can "
                 "get hidden by that"
             )
         comment1 = createObject("plone.Comment")
-        local_utc = datetime.datetime.utcnow()
+        local_utc = datetime.datetime.now().astimezone(datetime.timezone.utc)
         for date in (comment1.creation_date, comment1.modification_date):
             difference = abs(date - local_utc)
             difference = difference.seconds
             # We hope that between comment1 and local_utc happen less than
             # 10 seconds
             self.assertFalse(difference // 10)
 
@@ -360,15 +359,14 @@
         # is called directly
         view = View(comment, self.request)
         View.__call__(view)
         self.assertEqual(self.request.response.status, 302)
 
 
 class RepliesTest(unittest.TestCase):
-
     # test the IReplies adapter on a comment
 
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_comments_viewlet.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_comments_viewlet.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         return 1
 
     def read(self, *args):
         return self.data
 
 
 class TestCommentForm(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.portal.invokeFactory("Folder", "test-folder")
@@ -471,15 +470,14 @@
             commentForm.handleComment,
             commentForm,
             "foo",
         )
 
 
 class TestCommentsViewlet(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.portal.invokeFactory("Folder", "test-folder")
@@ -512,15 +510,17 @@
     def test_can_review(self):
         # Portal owner has 'can review' permission
         self.assertTrue(self.viewlet.can_review())
         logout()
         # Anonymous has no 'can review' permission
         self.assertFalse(self.viewlet.can_review())
         # The reviewer role has the 'Review comments' permission
-        self.portal.acl_users._doAddUser("reviewer", TEST_USER_PASSWORD, ["Reviewer"], [])
+        self.portal.acl_users._doAddUser(
+            "reviewer", TEST_USER_PASSWORD, ["Reviewer"], []
+        )
         login(self.portal, "reviewer")
         self.assertTrue(self.viewlet.can_review())
 
     def test_can_manage(self):
         """We keep this method for backward compatibility. This method has been
         removed in version 1.0b9 and added again in 1.0b11 because we don't
         do API changes in beta releases.
@@ -540,15 +540,14 @@
         self.assertFalse(self.viewlet.is_discussion_allowed())
         # Enable discussion
         self.portal.doc1.allow_discussion = True
         # Test if discussion has been enabled
         self.assertTrue(self.viewlet.is_discussion_allowed())
 
     def test_comment_transform_message(self):
-
         # Default transform is plain/text and comment moderation disabled
         self.assertTrue(self.viewlet.comment_transform_message())
         self.assertEqual(
             self.viewlet.comment_transform_message(),
             "You can add a comment by filling out the form below. Plain "
             + "text formatting.",
         )
@@ -653,15 +652,14 @@
             "http://nohost/plone/author/test-user",
         )
 
     def test_get_commenter_home_url_is_none(self):
         self.assertFalse(self.viewlet.get_commenter_home_url())
 
     def test_get_commenter_portrait(self):
-
         # Add a user with a member image
         self.membershipTool.addMember("jim", "Jim", ["Member"], [])
         self.memberdata._setPortrait(
             Image(
                 id="jim",
                 file=DummyFile(),
                 title="",
@@ -692,25 +690,23 @@
         # Check if the correct member image URL is returned
         self.assertEqual(
             portrait_url,
             "http://nohost/plone/portal_memberdata/portraits/jim",
         )
 
     def test_get_commenter_portrait_is_none(self):
-
         self.assertTrue(
             self.viewlet.get_commenter_portrait()
             in (
                 "defaultUser.png",
                 "defaultUser.gif",
             ),
         )
 
     def test_get_commenter_portrait_without_userimage(self):
-
         # Create a user without a user image
         self.membershipTool.addMember("jim", "Jim", ["Member"], [])
 
         # Add a conversation with a comment
         conversation = IConversation(self.portal.doc1)
         comment = createObject("plone.Comment")
         comment.text = "Comment text"
@@ -766,15 +762,15 @@
             "http://nohost/plone/login_form?came_from=http%3A//nohost",
         )
 
     def test_format_time(self):
         python_time = datetime(2009, 2, 1, 23, 32, 3, 57)
         # Python Time must be utc time. There seems to be no too simple way
         # to tell datetime to be of utc time.
-        # therefor, we convert the time to seconds since epoch, which seems
+        # therefore, we convert the time to seconds since epoch, which seems
         # to assume, that the datetime was given in local time, and does the
         # correction to the seconds since epoch. Then time.gmtime returns
         # a correct utc time that can be used to make datetime set the utc
         # time of the local time given above. That way, the time for the
         # example below is correct within each time zone, independent of DST
         python_time = datetime(*time.gmtime(time.mktime(python_time.timetuple()))[:7])
         localized_time = self.viewlet.format_time(python_time)
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_contentrules.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_contentrules.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_controlpanel.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_controlpanel.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from zope.component import getMultiAdapter
 from zope.component import queryUtility
 
 import unittest
 
 
 class RegistryTest(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.registry = Registry()
         self.registry.registerInterface(IDiscussionSettings)
@@ -148,15 +147,14 @@
     #
     #    self.assertTrue('user_notification_enabled' in IDiscussionSettings)
     #    self.assertEqual(self.registry['plone.app.discussion.interfaces.' +
     #        'IDiscussionSettings.user_notification_enabled'], False)
 
 
 class ConfigurationChangedSubscriberTest(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         registry = queryUtility(IRegistry)
         self.settings = registry.forInterface(IDiscussionSettings, check=False)
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_conversation.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_conversation.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,37 +4,45 @@
 from ..interfaces import IDiscussionSettings
 from ..interfaces import IReplies
 from ..testing import PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 from Acquisition import aq_base
 from Acquisition import aq_parent
 from datetime import datetime
 from datetime import timedelta
+from datetime import timezone
+from dateutil import tz
+from plone.app.event.base import default_timezone
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.vocabularies.types import BAD_TYPES
 from plone.dexterity.interfaces import IDexterityContent
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
 from zope import interface
 from zope.annotation.interfaces import IAnnotations
 from zope.component import createObject
+from zope.component import getUtility
 from zope.component import queryUtility
 
 import unittest
 
 
 class ConversationTest(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         interface.alsoProvides(self.portal.REQUEST, IDiscussionLayer)
 
+        # Set the portal timezone to something non-utc
+        reg_key = "plone.portal_timezone"
+        registry = getUtility(IRegistry)
+        registry[reg_key] = "America/Los_Angeles"
+
         self.typetool = self.portal.portal_types
         self.portal_discussion = getToolByName(
             self.portal,
             "portal_discussion",
             None,
         )
         # Allow discussion
@@ -66,16 +74,52 @@
             aq_base(conversation),
         )
         self.assertEqual(new_id, comment.comment_id)
         self.assertEqual(len(list(conversation.getComments())), 1)
         self.assertEqual(len(tuple(conversation.getThreads())), 1)
         self.assertEqual(conversation.total_comments(), 1)
         self.assertTrue(
-            conversation.last_comment_date - datetime.utcnow() < timedelta(seconds=1),
+            datetime.now().astimezone(tz.gettz(default_timezone()))
+            - conversation.last_comment_date
+            >= timedelta(seconds=0)
+            <= timedelta(seconds=1),
+        )
+
+    def test_timezone_naive_comment(self):
+        # Create a conversation. In this case we doesn't assign it to an
+        # object, as we just want to check the Conversation object API.
+        conversation = IConversation(self.portal.doc1)
+
+        # Add a comment. Note: in real life, we always create comments via the
+        # factory to allow different factories to be swapped in
+        comment = createObject("plone.Comment")
+        comment.text = "Comment text"
+
+        conversation.addComment(comment)
+
+        # Check that comments have the correct portal timezones
+        self.assertTrue(comment.creation_date.tzinfo, tz.gettz("America/Los_Angeles"))
+        self.assertTrue(
+            comment.modification_date.tzinfo, tz.gettz("America/Los_Angeles")
+        )
+
+        # Remove the timezone from the comment dates
+        comment.creation_date = datetime.utcnow()
+        comment.modification_date = datetime.utcnow()
+
+        # Check that the timezone naive date is converted to UTC
+        # See https://github.com/plone/plone.app.discussion/pull/204
+        self.assertTrue(
+            datetime.utcnow().replace(tzinfo=timezone.utc)
+            - conversation.last_comment_date
+            >= timedelta(seconds=0)
+            <= timedelta(seconds=1),
         )
+        self.assertTrue(comment.creation_date.tzinfo, timezone.utc)
+        self.assertTrue(comment.modification_date.tzinfo, timezone.utc)
 
     def test_private_comment(self):
         conversation = IConversation(self.portal.doc1)
 
         comment = createObject("plone.Comment")
         comment.author_username = "nobody"
         conversation.addComment(comment)
@@ -210,15 +254,14 @@
         portal_types = getToolByName(self.portal, "portal_types")
         document_fti = getattr(portal_types, "Document")
         document_fti.manage_changeProperties(allow_discussion=True)
 
         self.assertEqual(conversation.enabled(), True)
 
     def test_disable_commenting_globally(self):
-
         # Create a conversation.
         conversation = self.portal.doc1.restrictedTraverse("@@conversation_view")
 
         # We have to allow discussion on Document content type, since
         # otherwise allow_discussion will always return False
         portal_types = getToolByName(self.portal, "portal_types")
         document_fti = getattr(portal_types, "Document")
@@ -236,15 +279,14 @@
         self.assertEqual(conversation.enabled(), False)
 
         # Enable discussion again
         settings.globally_enabled = True
         self.assertEqual(conversation.enabled(), True)
 
     def test_allow_discussion_for_news_items(self):
-
         self.typetool.constructContent("News Item", self.portal, "newsitem")
         newsitem = self.portal.newsitem
         conversation = newsitem.restrictedTraverse("@@conversation_view")
 
         # We have to allow discussion on Document content type, since
         # otherwise allow_discussion will always return False
         portal_types = getToolByName(self.portal, "portal_types")
@@ -263,15 +305,14 @@
         self.assertEqual(conversation.enabled(), False)
 
         # Enable discussion again
         settings.globally_enabled = True
         self.assertEqual(conversation.enabled(), True)
 
     def test_disable_commenting_for_content_type(self):
-
         # Create a conversation.
         conversation = self.portal.doc1.restrictedTraverse(
             "@@conversation_view",
         )
 
         # The Document content type is disabled by default
         self.assertEqual(conversation.enabled(), False)
@@ -484,73 +525,84 @@
 
         # Add a three comments that are at least one day old
         # Note: in real life, we always create
         # comments via the factory to allow different factories to be
         # swapped in
         comment1 = createObject("plone.Comment")
         comment1.text = "Comment text"
-        comment1.creation_date = datetime.utcnow() - timedelta(4)
+        comment1.creation_date = datetime.now().astimezone(
+            tz.gettz(default_timezone())
+        ) - timedelta(4)
         conversation.addComment(comment1)
 
         comment2 = createObject("plone.Comment")
         comment2.text = "Comment text"
-        comment2.creation_date = datetime.utcnow() - timedelta(2)
+        comment2.creation_date = datetime.now().astimezone(
+            tz.gettz(default_timezone())
+        ) - timedelta(2)
         new_comment2_id = conversation.addComment(comment2)
 
         comment3 = createObject("plone.Comment")
         comment3.text = "Comment text"
-        comment3.creation_date = datetime.utcnow() - timedelta(1)
+        comment3.creation_date = datetime.now().astimezone(
+            tz.gettz(default_timezone())
+        ) - timedelta(1)
         new_comment3_id = conversation.addComment(comment3)
 
         # check if the latest comment is exactly one day old
         self.assertTrue(
             conversation.last_comment_date
-            < datetime.utcnow() - timedelta(hours=23, minutes=59, seconds=59),
+            < datetime.now().astimezone(tz.gettz(default_timezone()))
+            - timedelta(hours=23, minutes=59, seconds=59),
         )
         self.assertTrue(
             conversation.last_comment_date
-            > datetime.utcnow() - timedelta(days=1, seconds=1),
+            > datetime.now().astimezone(tz.gettz(default_timezone()))
+            - timedelta(days=1, seconds=1),
         )
 
         # remove the latest comment
         del conversation[new_comment3_id]
 
         # check if the latest comment has been updated
         # the latest comment should be exactly two days old
         self.assertTrue(
             conversation.last_comment_date
-            < datetime.utcnow() - timedelta(days=1, hours=23, minutes=59, seconds=59),
+            < datetime.now().astimezone(tz.gettz(default_timezone()))
+            - timedelta(days=1, hours=23, minutes=59, seconds=59),
         )
         self.assertTrue(
             conversation.last_comment_date
-            > datetime.utcnow() - timedelta(days=2, seconds=1),
+            > datetime.now().astimezone(tz.gettz(default_timezone()))
+            - timedelta(days=2, seconds=1),
         )
 
         # remove the latest comment again
         del conversation[new_comment2_id]
 
         # check if the latest comment has been updated
         # the latest comment should be exactly four days old
         self.assertTrue(
             conversation.last_comment_date
-            < datetime.utcnow() - timedelta(days=3, hours=23, minutes=59, seconds=59),
+            < datetime.now().astimezone(tz.gettz(default_timezone()))
+            - timedelta(days=3, hours=23, minutes=59, seconds=59),
         )
         self.assertTrue(
             conversation.last_comment_date
-            > datetime.utcnow() - timedelta(days=4, seconds=2),
+            > datetime.now().astimezone(tz.gettz(default_timezone()))
+            - timedelta(days=4, seconds=2),
         )
 
     def test_get_comments_full(self):
         pass
 
     def test_get_comments_batched(self):
         pass
 
     def test_get_threads(self):
-
         # Create a conversation. In this case we doesn't assign it to an
         # object, as we just want to check the Conversation object API.
         conversation = IConversation(self.portal.doc1)
 
         IReplies(conversation)
 
         # Create a nested comment structure:
@@ -663,15 +715,14 @@
         # Make sure no conversation has been created
         self.assertTrue(
             "plone.app.discussion:conversation" not in IAnnotations(self.portal.doc1),
         )
 
 
 class ConversationEnabledForDexterityTypesTest(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         interface.alsoProvides(
             self.portal.REQUEST,
@@ -723,15 +774,14 @@
         self._enable_discussion_on_portal_type("Document", True)
         self.portal.doc1.allow_discussion = True
         conversation = self._makeOne(self.portal.doc1)
         self.assertTrue(conversation.enabled())
 
 
 class RepliesTest(unittest.TestCase):
-
     # test the IReplies adapter on a conversation
 
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_events.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 
 class CommentEventsTest(unittest.TestCase):
     """Test custom comments events"""
 
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
-
         # Setup sandbox
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.registry = EventsRegistry
 
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.document = self.portal["doc1"]
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_functional.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_indexers.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_indexers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Test for the plone.app.discussion indexers
 """
 from .. import catalog
 from ..interfaces import IConversation
 from ..testing import PLONE_APP_DISCUSSION_INTEGRATION_TESTING  # noqa
 from datetime import datetime
 from DateTime import DateTime
+from dateutil import tz
+from plone.app.event.base import default_timezone
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.indexer.delegate import DelegatingIndexerFactory
+from plone.registry.interfaces import IRegistry
 from zope.component import createObject
+from zope.component import getUtility
 
 import unittest
 
 
 LONG_TEXT = """Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed
 diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat,
 sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum.
@@ -32,39 +36,55 @@
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
 
         workflow = self.portal.portal_workflow
         workflow.doActionFor(self.portal.doc1, "publish")
 
+        # Change the timezone to PDT to test timezones properly
+        reg_key = "plone.portal_timezone"
+        registry = getUtility(IRegistry)
+        registry[reg_key] = "America/Los_Angeles"
+        self.portal_timezone = tz.gettz(default_timezone())
+
         # Create a conversation.
         conversation = IConversation(self.portal.doc1)
 
         comment1 = createObject("plone.Comment")
         comment1.text = "Comment Text"
         comment1.creator = "jim"
         comment1.author_username = "Jim"
+        # Purposefully exclude timezone to test the conversation getter
+        # (see plone.app.discussion.comment.Comment object)
         comment1.creation_date = datetime(2006, 9, 17, 14, 18, 12)
         comment1.modification_date = datetime(2006, 9, 17, 14, 18, 12)
         self.new_id1 = conversation.addComment(comment1)
 
         comment2 = createObject("plone.Comment")
         comment2.text = "Comment Text"
         comment2.creator = "emma"
         comment2.author_username = "Emma"
-        comment2.creation_date = datetime(2007, 12, 13, 4, 18, 12)
-        comment2.modification_date = datetime(2007, 12, 13, 4, 18, 12)
+        comment2.creation_date = datetime(2007, 12, 13, 4, 18, 12).astimezone(
+            self.portal_timezone
+        )
+        comment2.modification_date = datetime(2007, 12, 13, 4, 18, 12).astimezone(
+            self.portal_timezone
+        )
         self.new_id2 = conversation.addComment(comment2)
 
         comment3 = createObject("plone.Comment")
         comment3.text = "Comment Text"
         comment3.creator = "lukas"
         comment3.author_username = "Lukas"
-        comment3.creation_date = datetime(2009, 4, 12, 11, 12, 12)
-        comment3.modification_date = datetime(2009, 4, 12, 11, 12, 12)
+        comment3.creation_date = datetime(2009, 4, 12, 11, 12, 12).astimezone(
+            self.portal_timezone
+        )
+        comment3.modification_date = datetime(2009, 4, 12, 11, 12, 12).astimezone(
+            self.portal_timezone
+        )
         self.new_id3 = conversation.addComment(comment3)
 
         self.conversation = conversation
 
     def test_conversation_total_comments(self):
         self.assertTrue(
             isinstance(
@@ -84,54 +104,66 @@
             isinstance(
                 catalog.last_comment_date,
                 DelegatingIndexerFactory,
             )
         )
         self.assertEqual(
             catalog.last_comment_date(self.portal.doc1)(),
-            datetime(2009, 4, 12, 11, 12, 12),
+            datetime(2009, 4, 12, 11, 12, 12).astimezone(self.portal_timezone),
         )
         del self.conversation[self.new_id3]
         self.assertEqual(
             catalog.last_comment_date(self.portal.doc1)(),
-            datetime(2007, 12, 13, 4, 18, 12),
+            datetime(2007, 12, 13, 4, 18, 12).astimezone(self.portal_timezone),
         )
         del self.conversation[self.new_id2]
         del self.conversation[self.new_id1]
         self.assertEqual(catalog.last_comment_date(self.portal.doc1)(), None)
 
     def test_conversation_commentators(self):
         pass
         # self.assertEqual(catalog.commentators(self.portal.doc1)(),
         #                  ('Jim', 'Emma', 'Lukas'))
         # self.assertTrue(isinstance(catalog.commentators,
         #                        DelegatingIndexerFactory))
 
 
 class CommentIndexersTest(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
 
         # Create a conversation. In this case we doesn't assign it to an
         # object, as we just want to check the Conversation object API.
         conversation = IConversation(self.portal.doc1)
 
         # Add a comment. Note: in real life, we always create comments via the
         # factory to allow different factories to be swapped in
 
+        # Set the portal timezone to something non-utc
+        reg_key = "plone.portal_timezone"
+        registry = getUtility(IRegistry)
+        registry[reg_key] = "America/Los_Angeles"
+
         comment = createObject("plone.Comment")
         comment.text = "Lorem ipsum dolor sit amet."
         comment.creator = "jim"
         comment.author_name = "Jim"
-        comment.creation_date = datetime(2006, 9, 17, 14, 18, 12)
-        comment.modification_date = datetime(2008, 3, 12, 7, 32, 52)
+
+        # Create date in PDT (ie daylight savings)
+        comment.creation_date = datetime(2006, 9, 17, 14, 18, 12).replace(
+            tzinfo=tz.gettz("America/Los_Angeles")
+        )
+
+        # Create date in PST (ie not daylight savings)
+        comment.modification_date = datetime(2008, 2, 12, 7, 32, 52).replace(
+            tzinfo=tz.gettz("America/Los_Angeles")
+        )
 
         self.comment_id = conversation.addComment(comment)
         self.comment = comment.__of__(conversation)
         self.conversation = conversation
 
     def test_title(self):
         self.assertEqual(catalog.title(self.comment)(), "Jim on Document 1")
@@ -157,23 +189,23 @@
             LONG_TEXT_CUT.replace("\n", " "),
         )
 
     def test_dates(self):
         # Test if created, modified, effective etc. are set correctly
         self.assertEqual(
             catalog.created(self.comment)(),
-            DateTime(2006, 9, 17, 14, 18, 12, "GMT"),
+            DateTime(2006, 9, 17, 14, 18, 12, "America/Los_Angeles"),
         )
         self.assertEqual(
             catalog.effective(self.comment)(),
-            DateTime(2006, 9, 17, 14, 18, 12, "GMT"),
+            DateTime(2006, 9, 17, 14, 18, 12, "America/Los_Angeles"),
         )
         self.assertEqual(
             catalog.modified(self.comment)(),
-            DateTime(2008, 3, 12, 7, 32, 52, "GMT"),
+            DateTime(2008, 2, 12, 7, 32, 52, "America/Los_Angeles"),
         )
 
     def test_searchable_text(self):
         # Test if searchable text is a concatenation of title and comment text
         self.assertEqual(
             catalog.searchable_text(self.comment)(),
             ("Lorem ipsum dolor sit amet."),
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_moderation_multiple_state_view.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_moderation_multiple_state_view.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 from ..browser.moderation import BulkActionsView
-from ..browser.moderation import CommentTransition
-from ..browser.moderation import DeleteComment
-from ..browser.moderation import View
 from ..interfaces import IConversation
-from ..interfaces import IDiscussionSettings
 from ..testing import PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
-from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
 from zope.component import createObject
-from zope.component import queryUtility
 
 import unittest
 
 
 class ModerationBulkActionsViewTest(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_moderation_view.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_moderation_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from zope.component import createObject
 from zope.component import queryUtility
 
 import unittest
 
 
 class ModerationViewTest(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
@@ -51,15 +50,14 @@
         self.wf_tool.setChainForPortalTypes(
             ("Discussion Item",), ("comment_review_workflow,")
         )
         self.assertEqual(self.view.moderation_enabled(), True)
 
 
 class ModerationBulkActionsViewTest(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
@@ -144,15 +142,14 @@
         self.assertEqual(len(self.conversation.objectIds()), 1)
         comment = next(self.conversation.getComments())
         self.assertTrue(comment)
         self.assertEqual(comment, self.comment2)
 
 
 class RedirectionTest(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         # Update settings.
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_notifications.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_notifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         msg, mto, mfrom = _mungeHeaders(
             messageText, mto, mfrom, subject, charset, msg_type, encode
         )
         self.messages.append(msg)
 
 
 class TestUserNotificationUnit(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         # Set up a mock mailhost
         self.portal._original_MailHost = self.portal.MailHost
@@ -185,15 +184,14 @@
         # new comment is added by the same user.
         self.assertEqual(len(self.mailhost.messages), 1)
         self.mailhost.reset()
         self.assertEqual(len(self.mailhost.messages), 0)
 
 
 class TestModeratorNotificationUnit(unittest.TestCase):
-
     layer = PLONE_APP_DISCUSSION_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         # Set up a mock mailhost
         self.portal._original_MailHost = self.portal.MailHost
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_robot.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tests/test_workflow.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tests/test_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,17 @@
         cid = conversation.addComment(comment)
 
         self.comment = self.folder.doc1.restrictedTraverse(
             f"++conversation++default/{cid}",
         )
 
         self.portal.acl_users._doAddUser("member", TEST_USER_PASSWORD, ["Member"], [])
-        self.portal.acl_users._doAddUser("reviewer", TEST_USER_PASSWORD, ["Reviewer"], [])
+        self.portal.acl_users._doAddUser(
+            "reviewer", TEST_USER_PASSWORD, ["Reviewer"], []
+        )
         self.portal.acl_users._doAddUser("manager", TEST_USER_PASSWORD, ["Manager"], [])
         self.portal.acl_users._doAddUser("editor", TEST_USER_PASSWORD, ["Editor"], [])
         self.portal.acl_users._doAddUser("reader", TEST_USER_PASSWORD, ["Reader"], [])
 
     def test_initial_workflow_state(self):
         """Make sure the initial workflow state of a comment is 'private'."""
         self.assertEqual(
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/tool.py` & `plone.app.discussion-4.0.1/plone/app/discussion/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from Products.CMFCore.utils import UniqueObject
 from zope import interface
 from zope.component import queryUtility
 
 
 @interface.implementer(ICommentingTool)
 class CommentingTool(UniqueObject, SimpleItem):
-
     meta_type = "plone.app.discussion tool"
     id = "portal_discussion"
 
     def reindexObject(self, object):
         # Reindex in catalog.
         catalog = getToolByName(self, "portal_catalog")
         return catalog.reindexObject(object)
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/upgrades.py` & `plone.app.discussion-4.0.1/plone/app/discussion/upgrades.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from datetime import timezone
+from plone import api
 from plone.app.discussion.interfaces import IDiscussionSettings
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
 from zope.component import getUtility
 
 import logging
 
@@ -73,7 +75,29 @@
 def add_js_to_plone_legacy(context):
     context.runImportStepFromProfile(default_profile, "plone.app.registry")
 
 
 def extend_review_workflow(context):
     """Apply changes made to review workflow."""
     upgrade_comment_workflows_retain_current_workflow(context)
+
+
+def set_timezone_on_dates(context):
+    """Ensure timezone data is stored against all creation/modified dates"""
+    pc = api.portal.get_tool("portal_catalog")
+    creations = 0
+    modifieds = 0
+    logger.info("Setting timezone information on comment dates")
+    comments = pc.search({"Type": "Comment"})
+    for cbrain in comments:
+        comment = cbrain.getObject()
+        if not comment.creation_date.tzinfo:
+            creations += 1
+            comment.creation_date = comment.creation_date.astimezone(timezone.utc)
+        if not comment.modification_date.tzinfo:
+            modifieds += 1
+            comment.modification_date = comment.modification_date.astimezone(
+                timezone.utc
+            )
+    logger.info(
+        "Updated %i creation dates and %i modification dates" % (creations, modifieds)
+    )
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/upgrades.zcml` & `plone.app.discussion-4.0.1/plone/app/discussion/upgrades.zcml`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:genericsetup="http://namespaces.zope.org/genericsetup">
+    xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
+    >
 
   <genericsetup:upgradeStep
-      source="*"
-      destination="100"
       title="Update plone.app.discussion setting registry"
       description=""
       profile="plone.app.discussion:default"
+      source="*"
+      destination="100"
       handler=".upgrades.update_registry"
       />
 
   <genericsetup:upgradeStep
       title="edit comments and delete own comments"
       description="reload registry config to enable new fields edit_comment_enabled and delete_own_comment_enabled"
+      profile="plone.app.discussion:default"
       source="100"
       destination="101"
       handler=".upgrades.update_registry"
       sortkey="1"
-      profile="plone.app.discussion:default"
       />
 
   <genericsetup:upgradeStep
       title="delete comments and delete own comments"
       description="reload rolemap config to enable new permissions 'Delete comments' and 'Delete own comments'"
+      profile="plone.app.discussion:default"
       source="101"
       destination="102"
       handler=".upgrades.update_rolemap"
       sortkey="1"
-      profile="plone.app.discussion:default"
       />
 
   <genericsetup:upgradeSteps
+      profile="plone.app.discussion:default"
       source="102"
       destination="1000"
-      profile="plone.app.discussion:default">
+      >
     <!-- Apply the update rolemap step again, to avoid missing it when
          updating from plone.app.discussion 2.2.x.  When originally
          adding this step in the 2.3.x release, we should have made a
          bigger metadata revision increase to leave some room for new
          upgrade steps in 2.2.x. -->
     <genericsetup:upgradeStep
         title="delete comments and delete own comments"
@@ -48,44 +50,62 @@
     <genericsetup:upgradeStep
         title="Update plone.app.discussion workflows"
         handler=".upgrades.upgrade_comment_workflows"
         />
   </genericsetup:upgradeSteps>
 
   <genericsetup:upgradeSteps
+      profile="plone.app.discussion:default"
       source="1000"
       destination="1001"
-      profile="plone.app.discussion:default">
+      >
     <genericsetup:upgradeStep
         title="Move comment.js into plone-legacy bundle"
         description=""
         handler=".upgrades.add_js_to_plone_legacy"
         />
   </genericsetup:upgradeSteps>
 
   <genericsetup:upgradeSteps
-    source="1001"
-    destination="1002"
-    profile="plone.app.discussion:default">
+      profile="plone.app.discussion:default"
+      source="1001"
+      destination="1002"
+      >
     <genericsetup:upgradeStep
         title="Extended review workflow with states pending, published and new: rejected and spam"
         description="Additional states allows moderator to review history of publishing and rejection"
         handler=".upgrades.extend_review_workflow"
         />
   </genericsetup:upgradeSteps>
 
   <genericsetup:upgradeSteps
+      profile="plone.app.discussion:default"
       source="1999"
       destination="2000"
-      profile="plone.app.discussion:default">
+      >
     <genericsetup:upgradeDepends
         title="Update controlpanel icon"
-        import_steps="controlpanel" />
+        import_steps="controlpanel"
+        />
     <genericsetup:upgradeDepends
         title="Add 'View comments' permission"
-        import_steps="rolemap" />
+        import_steps="rolemap"
+        />
     <genericsetup:upgradeStep
         title="Grant Site Administrator permissions on pending comments"
-        handler=".upgrades.upgrade_comment_workflows" />
+        handler=".upgrades.upgrade_comment_workflows"
+        />
+  </genericsetup:upgradeSteps>
+
+  <genericsetup:upgradeSteps
+      profile="plone.app.discussion:default"
+      source="2000"
+      destination="2001"
+      >
+    <genericsetup:upgradeStep
+        title="Set timezone on comment dates"
+        description="Ensure the timezone is set for comment dates"
+        handler=".upgrades.set_timezone_on_dates"
+        />
   </genericsetup:upgradeSteps>
 
 </configure>
```

### Comparing `plone.app.discussion-4.0.0b3/plone/app/discussion/vocabularies.py` & `plone.app.discussion-4.0.1/plone/app/discussion/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.discussion-4.0.0b3/plone.app.discussion.egg-info/PKG-INFO` & `plone.app.discussion-4.0.1/plone.app.discussion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.discussion
-Version: 4.0.0b3
+Version: 4.0.1
 Summary: Enhanced discussion support for Plone
 Home-page: https://pypi.org/project/plone.app.discussion
 Author: Timo Stollenwerk - Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: plone discussion
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
 
 
 plone.app.discussion is the commenting system used since Plone 4.1.
@@ -86,14 +88,36 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.1 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Remove translations folder,
+  for ages they are coming from p.a.locales.
+  [gforcada] (#1)
+- Update configuration files.
+  [plone devs] (#47959565)
+
+
+4.0.0 (2022-11-11)
+------------------
+
+Bug fixes:
+
+
+- Set timezones for creation and modification dates of comments [instification] (#204)
+
+
 4.0.0b3 (2022-10-11)
 --------------------
 
 Bug fixes:
 
 
 - Fix password used in tests.  [davisagli] (#203)
@@ -259,15 +283,15 @@
 
 3.4.0 (2020-04-20)
 ------------------
 
 New features:
 
 
-- Extended existing review workflow by stati ``rejected`` and ``spam``
+- Extended existing review workflow by state ``rejected`` and ``spam``
   Moderation view extended to handle four workflow states.
   [ksuess and precious input of agitator] (#164)
 
 
 Bug fixes:
 
 
@@ -817,15 +841,15 @@
   [toutpt]
 
 
 2.2.10 (2013-09-24)
 -------------------
 
 - Revert "Refactor tests to use the PLONE_APP_CONTENTTYPES_FIXTURE instead of
-  the PLONE_FIXTURE." that has been accidentially introduced into the 2.2.9
+  the PLONE_FIXTURE." that has been accidentally introduced into the 2.2.9
   release.
   [timo]
 
 
 2.2.9 (2013-09-24)
 ------------------
 
@@ -1145,15 +1169,15 @@
 - Remove one_state_workflow customizations.
   [timo]
 
 
 2.0.9 (2011-07-25)
 ------------------
 
-- Make sure the creator index always stores utf-8 encoded stings and not
+- Make sure the creator index always stores utf-8 encoded strings and not
   unicode.
   [timo]
 
 
 2.0.8 (2011-07-25)
 ------------------
```

### Comparing `plone.app.discussion-4.0.0b3/plone.app.discussion.egg-info/SOURCES.txt` & `plone.app.discussion-4.0.1/plone.app.discussion.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -68,34 +68,14 @@
 plone/app/discussion/browser/controlpanel.pt
 plone/app/discussion/browser/controlpanel.py
 plone/app/discussion/browser/conversation.py
 plone/app/discussion/browser/moderation.pt
 plone/app/discussion/browser/moderation.py
 plone/app/discussion/browser/traversal.py
 plone/app/discussion/browser/validator.py
-plone/app/discussion/i18n/plone-ca.po
-plone/app/discussion/i18n/plone-cs.po
-plone/app/discussion/i18n/plone-da.po
-plone/app/discussion/i18n/plone-de.po
-plone/app/discussion/i18n/plone-el.po
-plone/app/discussion/i18n/plone-es.po
-plone/app/discussion/i18n/plone-eu.po
-plone/app/discussion/i18n/plone-fr.po
-plone/app/discussion/i18n/plone-it.po
-plone/app/discussion/i18n/plone-ja.po
-plone/app/discussion/i18n/plone-manual.pot
-plone/app/discussion/i18n/plone-nl.po
-plone/app/discussion/i18n/plone-no.po
-plone/app/discussion/i18n/plone-pt_BR.po
-plone/app/discussion/i18n/plone-ru.po
-plone/app/discussion/i18n/plone-sk.po
-plone/app/discussion/i18n/plone-uk.po
-plone/app/discussion/i18n/plone-zh_CN.po
-plone/app/discussion/i18n/plone-zh_TW.po
-plone/app/discussion/i18n/plone.pot
 plone/app/discussion/profiles/default/actions.xml
 plone/app/discussion/profiles/default/browserlayer.xml
 plone/app/discussion/profiles/default/catalog.xml
 plone/app/discussion/profiles/default/controlpanel.xml
 plone/app/discussion/profiles/default/metadata.xml
 plone/app/discussion/profiles/default/portal_atct.xml
 plone/app/discussion/profiles/default/registry.xml
```

### Comparing `plone.app.discussion-4.0.0b3/setup.py` & `plone.app.discussion-4.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.0b3"
+version = "4.0.1"
 
 install_requires = [
+    "BTrees",
+    "Products.GenericSetup",
+    "Products.ZCatalog",
+    "Products.statusmessages",
+    "persistent",
+    "plone.api",
+    "plone.app.event",
+    "plone.dexterity",
+    "plone.registry",
+    "plone.resource",
+    "plone.uuid",
+    "zope.annotation",
     "setuptools",
     "plone.app.layout",
     "plone.app.registry",
     "plone.app.uuid",
-    "plone.app.z3cform",
     "plone.base",
     "plone.indexer",
     "plone.z3cform",
     "z3c.form>=2.3.3",
 ]
 
 setup(
@@ -30,29 +41,37 @@
         "Framework :: Zope :: 5",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="plone discussion",
     author="Timo Stollenwerk - Plone Foundation",
     author_email="plone-developers@lists.sourceforge.net",
     url="https://pypi.org/project/plone.app.discussion",
     license="GPL",
     packages=find_packages(),
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     install_requires=install_requires,
     extras_require={
         "test": [
             "plone.app.testing",
             "plone.stringinterp",
             "plone.contentrules",
             "plone.app.contentrules",
             "plone.app.contenttypes[test]",
             "plone.app.robotframework",
+            "plone.app.vocabularies",
+            "plone.testing",
+            "plone.protect",
+            "Products.MailHost",
+            "robotsuite",
+            "python-dateutil",
         ],
     },
 )
```

