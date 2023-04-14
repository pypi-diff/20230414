# Comparing `tmp/satnogs-network-1.98.tar.gz` & `tmp/satnogs-network-1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satnogs-network-1.98.tar", last modified: Thu Dec 15 10:13:57 2022, max compression
+gzip compressed data, was "satnogs-network-1.99.tar", last modified: Thu Dec 15 12:07:29 2022, max compression
```

## Comparing `satnogs-network-1.98.tar` & `satnogs-network-1.99.tar`

### file list

```diff
@@ -1,493 +1,493 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.412575 satnogs-network-1.98/
--rw-rw-rw-   0 root         (0) root         (0)    34523 2022-12-15 10:13:32.000000 satnogs-network-1.98/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      224 2022-12-15 10:13:32.000000 satnogs-network-1.98/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      865 2022-12-15 10:13:57.412575 satnogs-network-1.98/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1700 2022-12-15 10:13:32.000000 satnogs-network-1.98/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.235913 satnogs-network-1.98/auth0login/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 10:13:32.000000 satnogs-network-1.98/auth0login/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2022-12-15 10:13:32.000000 satnogs-network-1.98/auth0login/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      196 2022-12-15 10:13:32.000000 satnogs-network-1.98/auth0login/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2022-12-15 10:13:32.000000 satnogs-network-1.98/auth0login/auth0backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.236911 satnogs-network-1.98/auth0login/migrations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 10:13:32.000000 satnogs-network-1.98/auth0login/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-15 10:13:32.000000 satnogs-network-1.98/auth0login/models.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-15 10:13:32.000000 satnogs-network-1.98/auth0login/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2022-12-15 10:13:32.000000 satnogs-network-1.98/auth0login/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2022-12-15 10:13:32.000000 satnogs-network-1.98/auth0login/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.240903 satnogs-network-1.98/docs/
--rw-rw-rw-   0 root         (0) root         (0)     6766 2022-12-15 10:13:32.000000 satnogs-network-1.98/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.202976 satnogs-network-1.98/docs/_build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.245894 satnogs-network-1.98/docs/_build/html/
--rw-r--r--   0 root         (0) root         (0)      230 2022-12-15 10:02:57.000000 satnogs-network-1.98/docs/_build/html/.buildinfo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.248888 satnogs-network-1.98/docs/_build/html/.doctrees/
--rw-r--r--   0 root         (0) root         (0)     5013 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/.doctrees/api.doctree
--rw-r--r--   0 root         (0) root         (0)    27803 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/.doctrees/developer-guide.doctree
--rw-r--r--   0 root         (0) root         (0)    25317 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/.doctrees/environment.pickle
--rw-r--r--   0 root         (0) root         (0)     3674 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/.doctrees/index.doctree
--rw-r--r--   0 root         (0) root         (0)    15168 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/.doctrees/installation.doctree
--rw-r--r--   0 root         (0) root         (0)     7392 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/.doctrees/maintenance.doctree
--rw-r--r--   0 root         (0) root         (0)     7451 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/.doctrees/releasing.doctree
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.250884 satnogs-network-1.98/docs/_build/html/_sources/
--rw-r--r--   0 root         (0) root         (0)      452 2022-12-15 10:01:56.000000 satnogs-network-1.98/docs/_build/html/_sources/api.rst.txt
--rw-r--r--   0 root         (0) root         (0)     4708 2022-12-15 10:01:56.000000 satnogs-network-1.98/docs/_build/html/_sources/developer-guide.rst.txt
--rw-r--r--   0 root         (0) root         (0)      134 2022-12-15 10:01:56.000000 satnogs-network-1.98/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 root         (0) root         (0)     1999 2022-12-15 10:01:56.000000 satnogs-network-1.98/docs/_build/html/_sources/installation.rst.txt
--rw-r--r--   0 root         (0) root         (0)      675 2022-12-15 10:01:56.000000 satnogs-network-1.98/docs/_build/html/_sources/maintenance.rst.txt
--rw-r--r--   0 root         (0) root         (0)      865 2022-12-15 10:01:56.000000 satnogs-network-1.98/docs/_build/html/_sources/releasing.rst.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.257871 satnogs-network-1.98/docs/_build/html/_static/
--rw-r--r--   0 root         (0) root         (0)     4418 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 root         (0) root         (0)    14810 2022-12-15 10:02:57.000000 satnogs-network-1.98/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.258869 satnogs-network-1.98/docs/_build/html/_static/css/
--rw-r--r--   0 root         (0) root         (0)     3275 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.268850 satnogs-network-1.98/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 root         (0) root         (0)    87624 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 root         (0) root         (0)    67312 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 root         (0) root         (0)    86288 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 root         (0) root         (0)    66444 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 root         (0) root         (0)   165742 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   444379 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   165548 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    98024 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    77160 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 root         (0) root         (0)   323344 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 root         (0) root         (0)   193308 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 root         (0) root         (0)   309728 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 root         (0) root         (0)   184912 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 root         (0) root         (0)   328412 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 root         (0) root         (0)   195704 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 root         (0) root         (0)   309192 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 root         (0) root         (0)   182708 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 root         (0) root         (0)   123687 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 root         (0) root         (0)     4472 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/doctools.js
--rw-r--r--   0 root         (0) root         (0)      419 2022-12-15 10:02:57.000000 satnogs-network-1.98/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 root         (0) root         (0)      286 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/file.png
--rw-r--r--   0 root         (0) root         (0)   288580 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/jquery-3.6.0.js
--rw-r--r--   0 root         (0) root         (0)    89501 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/jquery.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.270846 satnogs-network-1.98/docs/_build/html/_static/js/
--rw-r--r--   0 root         (0) root         (0)      934 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 root         (0) root         (0)     4370 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 root         (0) root         (0)     2734 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 root         (0) root         (0)     4916 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 root         (0) root         (0)     4758 2022-12-15 10:02:57.000000 satnogs-network-1.98/docs/_build/html/_static/language_data.js
--rw-r--r--   0 root         (0) root         (0)       90 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/minus.png
--rw-r--r--   0 root         (0) root         (0)       90 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/plus.png
--rw-r--r--   0 root         (0) root         (0)     4819 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/_static/pygments.css
--rw-r--r--   0 root         (0) root         (0)    18215 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 root         (0) root         (0)     4712 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 root         (0) root         (0)    68420 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 root         (0) root         (0)    19530 2022-12-15 10:02:18.000000 satnogs-network-1.98/docs/_build/html/_static/underscore.js
--rw-r--r--   0 root         (0) root         (0)     6388 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/api.html
--rw-r--r--   0 root         (0) root         (0)    15157 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/developer-guide.html
--rw-r--r--   0 root         (0) root         (0)     4789 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/genindex.html
--rw-r--r--   0 root         (0) root         (0)     5863 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/index.html
--rw-r--r--   0 root         (0) root         (0)    11124 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/installation.html
--rw-r--r--   0 root         (0) root         (0)     7582 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/maintenance.html
--rw-r--r--   0 root         (0) root         (0)      326 2022-12-15 10:02:57.000000 satnogs-network-1.98/docs/_build/html/objects.inv
--rw-r--r--   0 root         (0) root         (0)     7235 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/releasing.html
--rw-r--r--   0 root         (0) root         (0)     5068 2022-12-15 10:02:56.000000 satnogs-network-1.98/docs/_build/html/search.html
--rw-r--r--   0 root         (0) root         (0)     6927 2022-12-15 10:02:57.000000 satnogs-network-1.98/docs/_build/html/searchindex.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.271844 satnogs-network-1.98/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 10:13:32.000000 satnogs-network-1.98/docs/_static/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      452 2022-12-15 10:13:32.000000 satnogs-network-1.98/docs/api.rst
--rw-rw-rw-   0 root         (0) root         (0)     3240 2022-12-15 10:13:32.000000 satnogs-network-1.98/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     4708 2022-12-15 10:13:32.000000 satnogs-network-1.98/docs/developer-guide.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-15 10:13:32.000000 satnogs-network-1.98/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1999 2022-12-15 10:13:32.000000 satnogs-network-1.98/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      675 2022-12-15 10:13:32.000000 satnogs-network-1.98/docs/maintenance.rst
--rw-rw-rw-   0 root         (0) root         (0)      865 2022-12-15 10:13:32.000000 satnogs-network-1.98/docs/releasing.rst
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-12-15 10:13:32.000000 satnogs-network-1.98/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      321 2022-12-15 10:13:32.000000 satnogs-network-1.98/docs/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    81180 2022-12-15 10:13:32.000000 satnogs-network-1.98/docs/versioneer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.415569 satnogs-network-1.98/network/
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/__init__.py
--rw-r--r--   0 root         (0) root         (0)      496 2022-12-15 10:13:57.415569 satnogs-network-1.98/network/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.277833 satnogs-network-1.98/network/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/api/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     3379 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/api/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/api/perms.py
--rw-rw-rw-   0 root         (0) root         (0)    24582 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     3746 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/api/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/api/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    10881 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/api/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.286815 satnogs-network-1.98/network/base/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5939 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      321 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1602 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/context_processors.py
--rw-rw-rw-   0 root         (0) root         (0)     4457 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/db_api.py
--rw-rw-rw-   0 root         (0) root         (0)      972 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)    11843 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.286815 satnogs-network-1.98/network/base/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.288812 satnogs-network-1.98/network/base/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/management/commands/fetch_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2937 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/management/commands/initialize.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/management/commands/update_station_last_seen.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.330731 satnogs-network-1.98/network/base/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     6933 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0002_auto_20151011_1406.py
--rw-rw-rw-   0 root         (0) root         (0)     1653 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0003_auto_20160119_1856.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0004_station_horizon.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0005_auto_20160320_1619.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0006_auto_20160325_0126.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0007_data_payload_demode.py
--rw-rw-rw-   0 root         (0) root         (0)      399 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0008_auto_20160406_1605.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0009_auto_20160506_0826.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0010_auto_20160507_1550.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0011_satellite_manual_tle.py
--rw-rw-rw-   0 root         (0) root         (0)      537 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0012_auto_20160508_1516.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0013_data_waterfall.py
--rw-rw-rw-   0 root         (0) root         (0)      537 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0014_auto_20170205_0059.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0015_auto_20170304_2041.py
--rw-rw-rw-   0 root         (0) root         (0)      519 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0016_antenna_frequency_max.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0017_auto_20170321_1046.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0018_auto_20170519_1955.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0019_satellite_status.py
--rw-rw-rw-   0 root         (0) root         (0)      399 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0020_station_description.py
--rw-rw-rw-   0 root         (0) root         (0)      388 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0021_auto_20170813_1258.py
--rw-rw-rw-   0 root         (0) root         (0)     2929 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0022_auto_20170909_2103.py
--rw-rw-rw-   0 root         (0) root         (0)     1996 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0023_auto_20170909_2103.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0024_remove_demoddata_data.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0025_auto_20170909_2111.py
--rw-rw-rw-   0 root         (0) root         (0)     2946 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0026_auto_20170909_2116.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0027_create_moderators_group.py
--rw-rw-rw-   0 root         (0) root         (0)      680 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0028_auto_20171127_2154.py
--rw-rw-rw-   0 root         (0) root         (0)      741 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0029_auto_20171216_1712.py
--rw-rw-rw-   0 root         (0) root         (0)      555 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0030_auto_20171224_1701.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0031_migrate_vetted.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0032_auto_20171224_1703.py
--rw-rw-rw-   0 root         (0) root         (0)      983 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0033_auto_20171228_1515.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0034_auto_20180202_1358.py
--rw-rw-rw-   0 root         (0) root         (0)      389 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0035_auto_20180307_1527.py
--rw-rw-rw-   0 root         (0) root         (0)     1005 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0036_auto_20180316_1216.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0037_stationstatuslog.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0038_auto_20180322_2054.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0039_auto_20180330_2243.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0040_auto_20180811_1350.py
--rw-rw-rw-   0 root         (0) root         (0)      702 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0041_auto_20180812_0915.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0042_auto_20180814_1325.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0043_auto_20180817_0923.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0044_auto_20180817_1351.py
--rw-rw-rw-   0 root         (0) root         (0)      754 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0045_auto_20180822_1947.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0046_station_client_version.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0047_auto_20180827_1318.py
--rw-rw-rw-   0 root         (0) root         (0)      558 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0048_auto_20180902_2217.py
--rw-rw-rw-   0 root         (0) root         (0)      784 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0049_auto_20180915_1503.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0050_satellite_norad_follow_id.py
--rw-rw-rw-   0 root         (0) root         (0)      399 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0051_auto_20181206_1832.py
--rw-rw-rw-   0 root         (0) root         (0)     1573 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0052_auto_20181230_2113.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0053_remove_station_uuid.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0054_station_target_utilization.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0055_add_new_antenna_type.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0056_unique_demoddata_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      512 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0057_no_null_demoddata_observation_field.py
--rw-rw-rw-   0 root         (0) root         (0)     5936 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0058_add_transmitter_into_observation_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1339 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0059_remove_mode_model.py
--rw-rw-rw-   0 root         (0) root         (0)      464 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0060_add_latest_tle_proxy_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1428 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0061_create_indexes.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0062_add_tle_source_field.py
--rw-rw-rw-   0 root         (0) root         (0)      425 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0063_increase_char_limit_on_transmitter_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0064_increase_mode_name_char_limit.py
--rw-rw-rw-   0 root         (0) root         (0)     3187 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0065_new_antenna_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1800 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0066_move_data_from_old_to_new_antenna_schema.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0067_fix_station_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0068_sort_frequency.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0069_increase_range_frequency_limits.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0070_remove_old_antenna_schema.py
--rw-rw-rw-   0 root         (0) root         (0)      345 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0071_rename_the_new_antenna_schema.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0072_change_station_antennas_related_name.py
--rw-rw-rw-   0 root         (0) root         (0)     1239 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0073_add_observation_status.py
--rw-rw-rw-   0 root         (0) root         (0)     1248 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0074_add_waterfall_status.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0075_add_waterfall_status_details.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0076_add_waterfalls_vetted_related_name.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0077_rename_observations_status_to_status.py
--rw-rw-rw-   0 root         (0) root         (0)     1324 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0078_fix_waterfall_status.py
--rw-rw-rw-   0 root         (0) root         (0)     2116 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0079_add_tle_field_in_observation_model.py
--rw-rw-rw-   0 root         (0) root         (0)      520 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0080_add_future_status.py
--rw-rw-rw-   0 root         (0) root         (0)      570 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0081_remove_tle_model.py
--rw-rw-rw-   0 root         (0) root         (0)      296 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0082_remove_transmitter_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0083_add_station_fields_in_observation.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0084_add_observation_status_index.py
--rw-rw-rw-   0 root         (0) root         (0)      736 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0085_add_audio_zipped_field_in_observation.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0086_add_index_to_observation_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      735 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0087_remove_low_cardinality_indexes_from_observation_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0088_allow_blank_value_on_station_fields_of_observations.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0089_rename_waterfall_filefield.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0090_rename_payload_filefield.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0091_filefields_for_s3_storage.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0092_add_is_image_field_for_demoddata_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0093_check_old_demoddata_if_are_images.py
--rw-rw-rw-   0 root         (0) root         (0)     2372 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0094_migrate_artifact_files_from_old_to_new_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0095_remove_satellite_manual_tle.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0096_add_violator_field_to_satellite_model.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0097_add_violator_scheduling_field_to_station_model.py
--rw-rw-rw-   0 root         (0) root         (0)      589 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0098_create_operators_group.py
--rw-rw-rw-   0 root         (0) root         (0)      943 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0099_add_basic_client_configuration_in_station_model.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0100_add_client_id_field_in_station_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0101_allow_null_alt_lat_lng_fields_in_station_model.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0102_remove_satellite_norad_follow_id.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/0103_observation_center_frequency.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26914 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/models.py
--rw-rw-rw-   0 root         (0) root         (0)     7672 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/perms.py
--rw-rw-rw-   0 root         (0) root         (0)     3987 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/rating_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)    24266 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/scheduling.py
--rw-rw-rw-   0 root         (0) root         (0)      623 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      872 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/signals.py
--rw-rw-rw-   0 root         (0) root         (0)     4305 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/stats.py
--rw-rw-rw-   0 root         (0) root         (0)    19505 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.332728 satnogs-network-1.98/network/base/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1218 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/templatetags/paginator.py
--rw-rw-rw-   0 root         (0) root         (0)     1897 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/templatetags/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/templatetags/url_replace.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/test_orbital.py
--rw-rw-rw-   0 root         (0) root         (0)     2303 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    16713 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/tests.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     7572 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9604 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.334724 satnogs-network-1.98/network/base/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1424 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/views/generic.py
--rw-rw-rw-   0 root         (0) root         (0)    16381 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/views/observation.py
--rw-rw-rw-   0 root         (0) root         (0)    21053 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/views/scheduling.py
--rw-rw-rw-   0 root         (0) root         (0)    16251 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/base/views/station.py
--rw-rw-rw-   0 root         (0) root         (0)     4143 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/celery.py
--rw-rw-rw-   0 root         (0) root         (0)    21986 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.335722 satnogs-network-1.98/network/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.335722 satnogs-network-1.98/network/static/css/
--rw-rw-rw-   0 root         (0) root         (0)      507 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/app.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.338716 satnogs-network-1.98/network/static/css/common/
--rw-rw-rw-   0 root         (0) root         (0)     4974 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/common/_custom.scss
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/common/_footer.scss
--rw-rw-rw-   0 root         (0) root         (0)      585 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/common/_info.scss
--rw-rw-rw-   0 root         (0) root         (0)      163 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/common/_navbar.scss
--rw-rw-rw-   0 root         (0) root         (0)     1831 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/common/_status.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.341710 satnogs-network-1.98/network/static/css/pages/
--rw-rw-rw-   0 root         (0) root         (0)      555 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/pages/_home.scss
--rw-rw-rw-   0 root         (0) root         (0)     1659 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/pages/_map_overrides.scss
--rw-rw-rw-   0 root         (0) root         (0)     1499 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/pages/_observation.scss
--rw-rw-rw-   0 root         (0) root         (0)     2921 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/pages/_observations.scss
--rw-rw-rw-   0 root         (0) root         (0)      634 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/pages/_satellites.scss
--rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/pages/_station_edit.scss
--rw-rw-rw-   0 root         (0) root         (0)      257 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/pages/_station_register.scss
--rw-rw-rw-   0 root         (0) root         (0)     1839 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/pages/_station_view.scss
--rw-rw-rw-   0 root         (0) root         (0)     1213 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/pages/_stations.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.342708 satnogs-network-1.98/network/static/css/partials/
--rw-rw-rw-   0 root         (0) root         (0)     1813 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/partials/_fonts.scss
--rw-rw-rw-   0 root         (0) root         (0)      695 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/partials/_mixins.scss
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/partials/_variables.scss
--rw-rw-rw-   0 root         (0) root         (0)      291 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/css/stage.css
--rw-rw-rw-   0 root         (0) root         (0)    99678 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.358678 satnogs-network-1.98/network/static/fonts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)   101828 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-Bold.eot
--rw-rw-rw-   0 root         (0) root         (0)  1156327 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-Bold.svg
--rw-rw-rw-   0 root         (0) root         (0)   269792 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-Bold.ttf
--rw-rw-rw-   0 root         (0) root         (0)   116584 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-Bold.woff
--rw-rw-rw-   0 root         (0) root         (0)   111311 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-BoldItalic.eot
--rw-rw-rw-   0 root         (0) root         (0)  1264442 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-BoldItalic.svg
--rw-rw-rw-   0 root         (0) root         (0)   287460 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-BoldItalic.ttf
--rw-rw-rw-   0 root         (0) root         (0)   128760 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-BoldItalic.woff
--rw-rw-rw-   0 root         (0) root         (0)   110273 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-Italic.eot
--rw-rw-rw-   0 root         (0) root         (0)  1234922 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-Italic.svg
--rw-rw-rw-   0 root         (0) root         (0)   282800 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-Italic.ttf
--rw-rw-rw-   0 root         (0) root         (0)   126128 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-Italic.woff
--rw-rw-rw-   0 root         (0) root         (0)   113875 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-Regular.eot
--rw-rw-rw-   0 root         (0) root         (0)  1390051 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-Regular.svg
--rw-rw-rw-   0 root         (0) root         (0)   304516 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)   130846 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/fonts/ClearSans-Regular.woff
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.359676 satnogs-network-1.98/network/static/html/
--rw-rw-rw-   0 root         (0) root         (0)     1038 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/html/502.html
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/html/503.html
--rw-rw-rw-   0 root         (0) root         (0)     1070 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/html/504.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.364666 satnogs-network-1.98/network/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     6962 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/img/error.png
--rw-rw-rw-   0 root         (0) root         (0)     5509 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/img/ground_station_no_image.png
--rw-rw-rw-   0 root         (0) root         (0)    64309 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/img/ground_station_test.jpg
--rw-rw-rw-   0 root         (0) root         (0)     5826 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/img/offline.png
--rw-rw-rw-   0 root         (0) root         (0)     1200 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/img/online.png
--rw-rw-rw-   0 root         (0) root         (0)     1432 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/img/pin.png
--rw-rw-rw-   0 root         (0) root         (0)     6336 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/img/sat.png
--rw-rw-rw-   0 root         (0) root         (0)    18476 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/img/satnogs-network-logo.png
--rw-rw-rw-   0 root         (0) root         (0)    14133 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/img/satnogs_net.png
--rw-rw-rw-   0 root         (0) root         (0)     1244 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/img/testing.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.372651 satnogs-network-1.98/network/static/js/
--rw-rw-rw-   0 root         (0) root         (0)      923 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/api-renew.js
--rw-rw-rw-   0 root         (0) root         (0)      622 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/app.js
--rw-rw-rw-   0 root         (0) root         (0)     7401 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/ax25monitor.js
--rw-rw-rw-   0 root         (0) root         (0)      399 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/current_utc.js
--rw-rw-rw-   0 root         (0) root         (0)     2977 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/frequency_utils.js
--rw-rw-rw-   0 root         (0) root         (0)      576 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/ga.js
--rw-rw-rw-   0 root         (0) root         (0)     2373 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/gridsquare.js
--rw-rw-rw-   0 root         (0) root         (0)     7150 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/map.js
--rw-rw-rw-   0 root         (0) root         (0)    45121 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/observation_new.js
--rw-rw-rw-   0 root         (0) root         (0)    19959 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/observation_view.js
--rw-rw-rw-   0 root         (0) root         (0)     6020 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/observations.js
--rw-rw-rw-   0 root         (0) root         (0)     3816 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/polar_svg.js
--rw-rw-rw-   0 root         (0) root         (0)     5379 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/satellite.js
--rw-rw-rw-   0 root         (0) root         (0)      317 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/settings_site.js
--rw-rw-rw-   0 root         (0) root         (0)    23217 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/station_edit.js
--rw-rw-rw-   0 root         (0) root         (0)      497 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/station_register_step1.js
--rw-rw-rw-   0 root         (0) root         (0)     1480 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/station_register_step2.js
--rw-rw-rw-   0 root         (0) root         (0)    19054 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/station_view.js
--rw-rw-rw-   0 root         (0) root         (0)     2491 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/stations.js
--rw-rw-rw-   0 root         (0) root         (0)      263 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/static/js/utc.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.225932 satnogs-network-1.98/network/static/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.211959 satnogs-network-1.98/network/static/lib/@eonasdan/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.211959 satnogs-network-1.98/network/static/lib/@eonasdan/tempus-dominus/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.213955 satnogs-network-1.98/network/static/lib/@eonasdan/tempus-dominus/dist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.372651 satnogs-network-1.98/network/static/lib/@eonasdan/tempus-dominus/dist/css/
--rw-r--r--   0 root         (0) root         (0)    24786 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/@eonasdan/tempus-dominus/dist/css/tempus-dominus.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.373649 satnogs-network-1.98/network/static/lib/@eonasdan/tempus-dominus/dist/js/
--rw-r--r--   0 root         (0) root         (0)    68349 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/@eonasdan/tempus-dominus/dist/js/tempus-dominus.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.373649 satnogs-network-1.98/network/static/lib/@eonasdan/tempus-dominus/dist/plugins/
--rw-r--r--   0 root         (0) root         (0)    12945 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/@eonasdan/tempus-dominus/dist/plugins/customDateFormat.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.213955 satnogs-network-1.98/network/static/lib/@popperjs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.214953 satnogs-network-1.98/network/static/lib/@popperjs/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.214953 satnogs-network-1.98/network/static/lib/@popperjs/core/dist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.374647 satnogs-network-1.98/network/static/lib/@popperjs/core/dist/umd/
--rw-r--r--   0 root         (0) root         (0)    20095 2022-08-11 07:51:20.000000 satnogs-network-1.98/network/static/lib/@popperjs/core/dist/umd/popper.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.219943 satnogs-network-1.98/network/static/lib/bootstrap/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.219943 satnogs-network-1.98/network/static/lib/bootstrap/dist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.379638 satnogs-network-1.98/network/static/lib/bootstrap/dist/css/
--rw-r--r--   0 root         (0) root         (0)   162264 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/bootstrap/dist/css/bootstrap.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.379638 satnogs-network-1.98/network/static/lib/bootstrap/dist/js/
--rw-r--r--   0 root         (0) root         (0)    83376 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/bootstrap/dist/js/bootstrap.bundle.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.215951 satnogs-network-1.98/network/static/lib/bootstrap-fileinput/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.374647 satnogs-network-1.98/network/static/lib/bootstrap-fileinput/css/
--rw-r--r--   0 root         (0) root         (0)    10232 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/bootstrap-fileinput/css/fileinput.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.375645 satnogs-network-1.98/network/static/lib/bootstrap-fileinput/js/
--rw-r--r--   0 root         (0) root         (0)   134987 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/bootstrap-fileinput/js/fileinput.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.216949 satnogs-network-1.98/network/static/lib/bootstrap-icons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.375645 satnogs-network-1.98/network/static/lib/bootstrap-icons/font/
--rw-r--r--   0 root         (0) root         (0)    95609 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/bootstrap-icons/font/bootstrap-icons.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.376644 satnogs-network-1.98/network/static/lib/bootstrap-icons/font/fonts/
--rw-r--r--   0 root         (0) root         (0)   164352 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/bootstrap-icons/font/fonts/bootstrap-icons.woff
--rw-r--r--   0 root         (0) root         (0)   121296 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/bootstrap-icons/font/fonts/bootstrap-icons.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.217947 satnogs-network-1.98/network/static/lib/bootstrap-select/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.217947 satnogs-network-1.98/network/static/lib/bootstrap-select/dist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.377642 satnogs-network-1.98/network/static/lib/bootstrap-select/dist/css/
--rw-r--r--   0 root         (0) root         (0)    11184 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/bootstrap-select/dist/css/bootstrap-select.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.377642 satnogs-network-1.98/network/static/lib/bootstrap-select/dist/js/
--rw-r--r--   0 root         (0) root         (0)    53644 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/bootstrap-select/dist/js/bootstrap-select.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.218945 satnogs-network-1.98/network/static/lib/bootstrap-slider/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.378640 satnogs-network-1.98/network/static/lib/bootstrap-slider/dist/
--rw-r--r--   0 root         (0) root         (0)    38829 2020-06-04 01:21:52.000000 satnogs-network-1.98/network/static/lib/bootstrap-slider/dist/bootstrap-slider.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.378640 satnogs-network-1.98/network/static/lib/bootstrap-slider/dist/css/
--rw-r--r--   0 root         (0) root         (0)    11184 2020-06-04 01:21:52.000000 satnogs-network-1.98/network/static/lib/bootstrap-slider/dist/css/bootstrap-slider.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.380636 satnogs-network-1.98/network/static/lib/d3/
--rw-r--r--   0 root         (0) root         (0)   151725 2016-05-05 00:29:51.000000 satnogs-network-1.98/network/static/lib/d3/d3.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.220941 satnogs-network-1.98/network/static/lib/d3-timeline/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.380636 satnogs-network-1.98/network/static/lib/d3-timeline/src/
--rw-r--r--   0 root         (0) root         (0)    21703 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/d3-timeline/src/d3-timeline.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.221939 satnogs-network-1.98/network/static/lib/dnt-helper/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.381634 satnogs-network-1.98/network/static/lib/dnt-helper/js/
--rw-r--r--   0 root         (0) root         (0)     2321 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/dnt-helper/js/dnt-helper.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.222937 satnogs-network-1.98/network/static/lib/jquery/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.382632 satnogs-network-1.98/network/static/lib/jquery/dist/
--rw-r--r--   0 root         (0) root         (0)    88145 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/jquery/dist/jquery.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.222937 satnogs-network-1.98/network/static/lib/jquery.json-viewer/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.382632 satnogs-network-1.98/network/static/lib/jquery.json-viewer/json-viewer/
--rw-r--r--   0 root         (0) root         (0)     1080 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/jquery.json-viewer/json-viewer/jquery.json-viewer.css
--rw-r--r--   0 root         (0) root         (0)     5020 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/jquery.json-viewer/json-viewer/jquery.json-viewer.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.383630 satnogs-network-1.98/network/static/lib/kaitai-struct/
--rw-r--r--   0 root         (0) root         (0)    25602 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/kaitai-struct/KaitaiStream.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.223935 satnogs-network-1.98/network/static/lib/mapbox-gl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.384628 satnogs-network-1.98/network/static/lib/mapbox-gl/dist/
--rw-r--r--   0 root         (0) root         (0)    32643 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/mapbox-gl/dist/mapbox-gl.css
--rw-r--r--   0 root         (0) root         (0)   705179 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/mapbox-gl/dist/mapbox-gl.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.224934 satnogs-network-1.98/network/static/lib/moment/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.385626 satnogs-network-1.98/network/static/lib/moment/min/
--rw-r--r--   0 root         (0) root         (0)    58103 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/moment/min/moment.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.225932 satnogs-network-1.98/network/static/lib/satellite.js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.385626 satnogs-network-1.98/network/static/lib/satellite.js/dist/
--rw-r--r--   0 root         (0) root         (0)    22342 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/satellite.js/dist/satellite.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.225932 satnogs-network-1.98/network/static/lib/wavesurfer.js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.386624 satnogs-network-1.98/network/static/lib/wavesurfer.js/dist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.386624 satnogs-network-1.98/network/static/lib/wavesurfer.js/dist/plugin/
--rw-r--r--   0 root         (0) root         (0)    10388 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/wavesurfer.js/dist/plugin/wavesurfer.spectrogram.min.js
--rw-r--r--   0 root         (0) root         (0)    58343 1985-10-26 08:15:00.000000 satnogs-network-1.98/network/static/lib/wavesurfer.js/dist/wavesurfer.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.388620 satnogs-network-1.98/network/templates/
--rw-rw-rw-   0 root         (0) root         (0)      401 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/404.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/500.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.394609 satnogs-network-1.98/network/templates/account/
--rw-rw-rw-   0 root         (0) root         (0)      111 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/base.html
--rw-rw-rw-   0 root         (0) root         (0)     2842 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/email.html
--rw-rw-rw-   0 root         (0) root         (0)      982 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/email_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      471 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/email_confirmed.html
--rw-rw-rw-   0 root         (0) root         (0)     1396 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/login.html
--rw-rw-rw-   0 root         (0) root         (0)      581 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/logout.html
--rw-rw-rw-   0 root         (0) root         (0)      466 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/password_change.html
--rw-rw-rw-   0 root         (0) root         (0)      850 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/password_reset.html
--rw-rw-rw-   0 root         (0) root         (0)      489 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      925 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/password_reset_from_key.html
--rw-rw-rw-   0 root         (0) root         (0)      267 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/password_reset_from_key_done.html
--rw-rw-rw-   0 root         (0) root         (0)      439 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/password_set.html
--rw-rw-rw-   0 root         (0) root         (0)      719 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/signup.html
--rw-rw-rw-   0 root         (0) root         (0)      578 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/verification_sent.html
--rw-rw-rw-   0 root         (0) root         (0)      936 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/account/verified_email_required.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.399600 satnogs-network-1.98/network/templates/base/
--rw-rw-rw-   0 root         (0) root         (0)     1947 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/base/about.html
--rw-rw-rw-   0 root         (0) root         (0)     3704 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/base/home.html
--rw-rw-rw-   0 root         (0) root         (0)    17110 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/base/observation_new.html
--rw-rw-rw-   0 root         (0) root         (0)    24810 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/base/observation_view.html
--rw-rw-rw-   0 root         (0) root         (0)    17224 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/base/observations.html
--rw-rw-rw-   0 root         (0) root         (0)     2046 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/base/paginator.html
--rw-rw-rw-   0 root         (0) root         (0)      781 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/base/settings_site.html
--rw-rw-rw-   0 root         (0) root         (0)    19162 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/base/station_edit.html
--rw-rw-rw-   0 root         (0) root         (0)     1088 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/base/station_register_step1.html
--rw-rw-rw-   0 root         (0) root         (0)     2220 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/base/station_register_step2.html
--rw-rw-rw-   0 root         (0) root         (0)    20653 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/base/station_view.html
--rw-rw-rw-   0 root         (0) root         (0)    10001 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/base/stations.html
--rw-rw-rw-   0 root         (0) root         (0)     7058 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.403592 satnogs-network-1.98/network/templates/includes/
--rw-rw-rw-   0 root         (0) root         (0)      138 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/includes/analytics.html
--rw-rw-rw-   0 root         (0) root         (0)       87 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/includes/auth_auth0.html
--rw-rw-rw-   0 root         (0) root         (0)      182 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/includes/auth_local.html
--rw-rw-rw-   0 root         (0) root         (0)     1705 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/includes/legend.html
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/includes/logout_auth0.html
--rw-rw-rw-   0 root         (0) root         (0)       70 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/includes/logout_local.html
--rw-rw-rw-   0 root         (0) root         (0)     1339 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/includes/observation-hotkeys.html
--rw-rw-rw-   0 root         (0) root         (0)      955 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/includes/observation-new-hotkeys.html
--rw-rw-rw-   0 root         (0) root         (0)     3955 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/includes/satellite.html
--rw-rw-rw-   0 root         (0) root         (0)      429 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/includes/stage_notice.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.404590 satnogs-network-1.98/network/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)      243 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/rest_framework/api.html
--rw-rw-rw-   0 root         (0) root         (0)      129 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/robots.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.404590 satnogs-network-1.98/network/templates/users/
--rw-rw-rw-   0 root         (0) root         (0)    13591 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/users/user_detail.html
--rw-rw-rw-   0 root         (0) root         (0)      773 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/templates/users/user_form.html
--rw-rw-rw-   0 root         (0) root         (0)      965 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.407584 satnogs-network-1.98/network/users/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1180 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/users/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/users/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.410579 satnogs-network-1.98/network/users/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     4198 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/users/migrations/0001_squashed_0002_auto_20150415_1141.py
--rw-rw-rw-   0 root         (0) root         (0)      787 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/users/migrations/0002_auto_20160123_0939.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/users/migrations/0003_auto_20160922_1505.py
--rw-rw-rw-   0 root         (0) root         (0)      691 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/users/migrations/0004_username_unicode_validator.py
--rw-rw-rw-   0 root         (0) root         (0)      433 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/users/migrations/0005_auto_20200713_0031.py
--rw-rw-rw-   0 root         (0) root         (0)      426 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/users/migrations/0006_auto_20210116_1844.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/users/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      953 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/users/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1346 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/users/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/users/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2908 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/users/views.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2022-12-15 10:13:32.000000 satnogs-network-1.98/network/wsgi.py
--rw-rw-rw-   0 root         (0) root         (0)       58 2022-12-15 10:13:32.000000 satnogs-network-1.98/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:57.412575 satnogs-network-1.98/satnogs_network.egg-info/
--rw-r--r--   0 root         (0) root         (0)      865 2022-12-15 10:13:57.000000 satnogs-network-1.98/satnogs_network.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17448 2022-12-15 10:13:57.000000 satnogs-network-1.98/satnogs_network.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-15 10:13:57.000000 satnogs-network-1.98/satnogs_network.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      756 2022-12-15 10:13:57.000000 satnogs-network-1.98/satnogs_network.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-12-15 10:13:57.000000 satnogs-network-1.98/satnogs_network.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2476 2022-12-15 10:13:57.415569 satnogs-network-1.98/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      283 2022-12-15 10:13:32.000000 satnogs-network-1.98/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    81180 2022-12-15 10:13:32.000000 satnogs-network-1.98/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.825835 satnogs-network-1.99/
+-rw-rw-rw-   0 root         (0) root         (0)    34523 2022-12-15 12:07:06.000000 satnogs-network-1.99/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      224 2022-12-15 12:07:06.000000 satnogs-network-1.99/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      865 2022-12-15 12:07:29.825835 satnogs-network-1.99/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2022-12-15 12:07:06.000000 satnogs-network-1.99/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.657817 satnogs-network-1.99/auth0login/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 12:07:06.000000 satnogs-network-1.99/auth0login/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2022-12-15 12:07:06.000000 satnogs-network-1.99/auth0login/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      196 2022-12-15 12:07:06.000000 satnogs-network-1.99/auth0login/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2022-12-15 12:07:06.000000 satnogs-network-1.99/auth0login/auth0backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.658817 satnogs-network-1.99/auth0login/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 12:07:06.000000 satnogs-network-1.99/auth0login/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-15 12:07:06.000000 satnogs-network-1.99/auth0login/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-15 12:07:06.000000 satnogs-network-1.99/auth0login/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2022-12-15 12:07:06.000000 satnogs-network-1.99/auth0login/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2022-12-15 12:07:06.000000 satnogs-network-1.99/auth0login/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.662818 satnogs-network-1.99/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     6766 2022-12-15 12:07:06.000000 satnogs-network-1.99/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.626814 satnogs-network-1.99/docs/_build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.666818 satnogs-network-1.99/docs/_build/html/
+-rw-r--r--   0 root         (0) root         (0)      230 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/.buildinfo
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.669818 satnogs-network-1.99/docs/_build/html/.doctrees/
+-rw-r--r--   0 root         (0) root         (0)     5013 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/.doctrees/api.doctree
+-rw-r--r--   0 root         (0) root         (0)    27803 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/.doctrees/developer-guide.doctree
+-rw-r--r--   0 root         (0) root         (0)    25317 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/.doctrees/environment.pickle
+-rw-r--r--   0 root         (0) root         (0)     3674 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/.doctrees/index.doctree
+-rw-r--r--   0 root         (0) root         (0)    15168 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/.doctrees/installation.doctree
+-rw-r--r--   0 root         (0) root         (0)     7392 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/.doctrees/maintenance.doctree
+-rw-r--r--   0 root         (0) root         (0)     7451 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/.doctrees/releasing.doctree
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.671819 satnogs-network-1.99/docs/_build/html/_sources/
+-rw-r--r--   0 root         (0) root         (0)      452 2022-12-15 11:55:28.000000 satnogs-network-1.99/docs/_build/html/_sources/api.rst.txt
+-rw-r--r--   0 root         (0) root         (0)     4708 2022-12-15 11:55:28.000000 satnogs-network-1.99/docs/_build/html/_sources/developer-guide.rst.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2022-12-15 11:55:28.000000 satnogs-network-1.99/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 root         (0) root         (0)     1999 2022-12-15 11:55:28.000000 satnogs-network-1.99/docs/_build/html/_sources/installation.rst.txt
+-rw-r--r--   0 root         (0) root         (0)      675 2022-12-15 11:55:28.000000 satnogs-network-1.99/docs/_build/html/_sources/maintenance.rst.txt
+-rw-r--r--   0 root         (0) root         (0)      865 2022-12-15 11:55:28.000000 satnogs-network-1.99/docs/_build/html/_sources/releasing.rst.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.678820 satnogs-network-1.99/docs/_build/html/_static/
+-rw-r--r--   0 root         (0) root         (0)     4418 2022-12-15 11:55:47.000000 satnogs-network-1.99/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 root         (0) root         (0)    14810 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.678820 satnogs-network-1.99/docs/_build/html/_static/css/
+-rw-r--r--   0 root         (0) root         (0)     3275 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.689821 satnogs-network-1.99/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 root         (0) root         (0)    87624 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 root         (0) root         (0)    67312 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 root         (0) root         (0)    86288 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 root         (0) root         (0)    66444 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 root         (0) root         (0)   165742 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   444379 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)   165548 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    98024 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)    77160 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 root         (0) root         (0)   323344 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 root         (0) root         (0)   193308 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 root         (0) root         (0)   309728 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 root         (0) root         (0)   184912 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 root         (0) root         (0)   328412 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 root         (0) root         (0)   195704 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 root         (0) root         (0)   309192 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 root         (0) root         (0)   182708 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 root         (0) root         (0)   123687 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 root         (0) root         (0)     4472 2022-12-15 11:55:47.000000 satnogs-network-1.99/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 root         (0) root         (0)      419 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 root         (0) root         (0)      286 2022-12-15 11:55:47.000000 satnogs-network-1.99/docs/_build/html/_static/file.png
+-rw-r--r--   0 root         (0) root         (0)   288580 2022-12-15 11:55:47.000000 satnogs-network-1.99/docs/_build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 root         (0) root         (0)    89501 2022-12-15 11:55:47.000000 satnogs-network-1.99/docs/_build/html/_static/jquery.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.690821 satnogs-network-1.99/docs/_build/html/_static/js/
+-rw-r--r--   0 root         (0) root         (0)      934 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 root         (0) root         (0)     4370 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 root         (0) root         (0)     2734 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 root         (0) root         (0)     4916 2022-12-15 11:55:48.000000 satnogs-network-1.99/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 root         (0) root         (0)     4758 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 root         (0) root         (0)       90 2022-12-15 11:55:47.000000 satnogs-network-1.99/docs/_build/html/_static/minus.png
+-rw-r--r--   0 root         (0) root         (0)       90 2022-12-15 11:55:47.000000 satnogs-network-1.99/docs/_build/html/_static/plus.png
+-rw-r--r--   0 root         (0) root         (0)     4819 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 root         (0) root         (0)    18215 2022-12-15 11:55:47.000000 satnogs-network-1.99/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 root         (0) root         (0)     4712 2022-12-15 11:55:47.000000 satnogs-network-1.99/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 root         (0) root         (0)    68420 2022-12-15 11:55:47.000000 satnogs-network-1.99/docs/_build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 root         (0) root         (0)    19530 2022-12-15 11:55:47.000000 satnogs-network-1.99/docs/_build/html/_static/underscore.js
+-rw-r--r--   0 root         (0) root         (0)     6388 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/api.html
+-rw-r--r--   0 root         (0) root         (0)    15157 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/developer-guide.html
+-rw-r--r--   0 root         (0) root         (0)     4789 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/genindex.html
+-rw-r--r--   0 root         (0) root         (0)     5863 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/index.html
+-rw-r--r--   0 root         (0) root         (0)    11124 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/installation.html
+-rw-r--r--   0 root         (0) root         (0)     7582 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/maintenance.html
+-rw-r--r--   0 root         (0) root         (0)      326 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/objects.inv
+-rw-r--r--   0 root         (0) root         (0)     7235 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/releasing.html
+-rw-r--r--   0 root         (0) root         (0)     5068 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/search.html
+-rw-r--r--   0 root         (0) root         (0)     6927 2022-12-15 11:56:22.000000 satnogs-network-1.99/docs/_build/html/searchindex.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.691821 satnogs-network-1.99/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 12:07:06.000000 satnogs-network-1.99/docs/_static/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      452 2022-12-15 12:07:06.000000 satnogs-network-1.99/docs/api.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3240 2022-12-15 12:07:06.000000 satnogs-network-1.99/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4708 2022-12-15 12:07:06.000000 satnogs-network-1.99/docs/developer-guide.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-15 12:07:06.000000 satnogs-network-1.99/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1999 2022-12-15 12:07:06.000000 satnogs-network-1.99/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      675 2022-12-15 12:07:06.000000 satnogs-network-1.99/docs/maintenance.rst
+-rw-rw-rw-   0 root         (0) root         (0)      865 2022-12-15 12:07:06.000000 satnogs-network-1.99/docs/releasing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-12-15 12:07:06.000000 satnogs-network-1.99/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      321 2022-12-15 12:07:06.000000 satnogs-network-1.99/docs/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    81180 2022-12-15 12:07:06.000000 satnogs-network-1.99/docs/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.827836 satnogs-network-1.99/network/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      496 2022-12-15 12:07:29.827836 satnogs-network-1.99/network/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.697821 satnogs-network-1.99/network/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/api/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     3379 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/api/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/api/perms.py
+-rw-rw-rw-   0 root         (0) root         (0)    24582 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3746 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/api/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/api/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    10881 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/api/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.705822 satnogs-network-1.99/network/base/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5939 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      321 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1602 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/context_processors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4457 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/db_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      972 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)    11843 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.706822 satnogs-network-1.99/network/base/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.707823 satnogs-network-1.99/network/base/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/management/commands/fetch_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/management/commands/initialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/management/commands/update_station_last_seen.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.747827 satnogs-network-1.99/network/base/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     6933 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0002_auto_20151011_1406.py
+-rw-rw-rw-   0 root         (0) root         (0)     1653 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0003_auto_20160119_1856.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0004_station_horizon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0005_auto_20160320_1619.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0006_auto_20160325_0126.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0007_data_payload_demode.py
+-rw-rw-rw-   0 root         (0) root         (0)      399 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0008_auto_20160406_1605.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0009_auto_20160506_0826.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0010_auto_20160507_1550.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0011_satellite_manual_tle.py
+-rw-rw-rw-   0 root         (0) root         (0)      537 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0012_auto_20160508_1516.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0013_data_waterfall.py
+-rw-rw-rw-   0 root         (0) root         (0)      537 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0014_auto_20170205_0059.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0015_auto_20170304_2041.py
+-rw-rw-rw-   0 root         (0) root         (0)      519 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0016_antenna_frequency_max.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0017_auto_20170321_1046.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0018_auto_20170519_1955.py
+-rw-rw-rw-   0 root         (0) root         (0)      480 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0019_satellite_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      399 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0020_station_description.py
+-rw-rw-rw-   0 root         (0) root         (0)      388 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0021_auto_20170813_1258.py
+-rw-rw-rw-   0 root         (0) root         (0)     2929 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0022_auto_20170909_2103.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0023_auto_20170909_2103.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0024_remove_demoddata_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0025_auto_20170909_2111.py
+-rw-rw-rw-   0 root         (0) root         (0)     2946 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0026_auto_20170909_2116.py
+-rw-rw-rw-   0 root         (0) root         (0)      564 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0027_create_moderators_group.py
+-rw-rw-rw-   0 root         (0) root         (0)      680 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0028_auto_20171127_2154.py
+-rw-rw-rw-   0 root         (0) root         (0)      741 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0029_auto_20171216_1712.py
+-rw-rw-rw-   0 root         (0) root         (0)      555 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0030_auto_20171224_1701.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0031_migrate_vetted.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0032_auto_20171224_1703.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0033_auto_20171228_1515.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0034_auto_20180202_1358.py
+-rw-rw-rw-   0 root         (0) root         (0)      389 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0035_auto_20180307_1527.py
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0036_auto_20180316_1216.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0037_stationstatuslog.py
+-rw-rw-rw-   0 root         (0) root         (0)      557 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0038_auto_20180322_2054.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0039_auto_20180330_2243.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0040_auto_20180811_1350.py
+-rw-rw-rw-   0 root         (0) root         (0)      702 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0041_auto_20180812_0915.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0042_auto_20180814_1325.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0043_auto_20180817_0923.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0044_auto_20180817_1351.py
+-rw-rw-rw-   0 root         (0) root         (0)      754 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0045_auto_20180822_1947.py
+-rw-rw-rw-   0 root         (0) root         (0)      404 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0046_station_client_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0047_auto_20180827_1318.py
+-rw-rw-rw-   0 root         (0) root         (0)      558 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0048_auto_20180902_2217.py
+-rw-rw-rw-   0 root         (0) root         (0)      784 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0049_auto_20180915_1503.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0050_satellite_norad_follow_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      399 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0051_auto_20181206_1832.py
+-rw-rw-rw-   0 root         (0) root         (0)     1573 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0052_auto_20181230_2113.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0053_remove_station_uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0054_station_target_utilization.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0055_add_new_antenna_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0056_unique_demoddata_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      512 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0057_no_null_demoddata_observation_field.py
+-rw-rw-rw-   0 root         (0) root         (0)     5936 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0058_add_transmitter_into_observation_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0059_remove_mode_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      464 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0060_add_latest_tle_proxy_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0061_create_indexes.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0062_add_tle_source_field.py
+-rw-rw-rw-   0 root         (0) root         (0)      425 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0063_increase_char_limit_on_transmitter_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0064_increase_mode_name_char_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3187 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0065_new_antenna_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1800 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0066_move_data_from_old_to_new_antenna_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0067_fix_station_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0068_sort_frequency.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0069_increase_range_frequency_limits.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0070_remove_old_antenna_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      345 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0071_rename_the_new_antenna_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      515 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0072_change_station_antennas_related_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0073_add_observation_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0074_add_waterfall_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0075_add_waterfall_status_details.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0076_add_waterfalls_vetted_related_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0077_rename_observations_status_to_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     1324 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0078_fix_waterfall_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     2116 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0079_add_tle_field_in_observation_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      520 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0080_add_future_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      570 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0081_remove_tle_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      296 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0082_remove_transmitter_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0083_add_station_fields_in_observation.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0084_add_observation_status_index.py
+-rw-rw-rw-   0 root         (0) root         (0)      736 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0085_add_audio_zipped_field_in_observation.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0086_add_index_to_observation_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0087_remove_low_cardinality_indexes_from_observation_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0088_allow_blank_value_on_station_fields_of_observations.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0089_rename_waterfall_filefield.py
+-rw-rw-rw-   0 root         (0) root         (0)      380 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0090_rename_payload_filefield.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0091_filefields_for_s3_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)      397 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0092_add_is_image_field_for_demoddata_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0093_check_old_demoddata_if_are_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0094_migrate_artifact_files_from_old_to_new_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0095_remove_satellite_manual_tle.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0096_add_violator_field_to_satellite_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0097_add_violator_scheduling_field_to_station_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      589 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0098_create_operators_group.py
+-rw-rw-rw-   0 root         (0) root         (0)      943 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0099_add_basic_client_configuration_in_station_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0100_add_client_id_field_in_station_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0101_allow_null_alt_lat_lng_fields_in_station_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0102_remove_satellite_norad_follow_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/0103_observation_center_frequency.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26914 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     7672 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/perms.py
+-rw-rw-rw-   0 root         (0) root         (0)     3987 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/rating_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)    24266 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/scheduling.py
+-rw-rw-rw-   0 root         (0) root         (0)      623 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      872 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)     4305 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/stats.py
+-rw-rw-rw-   0 root         (0) root         (0)    19505 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.748827 satnogs-network-1.99/network/base/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1218 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/templatetags/paginator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/templatetags/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/templatetags/url_replace.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/test_orbital.py
+-rw-rw-rw-   0 root         (0) root         (0)     2303 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    16713 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     7572 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9604 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.750827 satnogs-network-1.99/network/base/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/views/generic.py
+-rw-rw-rw-   0 root         (0) root         (0)    16123 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/views/observation.py
+-rw-rw-rw-   0 root         (0) root         (0)    21053 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/views/scheduling.py
+-rw-rw-rw-   0 root         (0) root         (0)    16251 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/base/views/station.py
+-rw-rw-rw-   0 root         (0) root         (0)     4143 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/celery.py
+-rw-rw-rw-   0 root         (0) root         (0)    21986 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.750827 satnogs-network-1.99/network/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.751827 satnogs-network-1.99/network/static/css/
+-rw-rw-rw-   0 root         (0) root         (0)      507 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/app.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.753827 satnogs-network-1.99/network/static/css/common/
+-rw-rw-rw-   0 root         (0) root         (0)     4974 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/common/_custom.scss
+-rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/common/_footer.scss
+-rw-rw-rw-   0 root         (0) root         (0)      585 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/common/_info.scss
+-rw-rw-rw-   0 root         (0) root         (0)      163 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/common/_navbar.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/common/_status.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.757828 satnogs-network-1.99/network/static/css/pages/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/pages/_home.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/pages/_map_overrides.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/pages/_observation.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2921 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/pages/_observations.scss
+-rw-rw-rw-   0 root         (0) root         (0)      634 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/pages/_satellites.scss
+-rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/pages/_station_edit.scss
+-rw-rw-rw-   0 root         (0) root         (0)      257 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/pages/_station_register.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/pages/_station_view.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/pages/_stations.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.758828 satnogs-network-1.99/network/static/css/partials/
+-rw-rw-rw-   0 root         (0) root         (0)     1813 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/partials/_fonts.scss
+-rw-rw-rw-   0 root         (0) root         (0)      695 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/partials/_mixins.scss
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/partials/_variables.scss
+-rw-rw-rw-   0 root         (0) root         (0)      291 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/css/stage.css
+-rw-rw-rw-   0 root         (0) root         (0)    99678 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.773830 satnogs-network-1.99/network/static/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)   101828 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-Bold.eot
+-rw-rw-rw-   0 root         (0) root         (0)  1156327 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-Bold.svg
+-rw-rw-rw-   0 root         (0) root         (0)   269792 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-Bold.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   116584 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-Bold.woff
+-rw-rw-rw-   0 root         (0) root         (0)   111311 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-BoldItalic.eot
+-rw-rw-rw-   0 root         (0) root         (0)  1264442 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-BoldItalic.svg
+-rw-rw-rw-   0 root         (0) root         (0)   287460 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-BoldItalic.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   128760 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-BoldItalic.woff
+-rw-rw-rw-   0 root         (0) root         (0)   110273 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-Italic.eot
+-rw-rw-rw-   0 root         (0) root         (0)  1234922 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-Italic.svg
+-rw-rw-rw-   0 root         (0) root         (0)   282800 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-Italic.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   126128 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-Italic.woff
+-rw-rw-rw-   0 root         (0) root         (0)   113875 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-Regular.eot
+-rw-rw-rw-   0 root         (0) root         (0)  1390051 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-Regular.svg
+-rw-rw-rw-   0 root         (0) root         (0)   304516 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   130846 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/fonts/ClearSans-Regular.woff
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.774830 satnogs-network-1.99/network/static/html/
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/html/502.html
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/html/503.html
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/html/504.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.779830 satnogs-network-1.99/network/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     6962 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/img/error.png
+-rw-rw-rw-   0 root         (0) root         (0)     5509 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/img/ground_station_no_image.png
+-rw-rw-rw-   0 root         (0) root         (0)    64309 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/img/ground_station_test.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     5826 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/img/offline.png
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/img/online.png
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/img/pin.png
+-rw-rw-rw-   0 root         (0) root         (0)     6336 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/img/sat.png
+-rw-rw-rw-   0 root         (0) root         (0)    18476 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/img/satnogs-network-logo.png
+-rw-rw-rw-   0 root         (0) root         (0)    14133 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/img/satnogs_net.png
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/img/testing.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.787831 satnogs-network-1.99/network/static/js/
+-rw-rw-rw-   0 root         (0) root         (0)      923 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/api-renew.js
+-rw-rw-rw-   0 root         (0) root         (0)      622 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/app.js
+-rw-rw-rw-   0 root         (0) root         (0)     7401 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/ax25monitor.js
+-rw-rw-rw-   0 root         (0) root         (0)      399 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/current_utc.js
+-rw-rw-rw-   0 root         (0) root         (0)     2977 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/frequency_utils.js
+-rw-rw-rw-   0 root         (0) root         (0)      576 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/ga.js
+-rw-rw-rw-   0 root         (0) root         (0)     2373 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/gridsquare.js
+-rw-rw-rw-   0 root         (0) root         (0)     7150 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/map.js
+-rw-rw-rw-   0 root         (0) root         (0)    45121 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/observation_new.js
+-rw-rw-rw-   0 root         (0) root         (0)    19959 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/observation_view.js
+-rw-rw-rw-   0 root         (0) root         (0)     6020 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/observations.js
+-rw-rw-rw-   0 root         (0) root         (0)     3816 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/polar_svg.js
+-rw-rw-rw-   0 root         (0) root         (0)     5379 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/satellite.js
+-rw-rw-rw-   0 root         (0) root         (0)      317 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/settings_site.js
+-rw-rw-rw-   0 root         (0) root         (0)    23217 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/station_edit.js
+-rw-rw-rw-   0 root         (0) root         (0)      497 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/station_register_step1.js
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/station_register_step2.js
+-rw-rw-rw-   0 root         (0) root         (0)    19054 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/station_view.js
+-rw-rw-rw-   0 root         (0) root         (0)     2491 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/stations.js
+-rw-rw-rw-   0 root         (0) root         (0)      263 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/static/js/utc.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.648816 satnogs-network-1.99/network/static/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.635815 satnogs-network-1.99/network/static/lib/@eonasdan/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.635815 satnogs-network-1.99/network/static/lib/@eonasdan/tempus-dominus/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.636815 satnogs-network-1.99/network/static/lib/@eonasdan/tempus-dominus/dist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.788831 satnogs-network-1.99/network/static/lib/@eonasdan/tempus-dominus/dist/css/
+-rw-r--r--   0 root         (0) root         (0)    24786 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/@eonasdan/tempus-dominus/dist/css/tempus-dominus.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.788831 satnogs-network-1.99/network/static/lib/@eonasdan/tempus-dominus/dist/js/
+-rw-r--r--   0 root         (0) root         (0)    68349 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/@eonasdan/tempus-dominus/dist/js/tempus-dominus.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.788831 satnogs-network-1.99/network/static/lib/@eonasdan/tempus-dominus/dist/plugins/
+-rw-r--r--   0 root         (0) root         (0)    12945 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/@eonasdan/tempus-dominus/dist/plugins/customDateFormat.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.637815 satnogs-network-1.99/network/static/lib/@popperjs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.637815 satnogs-network-1.99/network/static/lib/@popperjs/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.637815 satnogs-network-1.99/network/static/lib/@popperjs/core/dist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.789831 satnogs-network-1.99/network/static/lib/@popperjs/core/dist/umd/
+-rw-r--r--   0 root         (0) root         (0)    20095 2022-08-11 07:51:20.000000 satnogs-network-1.99/network/static/lib/@popperjs/core/dist/umd/popper.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.642815 satnogs-network-1.99/network/static/lib/bootstrap/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.643816 satnogs-network-1.99/network/static/lib/bootstrap/dist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.794832 satnogs-network-1.99/network/static/lib/bootstrap/dist/css/
+-rw-r--r--   0 root         (0) root         (0)   162264 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/bootstrap/dist/css/bootstrap.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.794832 satnogs-network-1.99/network/static/lib/bootstrap/dist/js/
+-rw-r--r--   0 root         (0) root         (0)    83376 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/bootstrap/dist/js/bootstrap.bundle.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.638815 satnogs-network-1.99/network/static/lib/bootstrap-fileinput/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.789831 satnogs-network-1.99/network/static/lib/bootstrap-fileinput/css/
+-rw-r--r--   0 root         (0) root         (0)    10232 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/bootstrap-fileinput/css/fileinput.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.790831 satnogs-network-1.99/network/static/lib/bootstrap-fileinput/js/
+-rw-r--r--   0 root         (0) root         (0)   134987 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/bootstrap-fileinput/js/fileinput.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.639815 satnogs-network-1.99/network/static/lib/bootstrap-icons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.790831 satnogs-network-1.99/network/static/lib/bootstrap-icons/font/
+-rw-r--r--   0 root         (0) root         (0)    95609 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/bootstrap-icons/font/bootstrap-icons.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.791832 satnogs-network-1.99/network/static/lib/bootstrap-icons/font/fonts/
+-rw-r--r--   0 root         (0) root         (0)   164352 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/bootstrap-icons/font/fonts/bootstrap-icons.woff
+-rw-r--r--   0 root         (0) root         (0)   121296 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/bootstrap-icons/font/fonts/bootstrap-icons.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.640815 satnogs-network-1.99/network/static/lib/bootstrap-select/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.640815 satnogs-network-1.99/network/static/lib/bootstrap-select/dist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.792832 satnogs-network-1.99/network/static/lib/bootstrap-select/dist/css/
+-rw-r--r--   0 root         (0) root         (0)    11184 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/bootstrap-select/dist/css/bootstrap-select.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.792832 satnogs-network-1.99/network/static/lib/bootstrap-select/dist/js/
+-rw-r--r--   0 root         (0) root         (0)    53644 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/bootstrap-select/dist/js/bootstrap-select.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.641815 satnogs-network-1.99/network/static/lib/bootstrap-slider/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.793832 satnogs-network-1.99/network/static/lib/bootstrap-slider/dist/
+-rw-r--r--   0 root         (0) root         (0)    38829 2020-06-04 01:21:52.000000 satnogs-network-1.99/network/static/lib/bootstrap-slider/dist/bootstrap-slider.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.793832 satnogs-network-1.99/network/static/lib/bootstrap-slider/dist/css/
+-rw-r--r--   0 root         (0) root         (0)    11184 2020-06-04 01:21:52.000000 satnogs-network-1.99/network/static/lib/bootstrap-slider/dist/css/bootstrap-slider.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.795832 satnogs-network-1.99/network/static/lib/d3/
+-rw-r--r--   0 root         (0) root         (0)   151725 2016-05-05 00:29:51.000000 satnogs-network-1.99/network/static/lib/d3/d3.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.643816 satnogs-network-1.99/network/static/lib/d3-timeline/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.795832 satnogs-network-1.99/network/static/lib/d3-timeline/src/
+-rw-r--r--   0 root         (0) root         (0)    21703 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/d3-timeline/src/d3-timeline.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.644816 satnogs-network-1.99/network/static/lib/dnt-helper/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.796832 satnogs-network-1.99/network/static/lib/dnt-helper/js/
+-rw-r--r--   0 root         (0) root         (0)     2321 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/dnt-helper/js/dnt-helper.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.645816 satnogs-network-1.99/network/static/lib/jquery/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.797832 satnogs-network-1.99/network/static/lib/jquery/dist/
+-rw-r--r--   0 root         (0) root         (0)    88145 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/jquery/dist/jquery.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.645816 satnogs-network-1.99/network/static/lib/jquery.json-viewer/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.796832 satnogs-network-1.99/network/static/lib/jquery.json-viewer/json-viewer/
+-rw-r--r--   0 root         (0) root         (0)     1080 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/jquery.json-viewer/json-viewer/jquery.json-viewer.css
+-rw-r--r--   0 root         (0) root         (0)     5020 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/jquery.json-viewer/json-viewer/jquery.json-viewer.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.797832 satnogs-network-1.99/network/static/lib/kaitai-struct/
+-rw-r--r--   0 root         (0) root         (0)    25602 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/kaitai-struct/KaitaiStream.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.646816 satnogs-network-1.99/network/static/lib/mapbox-gl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.798833 satnogs-network-1.99/network/static/lib/mapbox-gl/dist/
+-rw-r--r--   0 root         (0) root         (0)    32643 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/mapbox-gl/dist/mapbox-gl.css
+-rw-r--r--   0 root         (0) root         (0)   705179 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/mapbox-gl/dist/mapbox-gl.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.647816 satnogs-network-1.99/network/static/lib/moment/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.799832 satnogs-network-1.99/network/static/lib/moment/min/
+-rw-r--r--   0 root         (0) root         (0)    58103 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/moment/min/moment.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.647816 satnogs-network-1.99/network/static/lib/satellite.js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.800833 satnogs-network-1.99/network/static/lib/satellite.js/dist/
+-rw-r--r--   0 root         (0) root         (0)    22342 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/satellite.js/dist/satellite.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.648816 satnogs-network-1.99/network/static/lib/wavesurfer.js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.800833 satnogs-network-1.99/network/static/lib/wavesurfer.js/dist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.801833 satnogs-network-1.99/network/static/lib/wavesurfer.js/dist/plugin/
+-rw-r--r--   0 root         (0) root         (0)    10388 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/wavesurfer.js/dist/plugin/wavesurfer.spectrogram.min.js
+-rw-r--r--   0 root         (0) root         (0)    58343 1985-10-26 08:15:00.000000 satnogs-network-1.99/network/static/lib/wavesurfer.js/dist/wavesurfer.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.802833 satnogs-network-1.99/network/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      401 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/404.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/500.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.808833 satnogs-network-1.99/network/templates/account/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/base.html
+-rw-rw-rw-   0 root         (0) root         (0)     2842 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/email.html
+-rw-rw-rw-   0 root         (0) root         (0)      982 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/email_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      471 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/email_confirmed.html
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/login.html
+-rw-rw-rw-   0 root         (0) root         (0)      581 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/logout.html
+-rw-rw-rw-   0 root         (0) root         (0)      466 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/password_change.html
+-rw-rw-rw-   0 root         (0) root         (0)      850 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/password_reset.html
+-rw-rw-rw-   0 root         (0) root         (0)      489 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      925 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/password_reset_from_key.html
+-rw-rw-rw-   0 root         (0) root         (0)      267 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/password_reset_from_key_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      439 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/password_set.html
+-rw-rw-rw-   0 root         (0) root         (0)      719 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/signup.html
+-rw-rw-rw-   0 root         (0) root         (0)      578 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/verification_sent.html
+-rw-rw-rw-   0 root         (0) root         (0)      936 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/account/verified_email_required.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.813834 satnogs-network-1.99/network/templates/base/
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/base/about.html
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/base/home.html
+-rw-rw-rw-   0 root         (0) root         (0)    17110 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/base/observation_new.html
+-rw-rw-rw-   0 root         (0) root         (0)    24810 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/base/observation_view.html
+-rw-rw-rw-   0 root         (0) root         (0)    17221 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/base/observations.html
+-rw-rw-rw-   0 root         (0) root         (0)     2046 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/base/paginator.html
+-rw-rw-rw-   0 root         (0) root         (0)      781 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/base/settings_site.html
+-rw-rw-rw-   0 root         (0) root         (0)    19162 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/base/station_edit.html
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/base/station_register_step1.html
+-rw-rw-rw-   0 root         (0) root         (0)     2220 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/base/station_register_step2.html
+-rw-rw-rw-   0 root         (0) root         (0)    20653 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/base/station_view.html
+-rw-rw-rw-   0 root         (0) root         (0)    10001 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/base/stations.html
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.816834 satnogs-network-1.99/network/templates/includes/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/includes/analytics.html
+-rw-rw-rw-   0 root         (0) root         (0)       87 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/includes/auth_auth0.html
+-rw-rw-rw-   0 root         (0) root         (0)      182 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/includes/auth_local.html
+-rw-rw-rw-   0 root         (0) root         (0)     1705 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/includes/legend.html
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/includes/logout_auth0.html
+-rw-rw-rw-   0 root         (0) root         (0)       70 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/includes/logout_local.html
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/includes/observation-hotkeys.html
+-rw-rw-rw-   0 root         (0) root         (0)      955 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/includes/observation-new-hotkeys.html
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/includes/satellite.html
+-rw-rw-rw-   0 root         (0) root         (0)      429 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/includes/stage_notice.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.817834 satnogs-network-1.99/network/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)      243 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/rest_framework/api.html
+-rw-rw-rw-   0 root         (0) root         (0)      129 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/robots.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.818835 satnogs-network-1.99/network/templates/users/
+-rw-rw-rw-   0 root         (0) root         (0)    13591 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/users/user_detail.html
+-rw-rw-rw-   0 root         (0) root         (0)      773 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/templates/users/user_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      965 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.820835 satnogs-network-1.99/network/users/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/users/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/users/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.823835 satnogs-network-1.99/network/users/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/users/migrations/0001_squashed_0002_auto_20150415_1141.py
+-rw-rw-rw-   0 root         (0) root         (0)      787 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/users/migrations/0002_auto_20160123_0939.py
+-rw-rw-rw-   0 root         (0) root         (0)      688 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/users/migrations/0003_auto_20160922_1505.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/users/migrations/0004_username_unicode_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)      433 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/users/migrations/0005_auto_20200713_0031.py
+-rw-rw-rw-   0 root         (0) root         (0)      426 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/users/migrations/0006_auto_20210116_1844.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/users/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      953 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/users/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1346 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/users/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/users/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2908 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/users/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2022-12-15 12:07:06.000000 satnogs-network-1.99/network/wsgi.py
+-rw-rw-rw-   0 root         (0) root         (0)       58 2022-12-15 12:07:06.000000 satnogs-network-1.99/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:29.825835 satnogs-network-1.99/satnogs_network.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      865 2022-12-15 12:07:29.000000 satnogs-network-1.99/satnogs_network.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17448 2022-12-15 12:07:29.000000 satnogs-network-1.99/satnogs_network.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-15 12:07:29.000000 satnogs-network-1.99/satnogs_network.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      756 2022-12-15 12:07:29.000000 satnogs-network-1.99/satnogs_network.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-12-15 12:07:29.000000 satnogs-network-1.99/satnogs_network.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2476 2022-12-15 12:07:29.827836 satnogs-network-1.99/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      283 2022-12-15 12:07:06.000000 satnogs-network-1.99/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    81180 2022-12-15 12:07:06.000000 satnogs-network-1.99/versioneer.py
```

### Comparing `satnogs-network-1.98/LICENSE` & `satnogs-network-1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/PKG-INFO` & `satnogs-network-1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satnogs-network
-Version: 1.98
+Version: 1.99
 Summary: SatNOGS Network
 Home-page: https://gitlab.com/librespacefoundation/satnogs/satnogs-network
 Author: SatNOGS project
 Author-email: dev@satnogs.org
 License: AGPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `satnogs-network-1.98/README.md` & `satnogs-network-1.99/README.md`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/auth0login/auth0backend.py` & `satnogs-network-1.99/auth0login/auth0backend.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/Makefile` & `satnogs-network-1.99/docs/Makefile`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/.doctrees/api.doctree` & `satnogs-network-1.99/docs/_build/html/.doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/.doctrees/developer-guide.doctree` & `satnogs-network-1.99/docs/_build/html/.doctrees/developer-guide.doctree`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/.doctrees/environment.pickle` & `satnogs-network-1.99/docs/_build/html/.doctrees/environment.pickle`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 00000160: 6594 658c 0770 726f 6a65 6374 948c 0f53  e.e..project...S
 00000170: 6174 4e4f 4753 204e 6574 776f 726b 948c  atNOGS Network..
 00000180: 0963 6f70 7972 6967 6874 948c 2132 3031  .copyright..!201
 00000190: 342d 3230 3232 2c20 4c69 6272 6520 5370  4-2022, Libre Sp
 000001a0: 6163 6520 466f 756e 6461 7469 6f6e 948c  ace Foundation..
 000001b0: 0661 7574 686f 7294 8c07 5361 744e 4f47  .author...SatNOG
 000001c0: 5394 8c07 7665 7273 696f 6e94 8c04 312e  S...version...1.
-000001d0: 3938 948c 0772 656c 6561 7365 9468 1e8c  98...release.h..
+000001d0: 3939 948c 0772 656c 6561 7365 9468 1e8c  99...release.h..
 000001e0: 1761 7574 6f64 6f63 5f64 6566 6175 6c74  .autodoc_default
 000001f0: 5f6f 7074 696f 6e73 947d 9428 8c07 6d65  _options.}.(..me
 00000200: 6d62 6572 7394 888c 0f70 7269 7661 7465  mbers....private
 00000210: 2d6d 656d 6265 7273 9488 8c0d 756e 646f  -members....undo
 00000220: 632d 6d65 6d62 6572 7394 8875 8c0e 7465  c-members..u..te
 00000230: 6d70 6c61 7465 735f 7061 7468 945d 948c  mplates_path.]..
 00000240: 0a5f 7465 6d70 6c61 7465 7394 618c 1065  ._templates.a..e
@@ -212,18 +212,18 @@
 00000d30: 686f 7269 7a6f 6e74 616c 9468 e04e 8794  horizontal.h.N..
 00000d40: 682d 682e 685d 4e87 948c 0f68 746d 6c5f  h-h.h]N....html_
 00000d50: 7468 656d 655f 7061 7468 945d 9468 5d4e  theme_path.].h]N
 00000d60: 8794 8c12 6874 6d6c 5f74 6865 6d65 5f6f  ....html_theme_o
 00000d70: 7074 696f 6e73 947d 9468 5d4e 8794 8c0a  ptions.}.h]N....
 00000d80: 6874 6d6c 5f74 6974 6c65 948c 2253 6174  html_title.."Sat
 00000d90: 4e4f 4753 204e 6574 776f 726b 2031 2e39  NOGS Network 1.9
-00000da0: 3820 646f 6375 6d65 6e74 6174 696f 6e94  8 documentation.
+00000da0: 3920 646f 6375 6d65 6e74 6174 696f 6e94  9 documentation.
 00000db0: 685d 4e87 948c 1068 746d 6c5f 7368 6f72  h]N....html_shor
 00000dc0: 745f 7469 746c 6594 8c22 5361 744e 4f47  t_title.."SatNOG
-00000dd0: 5320 4e65 7477 6f72 6b20 312e 3938 2064  S Network 1.98 d
+00000dd0: 5320 4e65 7477 6f72 6b20 312e 3939 2064  S Network 1.99 d
 00000de0: 6f63 756d 656e 7461 7469 6f6e 9468 5d4e  ocumentation.h]N
 00000df0: 8794 8c0a 6874 6d6c 5f73 7479 6c65 944e  ....html_style.N
 00000e00: 685d 4e87 948c 0968 746d 6c5f 6c6f 676f  h]N....html_logo
 00000e10: 944e 685d 4e87 948c 0c68 746d 6c5f 6661  .Nh]N....html_fa
 00000e20: 7669 636f 6e94 4e68 5d4e 8794 6841 6842  vicon.Nh]N..hAhB
 00000e30: 685d 4e87 9468 4368 4468 5d4e 8794 682f  h]N..hChDh]N..h/
 00000e40: 6830 685d 4e87 948c 0f68 746d 6c5f 6578  h0h]N....html_ex
@@ -368,15 +368,15 @@
 000016f0: 5f69 676e 6f72 6594 5d94 8c02 5e21 9461  _ignore.]...^!.a
 00001700: 685c 4e87 948c 1c6c 696e 6b63 6865 636b  h\N....linkcheck
 00001710: 5f72 6174 655f 6c69 6d69 745f 7469 6d65  _rate_limit_time
 00001720: 6f75 7494 4740 72c0 0000 0000 0068 5c4e  out.G@r......h\N
 00001730: 8794 8c09 6d61 6e5f 7061 6765 7394 5d94  ....man_pages.].
 00001740: 2868 748c 0e73 6174 6e6f 6773 6e65 7477  (ht..satnogsnetw
 00001750: 6f72 6b94 8c14 5361 744e 4f47 5320 4e65  ork...SatNOGS Ne
-00001760: 7477 6f72 6b20 312e 3938 945d 9468 1c61  twork 1.98.].h.a
+00001760: 7477 6f72 6b20 312e 3939 945d 9468 1c61  twork 1.99.].h.a
 00001770: 4b01 7494 6168 5c4e 8794 8c0d 6d61 6e5f  K.t.ah\N....man_
 00001780: 7368 6f77 5f75 726c 7394 8968 5c4e 8794  show_urls..h\N..
 00001790: 8c1a 6d61 6e5f 6d61 6b65 5f73 6563 7469  ..man_make_secti
 000017a0: 6f6e 5f64 6972 6563 746f 7279 9489 685c  on_directory..h\
 000017b0: 4e87 948c 1373 696e 676c 6568 746d 6c5f  N....singlehtml_
 000017c0: 7369 6465 6261 7273 946a 3801 0000 685d  sidebars.j8...h]
 000017d0: 4e87 948c 1174 6578 696e 666f 5f64 6f63  N....texinfo_doc
@@ -445,15 +445,15 @@
 00001bc0: 0000 4e87 948c 1861 7070 6c65 6865 6c70  ..N....applehelp
 00001bd0: 5f62 756e 646c 655f 7665 7273 696f 6e94  _bundle_version.
 00001be0: 8c01 3194 6a48 0200 004e 8794 8c0e 6170  ..1.jH...N....ap
 00001bf0: 706c 6568 656c 705f 6963 6f6e 944e 6a48  plehelp_icon.NjH
 00001c00: 0200 004e 8794 8c14 6170 706c 6568 656c  ...N....applehel
 00001c10: 705f 6b62 5f70 726f 6475 6374 948c 1353  p_kb_product...S
 00001c20: 6174 4e4f 4753 4e65 7477 6f72 6b2d 312e  atNOGSNetwork-1.
-00001c30: 3938 946a 4802 0000 4e87 948c 1061 7070  98.jH...N....app
+00001c30: 3939 946a 4802 0000 4e87 948c 1061 7070  99.jH...N....app
 00001c40: 6c65 6865 6c70 5f6b 625f 7572 6c94 4e6a  lehelp_kb_url.Nj
 00001c50: 4802 0000 4e87 948c 1461 7070 6c65 6865  H...N....applehe
 00001c60: 6c70 5f72 656d 6f74 655f 7572 6c94 4e6a  lp_remote_url.Nj
 00001c70: 4802 0000 4e87 948c 1761 7070 6c65 6865  H...N....applehe
 00001c80: 6c70 5f69 6e64 6578 5f61 6e63 686f 7273  lp_index_anchors
 00001c90: 9489 6a48 0200 004e 8794 8c19 6170 706c  ..jH...N....appl
 00001ca0: 6568 656c 705f 6d69 6e5f 7465 726d 5f6c  ehelp_min_term_l
@@ -533,17 +533,17 @@
 00002140: 628c 0d63 6f6e 6669 675f 7374 6174 7573  b..config_status
 00002150: 944b 018c 1363 6f6e 6669 675f 7374 6174  .K...config_stat
 00002160: 7573 5f65 7874 7261 9468 5c8c 0665 7665  us_extra.h\..eve
 00002170: 6e74 7394 4e68 178c 0e73 7068 696e 782e  nts.Nh...sphinx.
 00002180: 7072 6f6a 6563 7494 8c07 5072 6f6a 6563  project...Projec
 00002190: 7494 9394 2981 947d 9428 6808 6809 6845  t...)..}.(h.h.hE
 000021a0: 6849 8c08 646f 636e 616d 6573 948f 9428  hI..docnames...(
-000021b0: 8c0f 6465 7665 6c6f 7065 722d 6775 6964  ..developer-guid
-000021c0: 6594 8c03 6170 6994 8c0c 696e 7374 616c  e...api...instal
-000021d0: 6c61 7469 6f6e 948c 0972 656c 6561 7369  lation...releasi
+000021b0: 8c0c 696e 7374 616c 6c61 7469 6f6e 948c  ..installation..
+000021c0: 0361 7069 948c 0f64 6576 656c 6f70 6572  .api...developer
+000021d0: 2d67 7569 6465 948c 0972 656c 6561 7369  -guide...releasi
 000021e0: 6e67 948c 0b6d 6169 6e74 656e 616e 6365  ng...maintenance
 000021f0: 948c 0569 6e64 6578 9490 7562 681d 7d94  ...index..ubh.}.
 00002200: 288c 1073 7068 696e 782e 646f 6d61 696e  (..sphinx.domain
 00002210: 732e 6394 4b02 8c18 7370 6869 6e78 2e64  s.c.K...sphinx.d
 00002220: 6f6d 6169 6e73 2e63 6861 6e67 6573 6574  omains.changeset
 00002230: 944b 018c 1773 7068 696e 782e 646f 6d61  .K...sphinx.doma
 00002240: 696e 732e 6369 7461 7469 6f6e 944b 018c  ins.citation.K..
@@ -586,20 +586,20 @@
 00002490: 6c94 4b05 8c16 6669 6c65 5f69 6e73 6572  l.K...file_inser
 000024a0: 7469 6f6e 5f65 6e61 626c 6564 9488 8c13  tion_enabled....
 000024b0: 736d 6172 7471 756f 7465 735f 6c6f 6361  smartquotes_loca
 000024c0: 6c65 7394 5d94 6858 6803 688c 898c 0d6c  les.].hXh.h....l
 000024d0: 616e 6775 6167 655f 636f 6465 9468 678c  anguage_code.hg.
 000024e0: 0c73 6d61 7274 5f71 756f 7465 7394 8875  .smart_quotes..u
 000024f0: 8c08 616c 6c5f 646f 6373 947d 9428 6abb  ..all_docs.}.(j.
-00002500: 0200 0047 41d8 e6bc 3427 3083 6aba 0200  ...GA...4'0.j...
-00002510: 0047 41d8 e6bc 3429 7d1c 6abf 0200 0047  .GA...4)}.j....G
-00002520: 41d8 e6bc 3429 eff0 6abc 0200 0047 41d8  A...4)..j....GA.
-00002530: e6bc 342b 0da7 6abe 0200 0047 41d8 e6bc  ..4+..j....GA...
-00002540: 342b b8ea 6abd 0200 0047 41d8 e6bc 342c  4+..j....GA...4,
-00002550: 68d0 758c 0c64 6570 656e 6465 6e63 6965  h.u..dependencie
+00002500: 0200 0047 41d8 e6c2 d98d 11a1 6abc 0200  ...GA.......j...
+00002510: 0047 41d8 e6c2 d98f 29ec 6abf 0200 0047  .GA.....).j....G
+00002520: 41d8 e6c2 d98f 826d 6aba 0200 0047 41d8  A......mj....GA.
+00002530: e6c2 d990 8573 6abe 0200 0047 41d8 e6c2  .....sj....GA...
+00002540: d991 1898 6abd 0200 0047 41d8 e6c2 d991  ....j....GA.....
+00002550: adbb 758c 0c64 6570 656e 6465 6e63 6965  ..u..dependencie
 00002560: 7394 6846 8c0b 6465 6661 756c 7464 6963  s.hF..defaultdic
 00002570: 7494 9394 8c08 6275 696c 7469 6e73 948c  t.....builtins..
 00002580: 0373 6574 9493 9485 9452 948c 0869 6e63  .set.....R...inc
 00002590: 6c75 6465 6494 6aec 0200 006a ef02 0000  luded.j....j....
 000025a0: 8594 5294 8c0d 7265 7265 6164 5f61 6c77  ..R...reread_alw
 000025b0: 6179 7394 8f94 8c08 6d65 7461 6461 7461  ays.....metadata
 000025c0: 946a ec02 0000 6aed 0200 008c 0464 6963  .j....j......dic
@@ -612,15 +612,15 @@
 00002630: 9493 948c 0341 5049 9485 9481 947d 948c  .....API.....}..
 00002640: 0670 6172 656e 7494 6a01 0300 0073 6261  .parent.j....sba
 00002650: 8c0a 6174 7472 6962 7574 6573 947d 9428  ..attributes.}.(
 00002660: 8c03 6964 7394 5d94 8c07 636c 6173 7365  ..ids.]...classe
 00002670: 7394 5d94 8c05 6e61 6d65 7394 5d94 8c08  s.]...names.]...
 00002680: 6475 706e 616d 6573 945d 948c 0862 6163  dupnames.]...bac
 00002690: 6b72 6566 7394 5d94 758c 0774 6167 6e61  krefs.].u..tagna
-000026a0: 6d65 946a ff02 0000 7562 6aba 0200 006a  me.j....ubj....j
+000026a0: 6d65 946a ff02 0000 7562 6abc 0200 006a  me.j....ubj....j
 000026b0: 0003 0000 2981 947d 9428 6a03 0300 0068  ....)..}.(j....h
 000026c0: 5c6a 0403 0000 5d94 6a07 0300 008c 0f44  \j....].j......D
 000026d0: 6576 656c 6f70 6572 2047 7569 6465 9485  eveloper Guide..
 000026e0: 9481 947d 946a 0c03 0000 6a1a 0300 0073  ...}.j....j....s
 000026f0: 6261 6a0d 0300 007d 9428 6a0f 0300 005d  baj....}.(j....]
 00002700: 946a 1103 0000 5d94 6a13 0300 005d 946a  .j....].j....].j
 00002710: 1503 0000 5d94 6a17 0300 005d 9475 6a19  ....].j....].uj.
@@ -628,15 +628,15 @@
 00002730: 0003 0000 2981 947d 9428 6a03 0300 0068  ....)..}.(j....h
 00002740: 5c6a 0403 0000 5d94 6a07 0300 008c 0f73  \j....].j......s
 00002750: 6174 6e6f 6773 2d6e 6574 776f 726b 9485  atnogs-network..
 00002760: 9481 947d 946a 0c03 0000 6a27 0300 0073  ...}.j....j'...s
 00002770: 6261 6a0d 0300 007d 9428 6a0f 0300 005d  baj....}.(j....]
 00002780: 946a 1103 0000 5d94 6a13 0300 005d 946a  .j....].j....].j
 00002790: 1503 0000 5d94 6a17 0300 005d 9475 6a19  ....].j....].uj.
-000027a0: 0300 006a ff02 0000 7562 6abc 0200 006a  ...j....ubj....j
+000027a0: 0300 006a ff02 0000 7562 6aba 0200 006a  ...j....ubj....j
 000027b0: 0003 0000 2981 947d 9428 6a03 0300 0068  ....)..}.(j....h
 000027c0: 5c6a 0403 0000 5d94 6a07 0300 008c 0c49  \j....].j......I
 000027d0: 6e73 7461 6c6c 6174 696f 6e94 8594 8194  nstallation.....
 000027e0: 7d94 6a0c 0300 006a 3403 0000 7362 616a  }.j....j4...sbaj
 000027f0: 0d03 0000 7d94 286a 0f03 0000 5d94 6a11  ....}.(j....].j.
 00002800: 0300 005d 946a 1303 0000 5d94 6a15 0300  ...].j....].j...
 00002810: 005d 946a 1703 0000 5d94 756a 1903 0000  .].j....].uj....
@@ -653,16 +653,16 @@
 000028c0: 946a 0703 0000 8c09 5265 6c65 6173 696e  .j......Releasin
 000028d0: 6794 8594 8194 7d94 6a0c 0300 006a 4e03  g.....}.j....jN.
 000028e0: 0000 7362 616a 0d03 0000 7d94 286a 0f03  ..sbaj....}.(j..
 000028f0: 0000 5d94 6a11 0300 005d 946a 1303 0000  ..].j....].j....
 00002900: 5d94 6a15 0300 005d 946a 1703 0000 5d94  ].j....].j....].
 00002910: 756a 1903 0000 6aff 0200 0075 6275 8c0a  uj....j....ubu..
 00002920: 6c6f 6e67 7469 746c 6573 947d 9428 6abb  longtitles.}.(j.
-00002930: 0200 006a 0103 0000 6aba 0200 006a 1a03  ...j....j....j..
-00002940: 0000 6abf 0200 006a 2703 0000 6abc 0200  ..j....j'...j...
+00002930: 0200 006a 0103 0000 6abc 0200 006a 1a03  ...j....j....j..
+00002940: 0000 6abf 0200 006a 2703 0000 6aba 0200  ..j....j'...j...
 00002950: 006a 3403 0000 6abe 0200 006a 4103 0000  .j4...j....jA...
 00002960: 6abd 0200 006a 4e03 0000 758c 0474 6f63  j....jN...u..toc
 00002970: 7394 7d94 286a bb02 0000 6afe 0200 008c  s.}.(j....j.....
 00002980: 0b62 756c 6c65 745f 6c69 7374 9493 9429  .bullet_list...)
 00002990: 8194 7d94 286a 0303 0000 685c 6a04 0300  ..}.(j....h\j...
 000029a0: 005d 946a fe02 0000 8c09 6c69 7374 5f69  .].j......list_i
 000029b0: 7465 6d94 9394 2981 947d 9428 6a03 0300  tem...)..}.(j...
@@ -741,29 +741,29 @@
 00002e40: 6a0d 0300 007d 9428 6a0f 0300 005d 946a  j....}.(j....].j
 00002e50: 1103 0000 5d94 6a13 0300 005d 946a 1503  ....].j....].j..
 00002e60: 0000 5d94 6a17 0300 005d 9475 6a19 0300  ..].j....].uj...
 00002e70: 006a 6403 0000 6a0c 0300 006a 6103 0000  .jd...j....ja...
 00002e80: 7562 616a 0d03 0000 7d94 286a 0f03 0000  ubaj....}.(j....
 00002e90: 5d94 6a11 0300 005d 946a 1303 0000 5d94  ].j....].j....].
 00002ea0: 6a15 0300 005d 946a 1703 0000 5d94 756a  j....].j....].uj
-00002eb0: 1903 0000 6a5f 0300 0075 626a ba02 0000  ....j_...ubj....
+00002eb0: 1903 0000 6a5f 0300 0075 626a bc02 0000  ....j_...ubj....
 00002ec0: 6a60 0300 0029 8194 7d94 286a 0303 0000  j`...)..}.(j....
 00002ed0: 685c 6a04 0300 005d 946a 6503 0000 2981  h\j....].je...).
 00002ee0: 947d 9428 6a03 0300 0068 5c6a 0403 0000  .}.(j....h\j....
 00002ef0: 5d94 286a 6b03 0000 2981 947d 9428 6a03  ].(jk...)..}.(j.
 00002f00: 0300 0068 5c6a 0403 0000 5d94 6a70 0300  ...h\j....].jp..
 00002f10: 0029 8194 7d94 286a 0303 0000 685c 6a04  .)..}.(j....h\j.
 00002f20: 0300 005d 946a 0703 0000 8c0f 4465 7665  ...].j......Deve
 00002f30: 6c6f 7065 7220 4775 6964 6594 8594 8194  loper Guide.....
 00002f40: 7d94 6a0c 0300 006a eb03 0000 7362 616a  }.j....j....sbaj
 00002f50: 0d03 0000 7d94 286a 0f03 0000 5d94 6a11  ....}.(j....].j.
 00002f60: 0300 005d 946a 1303 0000 5d94 6a15 0300  ...].j....].j...
 00002f70: 005d 946a 1703 0000 5d94 8c08 696e 7465  .].j....]...inte
 00002f80: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
