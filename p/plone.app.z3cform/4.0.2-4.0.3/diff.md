# Comparing `tmp/plone.app.z3cform-4.0.2.tar.gz` & `tmp/plone.app.z3cform-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.z3cform-4.0.2.tar", last modified: Thu Mar 23 11:59:53 2023, max compression
+gzip compressed data, was "plone.app.z3cform-4.0.3.tar", last modified: Thu Apr 13 22:51:53 2023, max compression
```

## Comparing `plone.app.z3cform-4.0.2.tar` & `plone.app.z3cform-4.0.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:59:53.153957 plone.app.z3cform-4.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)    24406 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      146 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    47638 2023-03-23 11:59:53.154096 plone.app.z3cform-4.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    13825 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:59:53.133851 plone.app.z3cform-4.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      749 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:59:53.134106 plone.app.z3cform-4.0.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:59:53.136318 plone.app.z3cform-4.0.2/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:59:53.140413 plone.app.z3cform-4.0.2/plone/app/z3cform/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4254 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    18540 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/converters.py
--rw-r--r--   0 maurits    (501) staff       (20)      724 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/csrf.py
--rw-r--r--   0 maurits    (501) staff       (20)      431 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/factories.py
--rw-r--r--   0 maurits    (501) staff       (20)     2349 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/inline_validation.py
--rw-r--r--   0 maurits    (501) staff       (20)     7482 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/inline_validation.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2496 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      212 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/layout.py
--rw-r--r--   0 maurits    (501) staff       (20)      152 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/overrides.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:59:53.130371 plone.app.z3cform-4.0.2/plone/app/z3cform/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:59:53.141016 plone.app.z3cform-4.0.2/plone/app/z3cform/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      163 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)       85 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      635 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/profiles.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:59:53.149519 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1013 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/ajaxselect_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3643 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/checkbox_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      140 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/contentprovider-widget.pt
--rw-r--r--   0 maurits    (501) staff       (20)      209 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/error.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4806 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/file_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      829 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4798 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/image_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      677 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3547 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/link_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9551 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/macros.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4033 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/multi_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1861 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/object_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5486 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/orderedselect_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1448 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/password_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      650 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/radio_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/radio_input_single.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1869 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/relateditems_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1937 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/select_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      976 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/singlecheckbox.pt
--rw-r--r--   0 maurits    (501) staff       (20)      765 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/singlecheckboxbool_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1357 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4046 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/singlecheckboxbool_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1335 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/submit_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1574 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/text_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1414 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/textarea_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3703 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/textfield_widget_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1356 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/textlines_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1812 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/templates/widget.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:59:53.152127 plone.app.z3cform-4.0.2/plone/app/z3cform/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2421 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/tests/example.py
--rw-r--r--   0 maurits    (501) staff       (20)     1139 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/tests/layer.py
--rw-r--r--   0 maurits    (501) staff       (20)      907 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/tests/test_csrf.py
--rw-r--r--   0 maurits    (501) staff       (20)     4554 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1349 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/tests/test_widget.py
--rw-r--r--   0 maurits    (501) staff       (20)    66068 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/tests/test_widgets.py
--rw-r--r--   0 maurits    (501) staff       (20)      776 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/tests/testing.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2208 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/tests/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)     3393 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2739 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/views.py
--rw-r--r--   0 maurits    (501) staff       (20)    33302 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/widget.py
--rw-r--r--   0 maurits    (501) staff       (20)     8895 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/widget.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:59:53.153740 plone.app.z3cform-4.0.2/plone/app/z3cform/wysiwyg/
--rw-r--r--   0 maurits    (501) staff       (20)      919 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/wysiwyg/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      127 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/wysiwyg/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      639 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/wysiwyg/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1693 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/wysiwyg/widget.py
--rw-r--r--   0 maurits    (501) staff       (20)      601 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/wysiwyg/wysiwyg_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1048 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/plone/app/z3cform/wysiwyg/wysiwyg_input.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 11:59:53.136046 plone.app.z3cform-4.0.2/plone.app.z3cform.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    47638 2023-03-23 11:59:53.000000 plone.app.z3cform-4.0.2/plone.app.z3cform.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2876 2023-03-23 11:59:53.000000 plone.app.z3cform-4.0.2/plone.app.z3cform.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-23 11:59:53.000000 plone.app.z3cform-4.0.2/plone.app.z3cform.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-03-23 11:59:53.000000 plone.app.z3cform-4.0.2/plone.app.z3cform.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-23 11:59:53.000000 plone.app.z3cform-4.0.2/plone.app.z3cform.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      543 2023-03-23 11:59:53.000000 plone.app.z3cform-4.0.2/plone.app.z3cform.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-23 11:59:53.000000 plone.app.z3cform-4.0.2/plone.app.z3cform.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1692 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      242 2023-03-23 11:59:53.154580 plone.app.z3cform-4.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2665 2023-03-23 11:59:52.000000 plone.app.z3cform-4.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.870687 plone.app.z3cform-4.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)    24821 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    48074 2023-04-13 22:51:53.870810 plone.app.z3cform-4.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    13825 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.848336 plone.app.z3cform-4.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      749 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.848564 plone.app.z3cform-4.0.3/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.851131 plone.app.z3cform-4.0.3/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.856082 plone.app.z3cform-4.0.3/plone/app/z3cform/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4254 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    18540 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/converters.py
+-rw-r--r--   0 maurits    (501) staff       (20)      724 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/csrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)      431 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/factories.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2349 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/inline_validation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7482 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/inline_validation.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2500 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      212 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)      152 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/overrides.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.845032 plone.app.z3cform-4.0.3/plone/app/z3cform/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.856946 plone.app.z3cform-4.0.3/plone/app/z3cform/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      163 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      635 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/profiles.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.865826 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     1013 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/ajaxselect_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3643 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/checkbox_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      140 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/contentprovider-widget.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      209 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/error.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4806 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/file_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      829 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4798 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/image_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      677 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3547 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/link_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9551 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/macros.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4033 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/multi_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1861 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/object_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5486 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/orderedselect_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1448 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/password_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      650 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/radio_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/radio_input_single.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1869 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/relateditems_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1937 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/select_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      976 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckbox.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      765 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckboxbool_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1357 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4046 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckboxbool_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1335 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/submit_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1574 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/text_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1414 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/textarea_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3703 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/textfield_widget_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1356 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/textlines_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1812 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/templates/widget.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.868712 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2421 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/example.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1139 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/layer.py
+-rw-r--r--   0 maurits    (501) staff       (20)      907 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_csrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4554 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1349 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_widget.py
+-rw-r--r--   0 maurits    (501) staff       (20)    66068 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_widgets.py
+-rw-r--r--   0 maurits    (501) staff       (20)      776 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/testing.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2208 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/tests/tests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3393 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2739 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/views.py
+-rw-r--r--   0 maurits    (501) staff       (20)    33302 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/widget.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8895 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/widget.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.870334 plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/
+-rw-r--r--   0 maurits    (501) staff       (20)      919 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      639 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1693 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/widget.py
+-rw-r--r--   0 maurits    (501) staff       (20)      601 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/wysiwyg_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1048 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/wysiwyg_input.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:51:53.850904 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    48074 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2876 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      735 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1692 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      242 2023-04-13 22:51:53.871275 plone.app.z3cform-4.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2881 2023-04-13 22:51:53.000000 plone.app.z3cform-4.0.3/setup.py
```

### Comparing `plone.app.z3cform-4.0.2/CHANGES.rst` & `plone.app.z3cform-4.0.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,35 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-04-14)
+------------------
+
+Bug fixes:
+
+
+- Fixes transitive circular dependency to plone.schema.
+  Inherit own Browserlayer from new intermediate browserlayer in plone.schema.
+  [jensens] (#163)
+- Add ``test`` extra with the same contents as the ``tests`` extra.
+  The ``tests`` extra will be removed in Plone 7.
+  [maurits] (#164)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3b8337e6)
+
+
 4.0.2 (2023-03-23)
 ------------------
 
 Bug fixes:
 
 
 - Fix relative URLs validation in link widget
```

### Comparing `plone.app.z3cform-4.0.2/PKG-INFO` & `plone.app.z3cform-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.z3cform
-Version: 4.0.2
+Version: 4.0.3
 Summary: A collection of widgets, templates and other components for use with z3c.form and Plone
 Home-page: https://pypi.org/project/plone.app.z3cform
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: zope plone form widget template
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Provides-Extra: test
 Provides-Extra: tests
 
 =================
 plone.app.z3cform
 =================
 
 A Plone specific integration and HTML mark-up for z3c.form.
@@ -676,14 +677,35 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-04-14)
+------------------
+
+Bug fixes:
+
+
+- Fixes transitive circular dependency to plone.schema.
+  Inherit own Browserlayer from new intermediate browserlayer in plone.schema.
+  [jensens] (#163)
+- Add ``test`` extra with the same contents as the ``tests`` extra.
+  The ``tests`` extra will be removed in Plone 7.
+  [maurits] (#164)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3b8337e6)
+
+
 4.0.2 (2023-03-23)
 ------------------
 
 Bug fixes:
 
 
 - Fix relative URLs validation in link widget
```

### Comparing `plone.app.z3cform-4.0.2/README.rst` & `plone.app.z3cform-4.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/docs/LICENSE.GPL` & `plone.app.z3cform-4.0.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/docs/LICENSE.txt` & `plone.app.z3cform-4.0.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/configure.zcml` & `plone.app.z3cform-4.0.3/plone/app/z3cform/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/converters.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/converters.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/csrf.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/csrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/inline_validation.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/inline_validation.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/inline_validation.rst` & `plone.app.z3cform-4.0.3/plone/app/z3cform/inline_validation.rst`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/interfaces.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from plone.app.textfield.widget import IRichTextWidget as patextfield_IRichTextWidget
-from z3c.form.interfaces import IFormLayer
+from plone.schema.interfaces import IFormLayer
 from z3c.form.interfaces import IRadioWidget
 from z3c.form.interfaces import ISelectWidget as IBaseSelectWidget
 from z3c.form.interfaces import ISingleCheckBoxWidget
 from z3c.form.interfaces import ITextWidget
 from zope.interface import Interface
 from zope.schema.interfaces import IDate
 from zope.schema.interfaces import IDatetime
```

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/profiles.zcml` & `plone.app.z3cform-4.0.3/plone/app/z3cform/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/ajaxselect_display.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/ajaxselect_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/checkbox_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/checkbox_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/file_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/file_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/form.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/form.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/image_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/image_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/layout.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/link_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/link_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/macros.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/macros.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/multi_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/multi_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/object_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/object_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/orderedselect_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/orderedselect_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/password_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/password_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/radio_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/radio_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/radio_input_single.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/radio_input_single.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/relateditems_display.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/relateditems_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/select_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/select_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/singlecheckbox.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckbox.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/singlecheckboxbool_display.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckboxbool_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/singlecheckboxbool_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/singlecheckboxbool_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/submit_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/submit_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/text_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/text_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/textarea_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/textarea_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/textfield_widget_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/textfield_widget_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/textlines_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/textlines_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/templates/widget.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/templates/widget.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/tests/example.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/example.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/tests/layer.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/layer.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/tests/test_csrf.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_csrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/tests/test_utils.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/tests/test_widget.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/tests/test_widgets.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/tests/testing.zcml` & `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/tests/tests.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/tests/tests.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/utils.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/views.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/views.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/widget.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/widget.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/widget.zcml` & `plone.app.z3cform-4.0.3/plone/app/z3cform/widget.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/wysiwyg/README.rst` & `plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/wysiwyg/configure.zcml` & `plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/wysiwyg/widget.py` & `plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/widget.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/wysiwyg/wysiwyg_display.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/wysiwyg_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone/app/z3cform/wysiwyg/wysiwyg_input.pt` & `plone.app.z3cform-4.0.3/plone/app/z3cform/wysiwyg/wysiwyg_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone.app.z3cform.egg-info/PKG-INFO` & `plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.z3cform
-Version: 4.0.2
+Version: 4.0.3
 Summary: A collection of widgets, templates and other components for use with z3c.form and Plone
 Home-page: https://pypi.org/project/plone.app.z3cform
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: zope plone form widget template
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Provides-Extra: test
 Provides-Extra: tests
 
 =================
 plone.app.z3cform
 =================
 
 A Plone specific integration and HTML mark-up for z3c.form.
@@ -676,14 +677,35 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-04-14)
+------------------
+
+Bug fixes:
+
+
+- Fixes transitive circular dependency to plone.schema.
+  Inherit own Browserlayer from new intermediate browserlayer in plone.schema.
+  [jensens] (#163)
+- Add ``test`` extra with the same contents as the ``tests`` extra.
+  The ``tests`` extra will be removed in Plone 7.
+  [maurits] (#164)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3b8337e6)
+
+
 4.0.2 (2023-03-23)
 ------------------
 
 Bug fixes:
 
 
 - Fix relative URLs validation in link widget
```

### Comparing `plone.app.z3cform-4.0.2/plone.app.z3cform.egg-info/SOURCES.txt` & `plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/plone.app.z3cform.egg-info/requires.txt` & `plone.app.z3cform-4.0.3/plone.app.z3cform.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,27 +5,40 @@
 plone.app.widgets>=2.4.2
 plone.base
 plone.dexterity
 plone.i18n
 plone.namedfile
 plone.protect
 plone.registry
+plone.schema
 plone.uuid
 plone.z3cform
 Products.GenericSetup
 pytz
 setuptools
 z3c.form>=4.0
 z3c.relationfield
 zope.browserpage
 zope.contentprovider
 zope.globalrequest
 zope.pagetemplate
 Zope
 
+[test]
+plone.app.contenttypes[test]
+plone.app.layout
+plone.app.testing
+plone.autoform
+plone.browserlayer
+plone.supermodel
+plone.testing
+zope.annotation
+zope.intid
+zope.publisher
+
 [tests]
 plone.app.contenttypes[test]
 plone.app.layout
 plone.app.testing
 plone.autoform
 plone.browserlayer
 plone.supermodel
```

### Comparing `plone.app.z3cform-4.0.2/pyproject.toml` & `plone.app.z3cform-4.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.0.2/setup.py` & `plone.app.z3cform-4.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,26 +4,38 @@
 import os
 
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
-version = "4.0.2"
+version = "4.0.3"
 
 long_description = (
     read("README.rst")
     + "\n"
     + read("plone", "app", "z3cform", "wysiwyg", "README.rst")
     + "\n"
     + read("plone", "app", "z3cform", "inline_validation.rst")
     + "\n"
     + read("CHANGES.rst")
     + "\n"
 )
+test_requirements = [
+    "plone.app.contenttypes[test]",
+    "plone.app.layout",
+    "plone.app.testing",
+    "plone.autoform",
+    "plone.browserlayer",
+    "plone.supermodel",
+    "plone.testing",
+    "zope.annotation",
+    "zope.intid",
+    "zope.publisher",
+]
 
 setup(
     name="plone.app.z3cform",
     version=version,
     description="A collection of widgets, templates and other components "
     "for use with z3c.form and Plone",
     long_description=long_description,
@@ -60,35 +72,30 @@
         "plone.app.widgets>=2.4.2",
         "plone.base",
         "plone.dexterity",
         "plone.i18n",
         "plone.namedfile",
         "plone.protect",
         "plone.registry",
+        "plone.schema",
         "plone.uuid",
         "plone.z3cform",
         "Products.GenericSetup",
         "pytz",
         "setuptools",
         "z3c.form >= 4.0",
         "z3c.relationfield",
         "zope.browserpage",
         "zope.contentprovider",
         "zope.globalrequest",
         "zope.pagetemplate",
         "Zope",
     ],
     extras_require={
-        "tests": [
-            "plone.app.contenttypes[test]",
-            "plone.app.layout",
-            "plone.app.testing",
-            "plone.autoform",
-            "plone.browserlayer",
-            "plone.supermodel",
-            "plone.testing",
-            "zope.annotation",
-            "zope.intid",
-            "zope.publisher",
-        ]
+        # Until plone.app.z3cform 4.0.2 we only had the 'tests' extra.
+        # In 4.0.3 we introduced the 'test' extra.
+        # Keep 'tests' for backwards compatibility.
+        # Remove it in Plone 7.
+        "test": test_requirements,
+        "tests": test_requirements,
     },
 )
```