-00002f90: ba02 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
+00002f90: bc02 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
 00002fa0: 9468 5c75 6a19 0300 006a 6f03 0000 6a0c  .h\uj....jo...j.
 00002fb0: 0300 006a e803 0000 7562 616a 0d03 0000  ...j....ubaj....
 00002fc0: 7d94 286a 0f03 0000 5d94 6a11 0300 005d  }.(j....].j....]
 00002fd0: 946a 1303 0000 5d94 6a15 0300 005d 946a  .j....].j....].j
 00002fe0: 1703 0000 5d94 756a 1903 0000 6a6a 0300  ....].uj....jj..
 00002ff0: 006a 0c03 0000 6ae5 0300 0075 626a 6003  .j....j....ubj`.
 00003000: 0000 2981 947d 9428 6a03 0300 0068 5c6a  ..)..}.(j....h\j
@@ -774,15 +774,15 @@
 00003050: 947d 9428 6a03 0300 0068 5c6a 0403 0000  .}.(j....h\j....
 00003060: 5d94 6a07 0300 008c 0857 6f72 6b66 6c6f  ].j......Workflo
 00003070: 7794 8594 8194 7d94 6a0c 0300 006a 0a04  w.....}.j....j..
 00003080: 0000 7362 616a 0d03 0000 7d94 286a 0f03  ..sbaj....}.(j..
 00003090: 0000 5d94 6a11 0300 005d 946a 1303 0000  ..].j....].j....
 000030a0: 5d94 6a15 0300 005d 946a 1703 0000 5d94  ].j....].j....].
 000030b0: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
-000030c0: 6675 7269 946a ba02 0000 8c0a 616e 6368  furi.j......anch
+000030c0: 6675 7269 946a bc02 0000 8c0a 616e 6368  furi.j......anch
 000030d0: 6f72 6e61 6d65 948c 0923 776f 726b 666c  orname...#workfl
 000030e0: 6f77 9475 6a19 0300 006a 6f03 0000 6a0c  ow.uj....jo...j.
 000030f0: 0300 006a 0704 0000 7562 616a 0d03 0000  ...j....ubaj....
 00003100: 7d94 286a 0f03 0000 5d94 6a11 0300 005d  }.(j....].j....]
 00003110: 946a 1303 0000 5d94 6a15 0300 005d 946a  .j....].j....].j
 00003120: 1703 0000 5d94 756a 1903 0000 6a6a 0300  ....].uj....jj..
 00003130: 006a 0c03 0000 6a04 0400 0075 6261 6a0d  .j....j....ubaj.
@@ -797,15 +797,15 @@
 000031c0: 0000 685c 6a04 0300 005d 946a 0703 0000  ..h\j....].j....
 000031d0: 8c09 5465 6d70 6c61 7465 7394 8594 8194  ..Templates.....
 000031e0: 7d94 6a0c 0300 006a 2d04 0000 7362 616a  }.j....j-...sbaj
 000031f0: 0d03 0000 7d94 286a 0f03 0000 5d94 6a11  ....}.(j....].j.
 00003200: 0300 005d 946a 1303 0000 5d94 6a15 0300  ...].j....].j...
 00003210: 005d 946a 1703 0000 5d94 8c08 696e 7465  .].j....]...inte
 00003220: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
-00003230: ba02 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
+00003230: bc02 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
 00003240: 948c 0a23 7465 6d70 6c61 7465 7394 756a  ...#templates.uj
 00003250: 1903 0000 6a6f 0300 006a 0c03 0000 6a2a  ....jo...j....j*
 00003260: 0400 0075 6261 6a0d 0300 007d 9428 6a0f  ...ubaj....}.(j.
 00003270: 0300 005d 946a 1103 0000 5d94 6a13 0300  ...].j....].j...
 00003280: 005d 946a 1503 0000 5d94 6a17 0300 005d  .].j....].j....]
 00003290: 9475 6a19 0300 006a 6a03 0000 6a0c 0300  .uj....jj...j...
 000032a0: 006a 2704 0000 7562 616a 0d03 0000 7d94  .j'...ubaj....}.
@@ -820,15 +820,15 @@
 00003330: 0403 0000 5d94 6a07 0300 008c 1446 726f  ....].j......Fro
 00003340: 6e74 656e 6420 6465 7665 6c6f 706d 656e  ntend developmen
 00003350: 7494 8594 8194 7d94 6a0c 0300 006a 5004  t.....}.j....jP.
 00003360: 0000 7362 616a 0d03 0000 7d94 286a 0f03  ..sbaj....}.(j..
 00003370: 0000 5d94 6a11 0300 005d 946a 1303 0000  ..].j....].j....
 00003380: 5d94 6a15 0300 005d 946a 1703 0000 5d94  ].j....].j....].
 00003390: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
-000033a0: 6675 7269 946a ba02 0000 8c0a 616e 6368  furi.j......anch
+000033a0: 6675 7269 946a bc02 0000 8c0a 616e 6368  furi.j......anch
 000033b0: 6f72 6e61 6d65 948c 1523 6672 6f6e 7465  orname...#fronte
 000033c0: 6e64 2d64 6576 656c 6f70 6d65 6e74 9475  nd-development.u
 000033d0: 6a19 0300 006a 6f03 0000 6a0c 0300 006a  j....jo...j....j
 000033e0: 4d04 0000 7562 616a 0d03 0000 7d94 286a  M...ubaj....}.(j
 000033f0: 0f03 0000 5d94 6a11 0300 005d 946a 1303  ....].j....].j..
 00003400: 0000 5d94 6a15 0300 005d 946a 1703 0000  ..].j....].j....
 00003410: 5d94 756a 1903 0000 6a6a 0300 006a 0c03  ].uj....jj...j..
@@ -844,15 +844,15 @@
 000034b0: 6a04 0300 005d 946a 0703 0000 8c13 4261  j....].j......Ba
 000034c0: 636b 656e 6420 6465 7665 6c6f 706d 656e  ckend developmen
 000034d0: 7494 8594 8194 7d94 6a0c 0300 006a 7304  t.....}.j....js.
 000034e0: 0000 7362 616a 0d03 0000 7d94 286a 0f03  ..sbaj....}.(j..
 000034f0: 0000 5d94 6a11 0300 005d 946a 1303 0000  ..].j....].j....
 00003500: 5d94 6a15 0300 005d 946a 1703 0000 5d94  ].j....].j....].
 00003510: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
-00003520: 6675 7269 946a ba02 0000 8c0a 616e 6368  furi.j......anch
+00003520: 6675 7269 946a bc02 0000 8c0a 616e 6368  furi.j......anch
 00003530: 6f72 6e61 6d65 948c 1423 6261 636b 656e  orname...#backen
 00003540: 642d 6465 7665 6c6f 706d 656e 7494 756a  d-development.uj
 00003550: 1903 0000 6a6f 0300 006a 0c03 0000 6a70  ....jo...j....jp
 00003560: 0400 0075 6261 6a0d 0300 007d 9428 6a0f  ...ubaj....}.(j.
 00003570: 0300 005d 946a 1103 0000 5d94 6a13 0300  ...].j....].j...
 00003580: 005d 946a 1503 0000 5d94 6a17 0300 005d  .].j....].j....]
 00003590: 9475 6a19 0300 006a 6a03 0000 6a0c 0300  .uj....jj...j...
@@ -868,15 +868,15 @@
 00003630: 0403 0000 5d94 6a07 0300 008c 1d53 696d  ....].j......Sim
 00003640: 756c 6174 696e 6720 7374 6174 696f 6e20  ulating station 
 00003650: 6865 6172 7462 6561 7473 9485 9481 947d  heartbeats.....}
 00003660: 946a 0c03 0000 6a96 0400 0073 6261 6a0d  .j....j....sbaj.
 00003670: 0300 007d 9428 6a0f 0300 005d 946a 1103  ...}.(j....].j..
 00003680: 0000 5d94 6a13 0300 005d 946a 1503 0000  ..].j....].j....
 00003690: 5d94 6a17 0300 005d 948c 0869 6e74 6572  ].j....]...inter
-000036a0: 6e61 6c94 888c 0672 6566 7572 6994 6aba  nal....refuri.j.
+000036a0: 6e61 6c94 888c 0672 6566 7572 6994 6abc  nal....refuri.j.
 000036b0: 0200 008c 0a61 6e63 686f 726e 616d 6594  .....anchorname.
 000036c0: 8c1e 2373 696d 756c 6174 696e 672d 7374  ..#simulating-st
 000036d0: 6174 696f 6e2d 6865 6172 7462 6561 7473  ation-heartbeats
 000036e0: 9475 6a19 0300 006a 6f03 0000 6a0c 0300  .uj....jo...j...
 000036f0: 006a 9304 0000 7562 616a 0d03 0000 7d94  .j....ubaj....}.
 00003700: 286a 0f03 0000 5d94 6a11 0300 005d 946a  (j....].j....].j
 00003710: 1303 0000 5d94 6a15 0300 005d 946a 1703  ....].j....].j..
@@ -894,15 +894,15 @@
 000037d0: 4d61 6e75 616c 6c79 2072 756e 2061 2063  Manually run a c
 000037e0: 656c 6572 7920 7461 736b 7394 8594 8194  elery tasks.....
 000037f0: 7d94 6a0c 0300 006a b904 0000 7362 616a  }.j....j....sbaj
 00003800: 0d03 0000 7d94 286a 0f03 0000 5d94 6a11  ....}.(j....].j.
 00003810: 0300 005d 946a 1303 0000 5d94 6a15 0300  ...].j....].j...
 00003820: 005d 946a 1703 0000 5d94 8c08 696e 7465  .].j....]...inte
 00003830: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
-00003840: ba02 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
+00003840: bc02 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
 00003850: 948c 1c23 6d61 6e75 616c 6c79 2d72 756e  ...#manually-run
 00003860: 2d61 2d63 656c 6572 792d 7461 736b 7394  -a-celery-tasks.
 00003870: 756a 1903 0000 6a6f 0300 006a 0c03 0000  uj....jo...j....
 00003880: 6ab6 0400 0075 6261 6a0d 0300 007d 9428  j....ubaj....}.(
 00003890: 6a0f 0300 005d 946a 1103 0000 5d94 6a13  j....].j....].j.
 000038a0: 0300 005d 946a 1503 0000 5d94 6a17 0300  ...].j....].j...
 000038b0: 005d 9475 6a19 0300 006a 6a03 0000 6a0c  .].uj....jj...j.
@@ -918,15 +918,15 @@
 00003950: 5c6a 0403 0000 5d94 6a07 0300 008c 1952  \j....].j......R
 00003960: 756e 6e69 6e67 2074 6865 2074 6573 7473  unning the tests
 00003970: 206c 6f63 616c 6c79 9485 9481 947d 946a   locally.....}.j
 00003980: 0c03 0000 6adc 0400 0073 6261 6a0d 0300  ....j....sbaj...
 00003990: 007d 9428 6a0f 0300 005d 946a 1103 0000  .}.(j....].j....
 000039a0: 5d94 6a13 0300 005d 946a 1503 0000 5d94  ].j....].j....].
 000039b0: 6a17 0300 005d 948c 0869 6e74 6572 6e61  j....]...interna
-000039c0: 6c94 888c 0672 6566 7572 6994 6aba 0200  l....refuri.j...
+000039c0: 6c94 888c 0672 6566 7572 6994 6abc 0200  l....refuri.j...
 000039d0: 008c 0a61 6e63 686f 726e 616d 6594 8c1a  ...anchorname...
 000039e0: 2372 756e 6e69 6e67 2d74 6865 2d74 6573  #running-the-tes
 000039f0: 7473 2d6c 6f63 616c 6c79 9475 6a19 0300  ts-locally.uj...
 00003a00: 006a 6f03 0000 6a0c 0300 006a d904 0000  .jo...j....j....
 00003a10: 7562 616a 0d03 0000 7d94 286a 0f03 0000  ubaj....}.(j....
 00003a20: 5d94 6a11 0300 005d 946a 1303 0000 5d94  ].j....].j....].
 00003a30: 6a15 0300 005d 946a 1703 0000 5d94 756a  j....].j....].uj
@@ -942,15 +942,15 @@
 00003ad0: 8194 7d94 286a 0303 0000 685c 6a04 0300  ..}.(j....h\j...
 00003ae0: 005d 946a 0703 0000 8c0c 436f 6469 6e67  .].j......Coding
 00003af0: 2053 7479 6c65 9485 9481 947d 946a 0c03   Style.....}.j..
 00003b00: 0000 6aff 0400 0073 6261 6a0d 0300 007d  ..j....sbaj....}
 00003b10: 9428 6a0f 0300 005d 946a 1103 0000 5d94  .(j....].j....].
 00003b20: 6a13 0300 005d 946a 1503 0000 5d94 6a17  j....].j....].j.
 00003b30: 0300 005d 948c 0869 6e74 6572 6e61 6c94  ...]...internal.
-00003b40: 888c 0672 6566 7572 6994 6aba 0200 008c  ...refuri.j.....
+00003b40: 888c 0672 6566 7572 6994 6abc 0200 008c  ...refuri.j.....
 00003b50: 0a61 6e63 686f 726e 616d 6594 8c0d 2363  .anchorname...#c
 00003b60: 6f64 696e 672d 7374 796c 6594 756a 1903  oding-style.uj..
 00003b70: 0000 6a6f 0300 006a 0c03 0000 6afc 0400  ..jo...j....j...
 00003b80: 0075 6261 6a0d 0300 007d 9428 6a0f 0300  .ubaj....}.(j...
 00003b90: 005d 946a 1103 0000 5d94 6a13 0300 005d  .].j....].j....]
 00003ba0: 946a 1503 0000 5d94 6a17 0300 005d 9475  .j....].j....].u
 00003bb0: 6a19 0300 006a 6a03 0000 6a0c 0300 006a  j....jj...j....j
@@ -965,15 +965,15 @@
 00003c40: 2981 947d 9428 6a03 0300 0068 5c6a 0403  )..}.(j....h\j..
 00003c50: 0000 5d94 6a07 0300 008c 0f57 6861 7420  ..].j......What 
 00003c60: 746f 2077 6f72 6b20 6f6e 9485 9481 947d  to work on.....}
 00003c70: 946a 0c03 0000 6a22 0500 0073 6261 6a0d  .j....j"...sbaj.
 00003c80: 0300 007d 9428 6a0f 0300 005d 946a 1103  ...}.(j....].j..
 00003c90: 0000 5d94 6a13 0300 005d 946a 1503 0000  ..].j....].j....
 00003ca0: 5d94 6a17 0300 005d 948c 0869 6e74 6572  ].j....]...inter
-00003cb0: 6e61 6c94 888c 0672 6566 7572 6994 6aba  nal....refuri.j.
+00003cb0: 6e61 6c94 888c 0672 6566 7572 6994 6abc  nal....refuri.j.
 00003cc0: 0200 008c 0a61 6e63 686f 726e 616d 6594  .....anchorname.
 00003cd0: 8c10 2377 6861 742d 746f 2d77 6f72 6b2d  ..#what-to-work-
 00003ce0: 6f6e 9475 6a19 0300 006a 6f03 0000 6a0c  on.uj....jo...j.
 00003cf0: 0300 006a 1f05 0000 7562 616a 0d03 0000  ...j....ubaj....
 00003d00: 7d94 286a 0f03 0000 5d94 6a11 0300 005d  }.(j....].j....]
 00003d10: 946a 1303 0000 5d94 6a15 0300 005d 946a  .j....].j....].j
 00003d20: 1703 0000 5d94 756a 1903 0000 6a6a 0300  ....].uj....jj..
@@ -1051,28 +1051,28 @@
 000041a0: 9428 6a0f 0300 005d 946a 1103 0000 5d94  .(j....].j....].
 000041b0: 6a13 0300 005d 946a 1503 0000 5d94 6a17  j....].j....].j.
 000041c0: 0300 005d 9475 6a19 0300 006a 6403 0000  ...].uj....jd...
 000041d0: 6a0c 0300 006a 5105 0000 7562 616a 0d03  j....jQ...ubaj..
 000041e0: 0000 7d94 286a 0f03 0000 5d94 6a11 0300  ..}.(j....].j...
 000041f0: 005d 946a 1303 0000 5d94 6a15 0300 005d  .].j....].j....]
 00004200: 946a 1703 0000 5d94 756a 1903 0000 6a5f  .j....].uj....j_
-00004210: 0300 0075 626a bc02 0000 6a60 0300 0029  ...ubj....j`...)
+00004210: 0300 0075 626a ba02 0000 6a60 0300 0029  ...ubj....j`...)
 00004220: 8194 7d94 286a 0303 0000 685c 6a04 0300  ..}.(j....h\j...
 00004230: 005d 946a 6503 0000 2981 947d 9428 6a03  .].je...)..}.(j.
 00004240: 0300 0068 5c6a 0403 0000 5d94 286a 6b03  ...h\j....].(jk.
 00004250: 0000 2981 947d 9428 6a03 0300 0068 5c6a  ..)..}.(j....h\j
 00004260: 0403 0000 5d94 6a70 0300 0029 8194 7d94  ....].jp...)..}.
 00004270: 286a 0303 0000 685c 6a04 0300 005d 946a  (j....h\j....].j
 00004280: 0703 0000 8c0c 496e 7374 616c 6c61 7469  ......Installati
 00004290: 6f6e 9485 9481 947d 946a 0c03 0000 6ab4  on.....}.j....j.
 000042a0: 0500 0073 6261 6a0d 0300 007d 9428 6a0f  ...sbaj....}.(j.
 000042b0: 0300 005d 946a 1103 0000 5d94 6a13 0300  ...].j....].j...
 000042c0: 005d 946a 1503 0000 5d94 6a17 0300 005d  .].j....].j....]
 000042d0: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
-000042e0: 6566 7572 6994 6abc 0200 008c 0a61 6e63  efuri.j......anc
+000042e0: 6566 7572 6994 6aba 0200 008c 0a61 6e63  efuri.j......anc
 000042f0: 686f 726e 616d 6594 685c 756a 1903 0000  horname.h\uj....
 00004300: 6a6f 0300 006a 0c03 0000 6ab1 0500 0075  jo...j....j....u
 00004310: 6261 6a0d 0300 007d 9428 6a0f 0300 005d  baj....}.(j....]
 00004320: 946a 1103 0000 5d94 6a13 0300 005d 946a  .j....].j....].j
 00004330: 1503 0000 5d94 6a17 0300 005d 9475 6a19  ....].j....].uj.
 00004340: 0300 006a 6a03 0000 6a0c 0300 006a ae05  ...jj...j....j..
 00004350: 0000 7562 6a60 0300 0029 8194 7d94 286a  ..ubj`...)..}.(j
@@ -1084,15 +1084,15 @@
 000043b0: 685c 6a04 0300 005d 946a 0703 0000 8c15  h\j....].j......
 000043c0: 5265 7175 6972 656d 656e 7473 2061 6e64  Requirements and
 000043d0: 2069 6e66 6f94 8594 8194 7d94 6a0c 0300   info.....}.j...
 000043e0: 006a d305 0000 7362 616a 0d03 0000 7d94  .j....sbaj....}.
 000043f0: 286a 0f03 0000 5d94 6a11 0300 005d 946a  (j....].j....].j
 00004400: 1303 0000 5d94 6a15 0300 005d 946a 1703  ....].j....].j..
 00004410: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
-00004420: 8c06 7265 6675 7269 946a bc02 0000 8c0a  ..refuri.j......
+00004420: 8c06 7265 6675 7269 946a ba02 0000 8c0a  ..refuri.j......
 00004430: 616e 6368 6f72 6e61 6d65 948c 1623 7265  anchorname...#re
 00004440: 7175 6972 656d 656e 7473 2d61 6e64 2d69  quirements-and-i
 00004450: 6e66 6f94 756a 1903 0000 6a6f 0300 006a  nfo.uj....jo...j
 00004460: 0c03 0000 6ad0 0500 0075 6261 6a0d 0300  ....j....ubaj...
 00004470: 007d 9428 6a0f 0300 005d 946a 1103 0000  .}.(j....].j....
 00004480: 5d94 6a13 0300 005d 946a 1503 0000 5d94  ].j....].j....].
 00004490: 6a17 0300 005d 9475 6a19 0300 006a 6a03  j....].uj....jj.
@@ -1107,15 +1107,15 @@
 00004520: 005d 946a 7003 0000 2981 947d 9428 6a03  .].jp...)..}.(j.
 00004530: 0300 0068 5c6a 0403 0000 5d94 6a07 0300  ...h\j....].j...
 00004540: 008c 0543 6c6f 6e65 9485 9481 947d 946a  ...Clone.....}.j
 00004550: 0c03 0000 6af6 0500 0073 6261 6a0d 0300  ....j....sbaj...
 00004560: 007d 9428 6a0f 0300 005d 946a 1103 0000  .}.(j....].j....
 00004570: 5d94 6a13 0300 005d 946a 1503 0000 5d94  ].j....].j....].
 00004580: 6a17 0300 005d 948c 0869 6e74 6572 6e61  j....]...interna
-00004590: 6c94 888c 0672 6566 7572 6994 6abc 0200  l....refuri.j...
+00004590: 6c94 888c 0672 6566 7572 6994 6aba 0200  l....refuri.j...
 000045a0: 008c 0a61 6e63 686f 726e 616d 6594 8c06  ...anchorname...
 000045b0: 2363 6c6f 6e65 9475 6a19 0300 006a 6f03  #clone.uj....jo.
 000045c0: 0000 6a0c 0300 006a f305 0000 7562 616a  ..j....j....ubaj
 000045d0: 0d03 0000 7d94 286a 0f03 0000 5d94 6a11  ....}.(j....].j.
 000045e0: 0300 005d 946a 1303 0000 5d94 6a15 0300  ...].j....].j...
 000045f0: 005d 946a 1703 0000 5d94 756a 1903 0000  .].j....].uj....
 00004600: 6a6a 0300 006a 0c03 0000 6af0 0500 0075  jj...j....j....u
@@ -1130,15 +1130,15 @@
 00004690: 286a 0303 0000 685c 6a04 0300 005d 946a  (j....h\j....].j
 000046a0: 0703 0000 8c0d 436f 6e66 6967 7572 6174  ......Configurat
 000046b0: 696f 6e94 8594 8194 7d94 6a0c 0300 006a  ion.....}.j....j
 000046c0: 1906 0000 7362 616a 0d03 0000 7d94 286a  ....sbaj....}.(j
 000046d0: 0f03 0000 5d94 6a11 0300 005d 946a 1303  ....].j....].j..
 000046e0: 0000 5d94 6a15 0300 005d 946a 1703 0000  ..].j....].j....
 000046f0: 5d94 8c08 696e 7465 726e 616c 9488 8c06  ]...internal....
-00004700: 7265 6675 7269 946a bc02 0000 8c0a 616e  refuri.j......an
+00004700: 7265 6675 7269 946a ba02 0000 8c0a 616e  refuri.j......an
 00004710: 6368 6f72 6e61 6d65 948c 0e23 636f 6e66  chorname...#conf
 00004720: 6967 7572 6174 696f 6e94 756a 1903 0000  iguration.uj....
 00004730: 6a6f 0300 006a 0c03 0000 6a16 0600 0075  jo...j....j....u
 00004740: 6261 6a0d 0300 007d 9428 6a0f 0300 005d  baj....}.(j....]
 00004750: 946a 1103 0000 5d94 6a13 0300 005d 946a  .j....].j....].j
 00004760: 1503 0000 5d94 6a17 0300 005d 9475 6a19  ....].j....].uj.
 00004770: 0300 006a 6a03 0000 6a0c 0300 006a 1306  ...jj...j....j..
@@ -1153,15 +1153,15 @@
 00004800: 8194 7d94 286a 0303 0000 685c 6a04 0300  ..}.(j....h\j...
 00004810: 005d 946a 0703 0000 8c0c 496e 7374 616c  .].j......Instal
 00004820: 6c61 7469 6f6e 9485 9481 947d 946a 0c03  lation.....}.j..
 00004830: 0000 6a3c 0600 0073 6261 6a0d 0300 007d  ..j<...sbaj....}
 00004840: 9428 6a0f 0300 005d 946a 1103 0000 5d94  .(j....].j....].
 00004850: 6a13 0300 005d 946a 1503 0000 5d94 6a17  j....].j....].j.
 00004860: 0300 005d 948c 0869 6e74 6572 6e61 6c94  ...]...internal.
-00004870: 888c 0672 6566 7572 6994 6abc 0200 008c  ...refuri.j.....
+00004870: 888c 0672 6566 7572 6994 6aba 0200 008c  ...refuri.j.....
 00004880: 0a61 6e63 686f 726e 616d 6594 8c04 2369  .anchorname...#i
 00004890: 6431 9475 6a19 0300 006a 6f03 0000 6a0c  d1.uj....jo...j.
 000048a0: 0300 006a 3906 0000 7562 616a 0d03 0000  ...j9...ubaj....
 000048b0: 7d94 286a 0f03 0000 5d94 6a11 0300 005d  }.(j....].j....]
 000048c0: 946a 1303 0000 5d94 6a15 0300 005d 946a  .j....].j....].j
 000048d0: 1703 0000 5d94 756a 1903 0000 6a6a 0300  ....].uj....jj..
 000048e0: 006a 0c03 0000 6a36 0600 0075 626a 6003  .j....j6...ubj`.
@@ -1173,15 +1173,15 @@
 00004940: 8194 7d94 286a 0303 0000 685c 6a04 0300  ..}.(j....h\j...
 00004950: 005d 946a 0703 0000 8c0d 5175 6963 6b20  .].j......Quick 
 00004960: 696e 7374 616c 6c94 8594 8194 7d94 6a0c  install.....}.j.
 00004970: 0300 006a 5c06 0000 7362 616a 0d03 0000  ...j\...sbaj....
 00004980: 7d94 286a 0f03 0000 5d94 6a11 0300 005d  }.(j....].j....]
 00004990: 946a 1303 0000 5d94 6a15 0300 005d 946a  .j....].j....].j
 000049a0: 1703 0000 5d94 8c08 696e 7465 726e 616c  ....]...internal
-000049b0: 9488 8c06 7265 6675 7269 946a bc02 0000  ....refuri.j....
+000049b0: 9488 8c06 7265 6675 7269 946a ba02 0000  ....refuri.j....
 000049c0: 8c0a 616e 6368 6f72 6e61 6d65 948c 0e23  ..anchorname...#
 000049d0: 7175 6963 6b2d 696e 7374 616c 6c94 756a  quick-install.uj
 000049e0: 1903 0000 6a6f 0300 006a 0c03 0000 6a59  ....jo...j....jY
 000049f0: 0600 0075 6261 6a0d 0300 007d 9428 6a0f  ...ubaj....}.(j.
 00004a00: 0300 005d 946a 1103 0000 5d94 6a13 0300  ...].j....].j...
 00004a10: 005d 946a 1503 0000 5d94 6a17 0300 005d  .].j....].j....]
 00004a20: 9475 6a19 0300 006a 6a03 0000 6a0c 0300  .uj....jj...j...
@@ -1195,15 +1195,15 @@
 00004aa0: 0000 8c1c 446f 636b 6572 2043 6f6d 706f  ....Docker Compo
 00004ab0: 7365 2028 7265 636f 6d6d 656e 6465 6429  se (recommended)
 00004ac0: 9485 9481 947d 946a 0c03 0000 6a7c 0600  .....}.j....j|..
 00004ad0: 0073 6261 6a0d 0300 007d 9428 6a0f 0300  .sbaj....}.(j...
 00004ae0: 005d 946a 1103 0000 5d94 6a13 0300 005d  .].j....].j....]
 00004af0: 946a 1503 0000 5d94 6a17 0300 005d 948c  .j....].j....]..
 00004b00: 0869 6e74 6572 6e61 6c94 888c 0672 6566  .internal....ref
-00004b10: 7572 6994 6abc 0200 008c 0a61 6e63 686f  uri.j......ancho
+00004b10: 7572 6994 6aba 0200 008c 0a61 6e63 686f  uri.j......ancho
 00004b20: 726e 616d 6594 8c1b 2364 6f63 6b65 722d  rname...#docker-
 00004b30: 636f 6d70 6f73 652d 7265 636f 6d6d 656e  compose-recommen
 00004b40: 6465 6494 756a 1903 0000 6a6f 0300 006a  ded.uj....jo...j
 00004b50: 0c03 0000 6a79 0600 0075 6261 6a0d 0300  ....jy...ubaj...
 00004b60: 007d 9428 6a0f 0300 005d 946a 1103 0000  .}.(j....].j....
 00004b70: 5d94 6a13 0300 005d 946a 1503 0000 5d94  ].j....].j....].
 00004b80: 6a17 0300 005d 9475 6a19 0300 006a 6a03  j....].uj....jj.
@@ -1219,15 +1219,15 @@
 00004c20: 0300 0068 5c6a 0403 0000 5d94 6a07 0300  ...h\j....].j...
 00004c30: 008c 0a56 6972 7475 616c 656e 7694 8594  ...Virtualenv...
 00004c40: 8194 7d94 6a0c 0300 006a 9f06 0000 7362  ..}.j....j....sb
 00004c50: 616a 0d03 0000 7d94 286a 0f03 0000 5d94  aj....}.(j....].
 00004c60: 6a11 0300 005d 946a 1303 0000 5d94 6a15  j....].j....].j.
 00004c70: 0300 005d 946a 1703 0000 5d94 8c08 696e  ...].j....]...in
 00004c80: 7465 726e 616c 9488 8c06 7265 6675 7269  ternal....refuri
-00004c90: 946a bc02 0000 8c0a 616e 6368 6f72 6e61  .j......anchorna
+00004c90: 946a ba02 0000 8c0a 616e 6368 6f72 6e61  .j......anchorna
 00004ca0: 6d65 948c 0423 6964 3294 756a 1903 0000  me...#id2.uj....
 00004cb0: 6a6f 0300 006a 0c03 0000 6a9c 0600 0075  jo...j....j....u
 00004cc0: 6261 6a0d 0300 007d 9428 6a0f 0300 005d  baj....}.(j....]
 00004cd0: 946a 1103 0000 5d94 6a13 0300 005d 946a  .j....].j....].j
 00004ce0: 1503 0000 5d94 6a17 0300 005d 9475 6a19  ....].j....].uj.
 00004cf0: 0300 006a 6a03 0000 6a0c 0300 006a 9906  ...jj...j....j..
 00004d00: 0000 7562 616a 0d03 0000 7d94 286a 0f03  ..ubaj....}.(j..
@@ -1250,15 +1250,15 @@
 00004e10: 685c 6a04 0300 005d 946a 0703 0000 8c12  h\j....].j......
 00004e20: 5072 6f64 7563 7469 6f6e 2069 6e73 7461  Production insta
 00004e30: 6c6c 9485 9481 947d 946a 0c03 0000 6ace  ll.....}.j....j.
 00004e40: 0600 0073 6261 6a0d 0300 007d 9428 6a0f  ...sbaj....}.(j.
 00004e50: 0300 005d 946a 1103 0000 5d94 6a13 0300  ...].j....].j...
 00004e60: 005d 946a 1503 0000 5d94 6a17 0300 005d  .].j....].j....]
 00004e70: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
-00004e80: 6566 7572 6994 6abc 0200 008c 0a61 6e63  efuri.j......anc
+00004e80: 6566 7572 6994 6aba 0200 008c 0a61 6e63  efuri.j......anc
 00004e90: 686f 726e 616d 6594 8c13 2370 726f 6475  horname...#produ
 00004ea0: 6374 696f 6e2d 696e 7374 616c 6c94 756a  ction-install.uj
 00004eb0: 1903 0000 6a6f 0300 006a 0c03 0000 6acb  ....jo...j....j.
 00004ec0: 0600 0075 6261 6a0d 0300 007d 9428 6a0f  ...ubaj....}.(j.
 00004ed0: 0300 005d 946a 1103 0000 5d94 6a13 0300  ...].j....].j...
 00004ee0: 005d 946a 1503 0000 5d94 6a17 0300 005d  .].j....].j....]
 00004ef0: 9475 6a19 0300 006a 6a03 0000 6a0c 0300  .uj....jj...j...
@@ -1271,15 +1271,15 @@
 00004f60: 0300 0068 5c6a 0403 0000 5d94 6a07 0300  ...h\j....].j...
 00004f70: 008c 0847 756e 6963 6f72 6e94 8594 8194  ...Gunicorn.....
 00004f80: 7d94 6a0c 0300 006a ee06 0000 7362 616a  }.j....j....sbaj
 00004f90: 0d03 0000 7d94 286a 0f03 0000 5d94 6a11  ....}.(j....].j.
 00004fa0: 0300 005d 946a 1303 0000 5d94 6a15 0300  ...].j....].j...
 00004fb0: 005d 946a 1703 0000 5d94 8c08 696e 7465  .].j....]...inte
 00004fc0: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
-00004fd0: bc02 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
+00004fd0: ba02 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
 00004fe0: 948c 0923 6775 6e69 636f 726e 9475 6a19  ...#gunicorn.uj.
 00004ff0: 0300 006a 6f03 0000 6a0c 0300 006a eb06  ...jo...j....j..
 00005000: 0000 7562 616a 0d03 0000 7d94 286a 0f03  ..ubaj....}.(j..
 00005010: 0000 5d94 6a11 0300 005d 946a 1303 0000  ..].j....].j....
 00005020: 5d94 6a15 0300 005d 946a 1703 0000 5d94  ].j....].j....].
 00005030: 756a 1903 0000 6a6a 0300 006a 0c03 0000  uj....jj...j....
 00005040: 6ae8 0600 0075 6261 6a0d 0300 007d 9428  j....ubaj....}.(
@@ -1477,16 +1477,16 @@
 00005c40: 1503 0000 5d94 6a17 0300 005d 9475 6a19  ....].j....].uj.
 00005c50: 0300 006a 6403 0000 6a0c 0300 006a af07  ...jd...j....j..
 00005c60: 0000 7562 616a 0d03 0000 7d94 286a 0f03  ..ubaj....}.(j..
 00005c70: 0000 5d94 6a11 0300 005d 946a 1303 0000  ..].j....].j....
 00005c80: 5d94 6a15 0300 005d 946a 1703 0000 5d94  ].j....].j....].
 00005c90: 756a 1903 0000 6a5f 0300 0075 6275 8c0f  uj....j_...ubu..
 00005ca0: 746f 635f 6e75 6d5f 656e 7472 6965 7394  toc_num_entries.
-00005cb0: 7d94 286a bb02 0000 4b03 6aba 0200 004b  }.(j....K.j....K
-00005cc0: 0a6a bf02 0000 4b01 6abc 0200 004b 0a6a  .j....K.j....K.j
+00005cb0: 7d94 286a bb02 0000 4b03 6abc 0200 004b  }.(j....K.j....K
+00005cc0: 0a6a bf02 0000 4b01 6aba 0200 004b 0a6a  .j....K.j....K.j
 00005cd0: be02 0000 4b03 6abd 0200 004b 0375 8c0e  ....K.j....K.u..
 00005ce0: 746f 635f 7365 636e 756d 6265 7273 947d  toc_secnumbers.}
 00005cf0: 948c 0e74 6f63 5f66 6967 6e75 6d62 6572  ...toc_fignumber
 00005d00: 7394 7d94 8c10 746f 6374 7265 655f 696e  s.}...toctree_in
 00005d10: 636c 7564 6573 947d 946a bf02 0000 5d94  cludes.}.j....].
 00005d20: 286a 8105 0000 6a83 0500 006a 8505 0000  (j....j....j....
 00005d30: 6a87 0500 006a 8905 0000 6573 8c10 6669  j....j....es..fi
@@ -1523,23 +1523,23 @@
 00005f20: 7094 4e8c 0e74 656d 706c 6174 6550 6172  p.N..templatePar
 00005f30: 616d 7394 4e8c 0c74 656d 706c 6174 6541  ams.N..templateA
 00005f40: 7267 7394 4e6a 4908 0000 4e6a 4a08 0000  rgs.NjI...NjJ...
 00005f50: 4e6a 9805 0000 4e6a 4b08 0000 896a 4c08  Nj....NjK....jL.
 00005f60: 0000 5d94 6a4e 0800 005d 9475 626a 1303  ..].jN...].ubj..
 00005f70: 0000 7d94 681d 4b00 7568 747d 9428 681d  ..}.h.K.uht}.(h.
 00005f80: 4b00 8c07 656e 7472 6965 7394 7d94 286a  K...entries.}.(j
-00005f90: bb02 0000 5d94 6aba 0200 005d 946a bf02  ....].j....].j..
-00005fa0: 0000 5d94 6abc 0200 005d 946a be02 0000  ..].j....].j....
+00005f90: bb02 0000 5d94 6abc 0200 005d 946a bf02  ....].j....].j..
+00005fa0: 0000 5d94 6aba 0200 005d 946a be02 0000  ..].j....].j....
 00005fb0: 5d94 6abd 0200 005d 9475 758c 026a 7394  ].j....].uu..js.
 00005fc0: 7d94 286a 5008 0000 7d94 8c07 6d6f 6475  }.(jP...}...modu
 00005fd0: 6c65 7394 7d94 681d 4b00 758c 046d 6174  les.}.h.K.u..mat
 00005fe0: 6894 7d94 286a 5008 0000 7d94 8c0d 6861  h.}.(jP...}...ha
 00005ff0: 735f 6571 7561 7469 6f6e 7394 7d94 286a  s_equations.}.(j
-00006000: bb02 0000 896a ba02 0000 896a bf02 0000  .....j.....j....
-00006010: 896a bc02 0000 896a be02 0000 896a bd02  .j.....j.....j..
+00006000: bb02 0000 896a bc02 0000 896a bf02 0000  .....j.....j....
+00006010: 896a ba02 0000 896a be02 0000 896a bd02  .j.....j.....j..
 00006020: 0000 8975 681d 4b00 7568 a97d 9428 6a50  ...uh.K.uh.}.(jP
 00006030: 0800 007d 946a 7308 0000 7d94 681d 4b00  ...}.js...}.h.K.
 00006040: 758c 0372 7374 947d 9428 6a50 0800 007d  u..rst.}.(jP...}
 00006050: 9468 1d4b 0075 8c03 7374 6494 7d94 288c  .h.K.u..std.}.(.
 00006060: 0b70 726f 676f 7074 696f 6e73 947d 946a  .progoptions.}.j
 00006070: 5008 0000 7d94 8c06 6c61 6265 6c73 947d  P...}...labels.}
 00006080: 9428 8c08 6765 6e69 6e64 6578 946a 8708  .(..genindex.j..
```

### Comparing `satnogs-network-1.98/docs/_build/html/.doctrees/index.doctree` & `satnogs-network-1.99/docs/_build/html/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/.doctrees/installation.doctree` & `satnogs-network-1.99/docs/_build/html/.doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/.doctrees/maintenance.doctree` & `satnogs-network-1.99/docs/_build/html/.doctrees/maintenance.doctree`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/.doctrees/releasing.doctree` & `satnogs-network-1.99/docs/_build/html/.doctrees/releasing.doctree`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_sources/developer-guide.rst.txt` & `satnogs-network-1.99/docs/_build/html/_sources/developer-guide.rst.txt`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_sources/installation.rst.txt` & `satnogs-network-1.99/docs/_build/html/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_sources/maintenance.rst.txt` & `satnogs-network-1.99/docs/_build/html/_sources/maintenance.rst.txt`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_sources/releasing.rst.txt` & `satnogs-network-1.99/docs/_build/html/_sources/releasing.rst.txt`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `satnogs-network-1.99/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/basic.css` & `satnogs-network-1.99/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/badge_only.css` & `satnogs-network-1.99/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-bold.woff` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-normal.woff` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `satnogs-network-1.99/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/css/theme.css` & `satnogs-network-1.99/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/doctools.js` & `satnogs-network-1.99/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/jquery-3.6.0.js` & `satnogs-network-1.99/docs/_build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/jquery.js` & `satnogs-network-1.99/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/js/badge_only.js` & `satnogs-network-1.99/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `satnogs-network-1.99/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/js/html5shiv.min.js` & `satnogs-network-1.99/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/js/theme.js` & `satnogs-network-1.99/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/language_data.js` & `satnogs-network-1.99/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/pygments.css` & `satnogs-network-1.99/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/searchtools.js` & `satnogs-network-1.99/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/sphinx_highlight.js` & `satnogs-network-1.99/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/underscore-1.13.1.js` & `satnogs-network-1.99/docs/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/_static/underscore.js` & `satnogs-network-1.99/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/_build/html/api.html` & `satnogs-network-1.99/docs/_build/html/api.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   
-  <title>API &mdash; SatNOGS Network 1.98 documentation</title>
+  <title>API &mdash; SatNOGS Network 1.99 documentation</title>
   
 
   
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
@@ -64,15 +64,15 @@
           
           </a>
 
           
             
             
               <div class="version">
-                1.98
+                1.99
               </div>
             
           
 
           
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
```

### Comparing `satnogs-network-1.98/docs/_build/html/developer-guide.html` & `satnogs-network-1.99/docs/_build/html/developer-guide.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   
-  <title>Developer Guide &mdash; SatNOGS Network 1.98 documentation</title>
+  <title>Developer Guide &mdash; SatNOGS Network 1.99 documentation</title>
   
 
   
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
@@ -65,15 +65,15 @@
           
           </a>
 
           
             
             
               <div class="version">
-                1.98
+                1.99
               </div>
             
           
 
           
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 
 
 
 
 
 
 SatNOGS_Network
-1.98
+1.99
 [q                   ]
     * Installation
     * Developer_Guide
           o Workflow
           o Templates
           o Frontend_development
           o Backend_development
```

### Comparing `satnogs-network-1.98/docs/_build/html/genindex.html` & `satnogs-network-1.99/docs/_build/html/genindex.html`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   
-  <title>Index &mdash; SatNOGS Network 1.98 documentation</title>
+  <title>Index &mdash; SatNOGS Network 1.99 documentation</title>
   
 
   
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
@@ -62,15 +62,15 @@
           
           </a>
 
           
             
             
               <div class="version">
-                1.98
+                1.99
               </div>
             
           
 
           
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
```

### Comparing `satnogs-network-1.98/docs/_build/html/index.html` & `satnogs-network-1.99/docs/_build/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   
-  <title>satnogs-network &mdash; SatNOGS Network 1.98 documentation</title>
+  <title>satnogs-network &mdash; SatNOGS Network 1.99 documentation</title>
   
 
   
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
@@ -64,15 +64,15 @@
           
           </a>
 
           
             
             
               <div class="version">
-                1.98
+                1.99
               </div>
             
           
 
           
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
```

### Comparing `satnogs-network-1.98/docs/_build/html/installation.html` & `satnogs-network-1.99/docs/_build/html/installation.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   
-  <title>Installation &mdash; SatNOGS Network 1.98 documentation</title>
+  <title>Installation &mdash; SatNOGS Network 1.99 documentation</title>
   
 
   
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
@@ -65,15 +65,15 @@
           
           </a>
 
           
             
             
               <div class="version">
-                1.98
+                1.99
               </div>
             
           
 
           
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 
 
 
 
 
 
 SatNOGS_Network
-1.98
+1.99
 [q                   ]
     * Installation
           o Requirements_and_info
           o Clone
           o Configuration
           o Installation
                 # Quick_install
```

### Comparing `satnogs-network-1.98/docs/_build/html/maintenance.html` & `satnogs-network-1.99/docs/_build/html/maintenance.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   
-  <title>Maintenance &mdash; SatNOGS Network 1.98 documentation</title>
+  <title>Maintenance &mdash; SatNOGS Network 1.99 documentation</title>
   
 
   
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
@@ -65,15 +65,15 @@
           
           </a>
 
           
             
             
               <div class="version">
-                1.98
+                1.99
               </div>
             
           
 
           
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
```

### Comparing `satnogs-network-1.98/docs/_build/html/releasing.html` & `satnogs-network-1.99/docs/_build/html/releasing.html`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   
-  <title>Releasing &mdash; SatNOGS Network 1.98 documentation</title>
+  <title>Releasing &mdash; SatNOGS Network 1.99 documentation</title>
   
 
   
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
@@ -65,15 +65,15 @@
           
           </a>
 
           
             
             
               <div class="version">
-                1.98
+                1.99
               </div>
             
           
 
           
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
```

### Comparing `satnogs-network-1.98/docs/_build/html/search.html` & `satnogs-network-1.99/docs/_build/html/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   
-  <title>Search &mdash; SatNOGS Network 1.98 documentation</title>
+  <title>Search &mdash; SatNOGS Network 1.99 documentation</title>
   
 
   
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
   <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
@@ -65,15 +65,15 @@
           
           </a>
 
           
             
             
               <div class="version">
-                1.98
+                1.99
               </div>
             
           
 
           
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
```

### Comparing `satnogs-network-1.98/docs/_build/html/searchindex.js` & `satnogs-network-1.99/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/conf.py` & `satnogs-network-1.99/docs/conf.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/developer-guide.rst` & `satnogs-network-1.99/docs/developer-guide.rst`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/installation.rst` & `satnogs-network-1.99/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/maintenance.rst` & `satnogs-network-1.99/docs/maintenance.rst`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/releasing.rst` & `satnogs-network-1.99/docs/releasing.rst`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/docs/versioneer.py` & `satnogs-network-1.99/docs/versioneer.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/api/authentication.py` & `satnogs-network-1.99/network/api/authentication.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/api/filters.py` & `satnogs-network-1.99/network/api/filters.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/api/pagination.py` & `satnogs-network-1.99/network/api/pagination.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/api/perms.py` & `satnogs-network-1.99/network/api/perms.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/api/serializers.py` & `satnogs-network-1.99/network/api/serializers.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/api/tests.py` & `satnogs-network-1.99/network/api/tests.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/api/urls.py` & `satnogs-network-1.99/network/api/urls.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/api/views.py` & `satnogs-network-1.99/network/api/views.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/admin.py` & `satnogs-network-1.99/network/base/admin.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/context_processors.py` & `satnogs-network-1.99/network/base/context_processors.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/db_api.py` & `satnogs-network-1.99/network/base/db_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/decorators.py` & `satnogs-network-1.99/network/base/decorators.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/forms.py` & `satnogs-network-1.99/network/base/forms.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/management/commands/fetch_data.py` & `satnogs-network-1.99/network/base/management/commands/fetch_data.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/management/commands/initialize.py` & `satnogs-network-1.99/network/base/management/commands/initialize.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/management/commands/update_station_last_seen.py` & `satnogs-network-1.99/network/base/management/commands/update_station_last_seen.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0001_initial.py` & `satnogs-network-1.99/network/base/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0003_auto_20160119_1856.py` & `satnogs-network-1.99/network/base/migrations/0003_auto_20160119_1856.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0005_auto_20160320_1619.py` & `satnogs-network-1.99/network/base/migrations/0005_auto_20160320_1619.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0006_auto_20160325_0126.py` & `satnogs-network-1.99/network/base/migrations/0006_auto_20160325_0126.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0010_auto_20160507_1550.py` & `satnogs-network-1.99/network/base/migrations/0010_auto_20160507_1550.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0012_auto_20160508_1516.py` & `satnogs-network-1.99/network/base/migrations/0012_auto_20160508_1516.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0014_auto_20170205_0059.py` & `satnogs-network-1.99/network/base/migrations/0014_auto_20170205_0059.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0015_auto_20170304_2041.py` & `satnogs-network-1.99/network/base/migrations/0015_auto_20170304_2041.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0016_antenna_frequency_max.py` & `satnogs-network-1.99/network/base/migrations/0016_antenna_frequency_max.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0017_auto_20170321_1046.py` & `satnogs-network-1.99/network/base/migrations/0017_auto_20170321_1046.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0018_auto_20170519_1955.py` & `satnogs-network-1.99/network/base/migrations/0018_auto_20170519_1955.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0022_auto_20170909_2103.py` & `satnogs-network-1.99/network/base/migrations/0022_auto_20170909_2103.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0023_auto_20170909_2103.py` & `satnogs-network-1.99/network/base/migrations/0023_auto_20170909_2103.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0025_auto_20170909_2111.py` & `satnogs-network-1.99/network/base/migrations/0025_auto_20170909_2111.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0026_auto_20170909_2116.py` & `satnogs-network-1.99/network/base/migrations/0026_auto_20170909_2116.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0027_create_moderators_group.py` & `satnogs-network-1.99/network/base/migrations/0027_create_moderators_group.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0028_auto_20171127_2154.py` & `satnogs-network-1.99/network/base/migrations/0028_auto_20171127_2154.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0029_auto_20171216_1712.py` & `satnogs-network-1.99/network/base/migrations/0029_auto_20171216_1712.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0030_auto_20171224_1701.py` & `satnogs-network-1.99/network/base/migrations/0030_auto_20171224_1701.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0031_migrate_vetted.py` & `satnogs-network-1.99/network/base/migrations/0031_migrate_vetted.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0033_auto_20171228_1515.py` & `satnogs-network-1.99/network/base/migrations/0033_auto_20171228_1515.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0034_auto_20180202_1358.py` & `satnogs-network-1.99/network/base/migrations/0034_auto_20180202_1358.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0036_auto_20180316_1216.py` & `satnogs-network-1.99/network/base/migrations/0036_auto_20180316_1216.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0037_stationstatuslog.py` & `satnogs-network-1.99/network/base/migrations/0037_stationstatuslog.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0038_auto_20180322_2054.py` & `satnogs-network-1.99/network/base/migrations/0038_auto_20180322_2054.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0041_auto_20180812_0915.py` & `satnogs-network-1.99/network/base/migrations/0041_auto_20180812_0915.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0043_auto_20180817_0923.py` & `satnogs-network-1.99/network/base/migrations/0043_auto_20180817_0923.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0044_auto_20180817_1351.py` & `satnogs-network-1.99/network/base/migrations/0044_auto_20180817_1351.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0045_auto_20180822_1947.py` & `satnogs-network-1.99/network/base/migrations/0045_auto_20180822_1947.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0048_auto_20180902_2217.py` & `satnogs-network-1.99/network/base/migrations/0048_auto_20180902_2217.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0049_auto_20180915_1503.py` & `satnogs-network-1.99/network/base/migrations/0049_auto_20180915_1503.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0052_auto_20181230_2113.py` & `satnogs-network-1.99/network/base/migrations/0052_auto_20181230_2113.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0054_station_target_utilization.py` & `satnogs-network-1.99/network/base/migrations/0054_station_target_utilization.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0055_add_new_antenna_type.py` & `satnogs-network-1.99/network/base/migrations/0055_add_new_antenna_type.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0057_no_null_demoddata_observation_field.py` & `satnogs-network-1.99/network/base/migrations/0057_no_null_demoddata_observation_field.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0058_add_transmitter_into_observation_model.py` & `satnogs-network-1.99/network/base/migrations/0058_add_transmitter_into_observation_model.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0059_remove_mode_model.py` & `satnogs-network-1.99/network/base/migrations/0059_remove_mode_model.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0061_create_indexes.py` & `satnogs-network-1.99/network/base/migrations/0061_create_indexes.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0065_new_antenna_schema.py` & `satnogs-network-1.99/network/base/migrations/0065_new_antenna_schema.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0066_move_data_from_old_to_new_antenna_schema.py` & `satnogs-network-1.99/network/base/migrations/0066_move_data_from_old_to_new_antenna_schema.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0067_fix_station_fields.py` & `satnogs-network-1.99/network/base/migrations/0067_fix_station_fields.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0069_increase_range_frequency_limits.py` & `satnogs-network-1.99/network/base/migrations/0069_increase_range_frequency_limits.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0072_change_station_antennas_related_name.py` & `satnogs-network-1.99/network/base/migrations/0072_change_station_antennas_related_name.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0073_add_observation_status.py` & `satnogs-network-1.99/network/base/migrations/0073_add_observation_status.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0074_add_waterfall_status.py` & `satnogs-network-1.99/network/base/migrations/0074_add_waterfall_status.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0075_add_waterfall_status_details.py` & `satnogs-network-1.99/network/base/migrations/0075_add_waterfall_status_details.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0076_add_waterfalls_vetted_related_name.py` & `satnogs-network-1.99/network/base/migrations/0076_add_waterfalls_vetted_related_name.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0078_fix_waterfall_status.py` & `satnogs-network-1.99/network/base/migrations/0078_fix_waterfall_status.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0079_add_tle_field_in_observation_model.py` & `satnogs-network-1.99/network/base/migrations/0079_add_tle_field_in_observation_model.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0080_add_future_status.py` & `satnogs-network-1.99/network/base/migrations/0080_add_future_status.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0081_remove_tle_model.py` & `satnogs-network-1.99/network/base/migrations/0081_remove_tle_model.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0083_add_station_fields_in_observation.py` & `satnogs-network-1.99/network/base/migrations/0083_add_station_fields_in_observation.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0085_add_audio_zipped_field_in_observation.py` & `satnogs-network-1.99/network/base/migrations/0085_add_audio_zipped_field_in_observation.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0086_add_index_to_observation_fields.py` & `satnogs-network-1.99/network/base/migrations/0086_add_index_to_observation_fields.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0087_remove_low_cardinality_indexes_from_observation_fields.py` & `satnogs-network-1.99/network/base/migrations/0087_remove_low_cardinality_indexes_from_observation_fields.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0088_allow_blank_value_on_station_fields_of_observations.py` & `satnogs-network-1.99/network/base/migrations/0088_allow_blank_value_on_station_fields_of_observations.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0091_filefields_for_s3_storage.py` & `satnogs-network-1.99/network/base/migrations/0091_filefields_for_s3_storage.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0093_check_old_demoddata_if_are_images.py` & `satnogs-network-1.99/network/base/migrations/0093_check_old_demoddata_if_are_images.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0094_migrate_artifact_files_from_old_to_new_fields.py` & `satnogs-network-1.99/network/base/migrations/0094_migrate_artifact_files_from_old_to_new_fields.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0098_create_operators_group.py` & `satnogs-network-1.99/network/base/migrations/0098_create_operators_group.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0099_add_basic_client_configuration_in_station_model.py` & `satnogs-network-1.99/network/base/migrations/0099_add_basic_client_configuration_in_station_model.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/migrations/0101_allow_null_alt_lat_lng_fields_in_station_model.py` & `satnogs-network-1.99/network/base/migrations/0101_allow_null_alt_lat_lng_fields_in_station_model.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/models.py` & `satnogs-network-1.99/network/base/models.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/perms.py` & `satnogs-network-1.99/network/base/perms.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/rating_tasks.py` & `satnogs-network-1.99/network/base/rating_tasks.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/scheduling.py` & `satnogs-network-1.99/network/base/scheduling.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/serializers.py` & `satnogs-network-1.99/network/base/serializers.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/signals.py` & `satnogs-network-1.99/network/base/signals.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/stats.py` & `satnogs-network-1.99/network/base/stats.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/tasks.py` & `satnogs-network-1.99/network/base/tasks.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/templatetags/paginator.py` & `satnogs-network-1.99/network/base/templatetags/paginator.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/templatetags/tags.py` & `satnogs-network-1.99/network/base/templatetags/tags.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/test_orbital.py` & `satnogs-network-1.99/network/base/test_orbital.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/test_utils.py` & `satnogs-network-1.99/network/base/test_utils.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/tests.py` & `satnogs-network-1.99/network/base/tests.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/urls.py` & `satnogs-network-1.99/network/base/urls.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/utils.py` & `satnogs-network-1.99/network/base/utils.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/validators.py` & `satnogs-network-1.99/network/base/validators.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/views/generic.py` & `satnogs-network-1.99/network/base/views/generic.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/views/observation.py` & `satnogs-network-1.99/network/base/views/observation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Django base views for SatNOGS Network"""
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required
-from django.db.models import Count
 from django.http import JsonResponse
 from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse
 from django.utils.timezone import now
 from django.views.generic import ListView
 
 from network.base.db_api import DBConnectionError, get_transmitters_by_norad_id
@@ -56,18 +55,17 @@
         Optionally filter based on future/good/bad/unknown/failed
         """
         filter_params = self.get_filter_params()
 
         results = self.request.GET.getlist('results')
         rated = self.request.GET.getlist('rated')
 
-        observations = Observation.objects.select_related('satellite', 'author',
-                                                          'ground_station').annotate(
-                                                              demoddata_count=Count('demoddata')
-                                                          ).order_by('-start', '-end')  # noqa
+        observations = Observation.objects.prefetch_related(
+            'satellite', 'demoddata', 'author', 'ground_station'
+        )
 
         # Mapping between the HTTP POST parameters and the fiter keys
         parameter_filter_mapping = {
             'norad': 'satellite__norad_cat_id',
             'observer': 'author',
             'station': 'ground_station_id',
             'start': 'start__gt',
```

### Comparing `satnogs-network-1.98/network/base/views/scheduling.py` & `satnogs-network-1.99/network/base/views/scheduling.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/base/views/station.py` & `satnogs-network-1.99/network/base/views/station.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/celery.py` & `satnogs-network-1.99/network/celery.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/settings.py` & `satnogs-network-1.99/network/settings.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/css/common/_custom.scss` & `satnogs-network-1.99/network/static/css/common/_custom.scss`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/css/common/_info.scss` & `satnogs-network-1.99/network/static/css/common/_info.scss`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/css/common/_status.scss` & `satnogs-network-1.99/network/static/css/common/_status.scss`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/css/pages/_home.scss` & `satnogs-network-1.99/network/static/css/pages/_home.scss`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/css/pages/_map_overrides.scss` & `satnogs-network-1.99/network/static/css/pages/_map_overrides.scss`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/css/pages/_observation.scss` & `satnogs-network-1.99/network/static/css/pages/_observation.scss`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/css/pages/_observations.scss` & `satnogs-network-1.99/network/static/css/pages/_observations.scss`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/css/pages/_satellites.scss` & `satnogs-network-1.99/network/static/css/pages/_satellites.scss`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/css/pages/_station_view.scss` & `satnogs-network-1.99/network/static/css/pages/_station_view.scss`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/css/pages/_stations.scss` & `satnogs-network-1.99/network/static/css/pages/_stations.scss`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/css/partials/_fonts.scss` & `satnogs-network-1.99/network/static/css/partials/_fonts.scss`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/css/partials/_mixins.scss` & `satnogs-network-1.99/network/static/css/partials/_mixins.scss`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/favicon.ico` & `satnogs-network-1.99/network/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-Bold.eot` & `satnogs-network-1.99/network/static/fonts/ClearSans-Bold.eot`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-Bold.svg` & `satnogs-network-1.99/network/static/fonts/ClearSans-Bold.svg`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-Bold.ttf` & `satnogs-network-1.99/network/static/fonts/ClearSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-Bold.woff` & `satnogs-network-1.99/network/static/fonts/ClearSans-Bold.woff`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-BoldItalic.eot` & `satnogs-network-1.99/network/static/fonts/ClearSans-BoldItalic.eot`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-BoldItalic.svg` & `satnogs-network-1.99/network/static/fonts/ClearSans-BoldItalic.svg`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-BoldItalic.ttf` & `satnogs-network-1.99/network/static/fonts/ClearSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-BoldItalic.woff` & `satnogs-network-1.99/network/static/fonts/ClearSans-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-Italic.eot` & `satnogs-network-1.99/network/static/fonts/ClearSans-Italic.eot`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-Italic.svg` & `satnogs-network-1.99/network/static/fonts/ClearSans-Italic.svg`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-Italic.ttf` & `satnogs-network-1.99/network/static/fonts/ClearSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-Italic.woff` & `satnogs-network-1.99/network/static/fonts/ClearSans-Italic.woff`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-Regular.eot` & `satnogs-network-1.99/network/static/fonts/ClearSans-Regular.eot`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-Regular.svg` & `satnogs-network-1.99/network/static/fonts/ClearSans-Regular.svg`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-Regular.ttf` & `satnogs-network-1.99/network/static/fonts/ClearSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/fonts/ClearSans-Regular.woff` & `satnogs-network-1.99/network/static/fonts/ClearSans-Regular.woff`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/html/502.html` & `satnogs-network-1.99/network/static/html/502.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/html/503.html` & `satnogs-network-1.99/network/static/html/503.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/html/504.html` & `satnogs-network-1.99/network/static/html/504.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/img/error.png` & `satnogs-network-1.99/network/static/img/error.png`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/img/ground_station_no_image.png` & `satnogs-network-1.99/network/static/img/ground_station_no_image.png`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/img/ground_station_test.jpg` & `satnogs-network-1.99/network/static/img/ground_station_test.jpg`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/img/offline.png` & `satnogs-network-1.99/network/static/img/offline.png`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/img/online.png` & `satnogs-network-1.99/network/static/img/online.png`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/img/pin.png` & `satnogs-network-1.99/network/static/img/pin.png`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/img/sat.png` & `satnogs-network-1.99/network/static/img/sat.png`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/img/satnogs-network-logo.png` & `satnogs-network-1.99/network/static/img/satnogs-network-logo.png`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/img/satnogs_net.png` & `satnogs-network-1.99/network/static/img/satnogs_net.png`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/img/testing.png` & `satnogs-network-1.99/network/static/img/testing.png`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/api-renew.js` & `satnogs-network-1.99/network/static/js/api-renew.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/app.js` & `satnogs-network-1.99/network/static/js/app.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/ax25monitor.js` & `satnogs-network-1.99/network/static/js/ax25monitor.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/frequency_utils.js` & `satnogs-network-1.99/network/static/js/frequency_utils.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/ga.js` & `satnogs-network-1.99/network/static/js/ga.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/gridsquare.js` & `satnogs-network-1.99/network/static/js/gridsquare.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/map.js` & `satnogs-network-1.99/network/static/js/map.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/observation_new.js` & `satnogs-network-1.99/network/static/js/observation_new.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/observation_view.js` & `satnogs-network-1.99/network/static/js/observation_view.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/observations.js` & `satnogs-network-1.99/network/static/js/observations.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/polar_svg.js` & `satnogs-network-1.99/network/static/js/polar_svg.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/satellite.js` & `satnogs-network-1.99/network/static/js/satellite.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/station_edit.js` & `satnogs-network-1.99/network/static/js/station_edit.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/station_register_step2.js` & `satnogs-network-1.99/network/static/js/station_register_step2.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/station_view.js` & `satnogs-network-1.99/network/static/js/station_view.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/js/stations.js` & `satnogs-network-1.99/network/static/js/stations.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/@eonasdan/tempus-dominus/dist/css/tempus-dominus.min.css` & `satnogs-network-1.99/network/static/lib/@eonasdan/tempus-dominus/dist/css/tempus-dominus.min.css`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/@eonasdan/tempus-dominus/dist/js/tempus-dominus.min.js` & `satnogs-network-1.99/network/static/lib/@eonasdan/tempus-dominus/dist/js/tempus-dominus.min.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/@eonasdan/tempus-dominus/dist/plugins/customDateFormat.js` & `satnogs-network-1.99/network/static/lib/@eonasdan/tempus-dominus/dist/plugins/customDateFormat.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/@popperjs/core/dist/umd/popper.min.js` & `satnogs-network-1.99/network/static/lib/@popperjs/core/dist/umd/popper.min.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/bootstrap/dist/css/bootstrap.min.css` & `satnogs-network-1.99/network/static/lib/bootstrap/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/bootstrap/dist/js/bootstrap.bundle.min.js` & `satnogs-network-1.99/network/static/lib/bootstrap/dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/bootstrap-fileinput/css/fileinput.min.css` & `satnogs-network-1.99/network/static/lib/bootstrap-fileinput/css/fileinput.min.css`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/bootstrap-fileinput/js/fileinput.min.js` & `satnogs-network-1.99/network/static/lib/bootstrap-fileinput/js/fileinput.min.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/bootstrap-icons/font/bootstrap-icons.css` & `satnogs-network-1.99/network/static/lib/bootstrap-icons/font/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/bootstrap-icons/font/fonts/bootstrap-icons.woff` & `satnogs-network-1.99/network/static/lib/bootstrap-icons/font/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/bootstrap-icons/font/fonts/bootstrap-icons.woff2` & `satnogs-network-1.99/network/static/lib/bootstrap-icons/font/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/bootstrap-select/dist/css/bootstrap-select.min.css` & `satnogs-network-1.99/network/static/lib/bootstrap-select/dist/css/bootstrap-select.min.css`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/bootstrap-select/dist/js/bootstrap-select.min.js` & `satnogs-network-1.99/network/static/lib/bootstrap-select/dist/js/bootstrap-select.min.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/bootstrap-slider/dist/bootstrap-slider.min.js` & `satnogs-network-1.99/network/static/lib/bootstrap-slider/dist/bootstrap-slider.min.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/bootstrap-slider/dist/css/bootstrap-slider.min.css` & `satnogs-network-1.99/network/static/lib/bootstrap-slider/dist/css/bootstrap-slider.min.css`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/d3/d3.min.js` & `satnogs-network-1.99/network/static/lib/d3/d3.min.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/d3-timeline/src/d3-timeline.js` & `satnogs-network-1.99/network/static/lib/d3-timeline/src/d3-timeline.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/dnt-helper/js/dnt-helper.js` & `satnogs-network-1.99/network/static/lib/dnt-helper/js/dnt-helper.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/jquery/dist/jquery.min.js` & `satnogs-network-1.99/network/static/lib/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/jquery.json-viewer/json-viewer/jquery.json-viewer.css` & `satnogs-network-1.99/network/static/lib/jquery.json-viewer/json-viewer/jquery.json-viewer.css`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/jquery.json-viewer/json-viewer/jquery.json-viewer.js` & `satnogs-network-1.99/network/static/lib/jquery.json-viewer/json-viewer/jquery.json-viewer.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/kaitai-struct/KaitaiStream.js` & `satnogs-network-1.99/network/static/lib/kaitai-struct/KaitaiStream.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/mapbox-gl/dist/mapbox-gl.css` & `satnogs-network-1.99/network/static/lib/mapbox-gl/dist/mapbox-gl.css`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/mapbox-gl/dist/mapbox-gl.js` & `satnogs-network-1.99/network/static/lib/mapbox-gl/dist/mapbox-gl.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/moment/min/moment.min.js` & `satnogs-network-1.99/network/static/lib/moment/min/moment.min.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/satellite.js/dist/satellite.min.js` & `satnogs-network-1.99/network/static/lib/satellite.js/dist/satellite.min.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/wavesurfer.js/dist/plugin/wavesurfer.spectrogram.min.js` & `satnogs-network-1.99/network/static/lib/wavesurfer.js/dist/plugin/wavesurfer.spectrogram.min.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/static/lib/wavesurfer.js/dist/wavesurfer.min.js` & `satnogs-network-1.99/network/static/lib/wavesurfer.js/dist/wavesurfer.min.js`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/account/email.html` & `satnogs-network-1.99/network/templates/account/email.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/account/email_confirm.html` & `satnogs-network-1.99/network/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/account/login.html` & `satnogs-network-1.99/network/templates/account/login.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/account/logout.html` & `satnogs-network-1.99/network/templates/account/logout.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/account/password_reset.html` & `satnogs-network-1.99/network/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/account/password_reset_from_key.html` & `satnogs-network-1.99/network/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/account/signup.html` & `satnogs-network-1.99/network/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/account/verification_sent.html` & `satnogs-network-1.99/network/templates/account/verification_sent.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/account/verified_email_required.html` & `satnogs-network-1.99/network/templates/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/base/about.html` & `satnogs-network-1.99/network/templates/base/about.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/base/home.html` & `satnogs-network-1.99/network/templates/base/home.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/base/observation_new.html` & `satnogs-network-1.99/network/templates/base/observation_new.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/base/observation_view.html` & `satnogs-network-1.99/network/templates/base/observation_view.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/base/observations.html` & `satnogs-network-1.99/network/templates/base/observations.html`

 * *Files 0% similar despite different names*

```diff
@@ -293,16 +293,16 @@
                         title="Waterfall uploaded"></span>
                 {% endif %}
                 {% if observation.has_audio %}
                   <span class="bi bi-volume-up-fill" aria-hidden="true"
                         data-toggle="tooltip" data-placement="bottom"
                         title="Audio uploaded"></span>
                 {% endif %}
-                {% if observation.demoddata_count > 0 %}
-                  {% with total_data=observation.demoddata_count %}
+                {% if observation.demoddata.exists %}
+                  {% with total_data=observation.demoddata.count %}
                     <span class="bi bi-file-earmark-fill" aria-hidden="true"
                           data-toggle="tooltip" data-placement="bottom"
                           title="{{ total_data }} Data uploaded"></span>
                     <span class="badge badge-data-count">{{ total_data }}</span>
                   {% endwith %}
                 {% endif %}
               </td>
```

#### html2text {}

```diff
@@ -55,17 +55,17 @@
 observation.status_<
 -100_%}_{
 {_observation.id_}}_                                                                                                                         {
 {%_elif                                                                                                                                     {
 observation.status_>=                                                                                                                       observation.start|date: {% if observation.has_waterfall %}  {%
 -100_and                                         {% if observation.center_frequency %} {   {{ observation.transmitter_mode|default:"-" }}   "Y-m-d" }} {            endif %} {% if observation.has_audio                                  {% if
 observation.status_<  {                          { observation.center_frequency|frq }} {% {                                                 {                       %}  {% endif %} {% if                  {% if observation.author %} {  observation.ground_station
-0_%}_{                {                          else %} {                                {                                                 observation.start|date: observation.demoddata_count > 0 %} {%  {                              %} {
+0_%}_{                {                          else %} {                                {                                                 observation.start|date: observation.demoddata.exists %} {%     {                              %} {
 {_observation.id_}}_  observation.satellite.name {                                        observation.transmitter_baud|floatformat|default: "H:i:s" }}              with                                   observation.author.displayname {
-{%_elif               }}                         observation.transmitter_downlink_low|frq "" }}                                               {                     total_data=observation.demoddata_count }} {% else %} - {% endif %}    observation.ground_station
+{%_elif               }}                         observation.transmitter_downlink_low|frq "" }}                                               {                     total_data=observation.demoddata.count }} {% else %} - {% endif %}    observation.ground_station
 observation.status_>=                            }} {% endif %}                                                                             { observation.end|date: %}  {{ total_data }} {% endwith %} {%                                 }} {% endif %}
 0_and                                                                                                                                       "Y-m-d" }} {            endif %}
 observation.status_<                                                                                                                        { observation.end|date:
 100_%}_{                                                                                                                                    "H:i:s" }}
 {_observation.id_}}_
 {%_elif
 observation.status_>=
```

### Comparing `satnogs-network-1.98/network/templates/base/paginator.html` & `satnogs-network-1.99/network/templates/base/paginator.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/base/settings_site.html` & `satnogs-network-1.99/network/templates/base/settings_site.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/base/station_edit.html` & `satnogs-network-1.99/network/templates/base/station_edit.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/base/station_register_step1.html` & `satnogs-network-1.99/network/templates/base/station_register_step1.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/base/station_register_step2.html` & `satnogs-network-1.99/network/templates/base/station_register_step2.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/base/station_view.html` & `satnogs-network-1.99/network/templates/base/station_view.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/base/stations.html` & `satnogs-network-1.99/network/templates/base/stations.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/base.html` & `satnogs-network-1.99/network/templates/base.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/includes/legend.html` & `satnogs-network-1.99/network/templates/includes/legend.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/includes/observation-hotkeys.html` & `satnogs-network-1.99/network/templates/includes/observation-hotkeys.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/includes/observation-new-hotkeys.html` & `satnogs-network-1.99/network/templates/includes/observation-new-hotkeys.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/includes/satellite.html` & `satnogs-network-1.99/network/templates/includes/satellite.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/users/user_detail.html` & `satnogs-network-1.99/network/templates/users/user_detail.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/templates/users/user_form.html` & `satnogs-network-1.99/network/templates/users/user_form.html`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/urls.py` & `satnogs-network-1.99/network/urls.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/users/admin.py` & `satnogs-network-1.99/network/users/admin.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/users/migrations/0001_squashed_0002_auto_20150415_1141.py` & `satnogs-network-1.99/network/users/migrations/0001_squashed_0002_auto_20150415_1141.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/users/migrations/0002_auto_20160123_0939.py` & `satnogs-network-1.99/network/users/migrations/0002_auto_20160123_0939.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/users/migrations/0003_auto_20160922_1505.py` & `satnogs-network-1.99/network/users/migrations/0003_auto_20160922_1505.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/users/migrations/0004_username_unicode_validator.py` & `satnogs-network-1.99/network/users/migrations/0004_username_unicode_validator.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/users/models.py` & `satnogs-network-1.99/network/users/models.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/users/tests.py` & `satnogs-network-1.99/network/users/tests.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/network/users/views.py` & `satnogs-network-1.99/network/users/views.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/satnogs_network.egg-info/PKG-INFO` & `satnogs-network-1.99/satnogs_network.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satnogs-network
-Version: 1.98
+Version: 1.99
 Summary: SatNOGS Network
 Home-page: https://gitlab.com/librespacefoundation/satnogs/satnogs-network
 Author: SatNOGS project
 Author-email: dev@satnogs.org
 License: AGPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `satnogs-network-1.98/satnogs_network.egg-info/SOURCES.txt` & `satnogs-network-1.99/satnogs_network.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/satnogs_network.egg-info/requires.txt` & `satnogs-network-1.99/satnogs_network.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/setup.cfg` & `satnogs-network-1.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `satnogs-network-1.98/versioneer.py` & `satnogs-network-1.99/versioneer.py`

 * *Files identical despite different names*

