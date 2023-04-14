# Comparing `tmp/django-dashboards-0.1.0.tar.gz` & `tmp/django-dashboards-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dashboards-0.1.0.tar", last modified: Fri Apr 14 14:12:18 2023, max compression
+gzip compressed data, was "django-dashboards-0.1.1.tar", last modified: Fri Apr 14 15:08:16 2023, max compression
```

## Comparing `django-dashboards-0.1.0.tar` & `django-dashboards-0.1.1.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.495064 django-dashboards-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-14 14:12:18.495064 django-dashboards-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.471064 django-dashboards-0.1.0/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.471064 django-dashboards-0.1.0/dashboards/component/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/component/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.471064 django-dashboards-0.1.0/dashboards/component/chart/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/component/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/component/chart/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/component/chart/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/component/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/component/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/component/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.471064 django-dashboards-0.1.0/dashboards/component/table/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/component/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/component/table/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/component/table/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/component/table/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/component/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.475064 django-dashboards-0.1.0/dashboards/menus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/menus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/menus/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/menus/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.475064 django-dashboards-0.1.0/dashboards/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.467064 django-dashboards-0.1.0/dashboards/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.467064 django-dashboards-0.1.0/dashboards/static/dashboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.475064 django-dashboards-0.1.0/dashboards/static/dashboards/css/
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/static/dashboards/css/dashboards.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.475064 django-dashboards-0.1.0/dashboards/static/dashboards/css/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/static/dashboards/css/src/dashboards.css
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/static/dashboards/css/src/grid.css
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/static/dashboards/css/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/static/dashboards/css/src/layout.css
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/static/dashboards/css/src/menu.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.467064 django-dashboards-0.1.0/dashboards/static/dashboards/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.475064 django-dashboards-0.1.0/dashboards/static/dashboards/vendor/css/
--rw-r--r--   0 runner    (1001) docker     (123)    28778 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/static/dashboards/vendor/css/datatables.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.475064 django-dashboards-0.1.0/dashboards/static/dashboards/vendor/js/
--rw-r--r--   0 runner    (1001) docker     (123)    39713 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/static/dashboards/vendor/js/alpine.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   190782 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/static/dashboards/vendor/js/datatables.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    39433 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/static/dashboards/vendor/js/htmx.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/static/dashboards/vendor/js/htmx.sse.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89663 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/static/dashboards/vendor/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  3682474 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/static/dashboards/vendor/js/plotly.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.467064 django-dashboards-0.1.0/dashboards/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.479064 django-dashboards-0.1.0/dashboards/templates/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.479064 django-dashboards-0.1.0/dashboards/templates/dashboards/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.479064 django-dashboards-0.1.0/dashboards/templates/dashboards/components/chart/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/components/chart/chart.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/components/component.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.479064 django-dashboards-0.1.0/dashboards/templates/dashboards/components/form/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/components/form/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/components/loading.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.479064 django-dashboards-0.1.0/dashboards/templates/dashboards/components/map/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/components/map/map.html
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/components/partial.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.479064 django-dashboards-0.1.0/dashboards/templates/dashboards/components/table/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/components/table/basic.html
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/components/table/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.479064 django-dashboards-0.1.0/dashboards/templates/dashboards/components/text/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/components/text/html.html
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/components/text/stat.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/components/text/text.html
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/dashboard_partial.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.471064 django-dashboards-0.1.0/dashboards/templates/dashboards/includes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.479064 django-dashboards-0.1.0/dashboards/templates/dashboards/includes/static/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/includes/static/js.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/includes/static/style.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.471064 django-dashboards-0.1.0/dashboards/templates/dashboards/layout/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.479064 django-dashboards-0.1.0/dashboards/templates/dashboards/layout/components/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/layout/components/card.html
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/layout/components/div.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.479064 django-dashboards-0.1.0/dashboards/templates/dashboards/layout/components/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/layout/components/tabs/container.html
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/layout/components/tabs/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templates/dashboards/layout/components/tabs/tab.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.479064 django-dashboards-0.1.0/dashboards/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/templatetags/dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/dashboards/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.479064 django-dashboards-0.1.0/django_dashboards.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-14 14:12:18.000000 django-dashboards-0.1.0/django_dashboards.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-04-14 14:12:18.000000 django-dashboards-0.1.0/django_dashboards.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:12:18.000000 django-dashboards-0.1.0/django_dashboards.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 14:12:18.000000 django-dashboards-0.1.0/django_dashboards.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 14:12:18.000000 django-dashboards-0.1.0/django_dashboards.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.483064 django-dashboards-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.483064 django-dashboards-0.1.0/docs/dashboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.483064 django-dashboards-0.1.0/docs/dashboards/howto/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.491064 django-dashboards-0.1.0/docs/dashboards/howto/_images/
--rw-r--r--   0 runner    (1001) docker     (123)   100655 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/async_component.gif
--rw-r--r--   0 runner    (1001) docker     (123)    40145 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/components_add_form.png
--rw-r--r--   0 runner    (1001) docker     (123)   102530 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/components_chart_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    22585 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/components_gauge.png
--rw-r--r--   0 runner    (1001) docker     (123)    85957 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/components_map_examples.png
--rw-r--r--   0 runner    (1001) docker     (123)    54151 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/components_table.png
--rw-r--r--   0 runner    (1001) docker     (123)  5090771 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/demo.gif
--rw-r--r--   0 runner    (1001) docker     (123)   152677 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/dependent_table_dashboard.gif
--rw-r--r--   0 runner    (1001) docker     (123)    29811 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/layout_basic.png
--rw-r--r--   0 runner    (1001) docker     (123)    52925 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/layout_complex.png
--rw-r--r--   0 runner    (1001) docker     (123)  1040391 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/quickstart_dashboard.gif
--rw-r--r--   0 runner    (1001) docker     (123)    35761 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/quickstart_dashboard.png
--rw-r--r--   0 runner    (1001) docker     (123)    86305 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/serializers_chart.png
--rw-r--r--   0 runner    (1001) docker     (123)    97282 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/serializers_layout.png
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/templates_custom_component_template.png
--rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/templates_custom_loading.png
--rw-r--r--   0 runner    (1001) docker     (123)   100070 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/templates_custom_template.png
--rw-r--r--   0 runner    (1001) docker     (123)    79174 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/_images/templates_style.png
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/async.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.491064 django-dashboards-0.1.0/docs/dashboards/howto/components/
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/components/attributes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/components/custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/components/included.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/components/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/dashboards.rst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/demo.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/dynamic.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/layout.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/menus.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/permissions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.491064 django-dashboards-0.1.0/docs/dashboards/howto/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/serializers/chart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/serializers/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/serializers/table.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/sse.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/templates.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/howto/views.rst
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/dashboards/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/docs_dj_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-14 14:12:18.495064 django-dashboards-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.491064 django-dashboards-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.491064 django-dashboards-0.1.0/tests/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.491064 django-dashboards-0.1.0/tests/dashboards/app1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/app1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/app1/dashboards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.491064 django-dashboards-0.1.0/tests/dashboards/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.491064 django-dashboards-0.1.0/tests/dashboards/components/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/components/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/components/snapshots/snap_test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/components/snapshots/snap_test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/components/snapshots/snap_test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/components/snapshots/snap_test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/components/snapshots/snap_test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/components/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/components/test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/components/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/components/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/components/test_text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.495064 django-dashboards-0.1.0/tests/dashboards/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.495064 django-dashboards-0.1.0/tests/dashboards/dashboard/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/dashboard/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/dashboard/snapshots/snap_test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/dashboard/snapshots/snap_test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/dashboard/snapshots/snap_test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/dashboard/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/dashboard/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/dashboard/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/dashboard/test_model_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/dashboard/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.495064 django-dashboards-0.1.0/tests/dashboards/menu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/menu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/menu/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/menu/test_menutags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.495064 django-dashboards-0.1.0/tests/dashboards/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/snapshots/snap_test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/snapshots/snap_test_dashboard_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/snapshots/snap_test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/snapshots/snap_test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/test_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.495064 django-dashboards-0.1.0/tests/dashboards/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.495064 django-dashboards-0.1.0/tests/dashboards/views/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/views/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/views/snapshots/snap_test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/views/snapshots/snap_test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/views/snapshots/snap_test_form_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/views/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/views/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/dashboards/views/test_form_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:18.495064 django-dashboards-0.1.0/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/meta/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-14 14:12:15.000000 django-dashboards-0.1.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8641 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/component/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/chart/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/chart/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/component/table/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/table/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/table/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/table/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/menus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/menus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/menus/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/menus/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.344059 django-dashboards-0.1.1/dashboards/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.344059 django-dashboards-0.1.1/dashboards/static/dashboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/static/dashboards/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/css/dashboards.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/static/dashboards/css/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/css/src/dashboards.css
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/css/src/grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/css/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/css/src/layout.css
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/css/src/menu.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.344059 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    28778 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/css/datatables.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.356059 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    39713 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/alpine.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   190782 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/datatables.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39433 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/htmx.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/htmx.sse.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89663 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3682474 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/plotly.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.344059 django-dashboards-0.1.1/dashboards/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/components/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/chart/chart.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/component.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/components/form/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/form/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/loading.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/components/map/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/map/map.html
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/partial.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/components/table/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/table/basic.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/table/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/components/text/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/text/html.html
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/text/stat.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/text/text.html
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/dashboard_partial.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.344059 django-dashboards-0.1.1/dashboards/templates/dashboards/includes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/includes/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/includes/static/js.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/includes/static/style.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.348059 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/card.html
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/div.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/tabs/container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/tabs/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/tabs/tab.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templatetags/dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/django_dashboards.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8641 2023-04-14 15:08:16.000000 django-dashboards-0.1.1/django_dashboards.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-04-14 15:08:16.000000 django-dashboards-0.1.1/django_dashboards.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:08:16.000000 django-dashboards-0.1.1/django_dashboards.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 15:08:16.000000 django-dashboards-0.1.1/django_dashboards.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 15:08:16.000000 django-dashboards-0.1.1/django_dashboards.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.364059 django-dashboards-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.364059 django-dashboards-0.1.1/docs/dashboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.364059 django-dashboards-0.1.1/docs/dashboards/howto/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.372059 django-dashboards-0.1.1/docs/dashboards/howto/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)   100655 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/async_component.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    40145 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/components_add_form.png
+-rw-r--r--   0 runner    (1001) docker     (123)   102530 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/components_chart_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22585 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/components_gauge.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85957 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/components_map_examples.png
+-rw-r--r--   0 runner    (1001) docker     (123)    54151 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/components_table.png
+-rw-r--r--   0 runner    (1001) docker     (123)  5090771 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/demo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   152677 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/dependent_table_dashboard.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    29811 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/layout_basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52925 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/layout_complex.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1040391 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/quickstart_dashboard.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    35761 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/quickstart_dashboard.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86305 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/serializers_chart.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97282 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/serializers_layout.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_custom_component_template.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_custom_loading.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100070 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_custom_template.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79174 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_style.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/async.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.376059 django-dashboards-0.1.1/docs/dashboards/howto/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/components/attributes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/components/custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/components/included.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/components/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/dashboards.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/demo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/dynamic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/layout.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/menus.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/permissions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.376059 django-dashboards-0.1.1/docs/dashboards/howto/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/serializers/chart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/serializers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/serializers/table.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/sse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/views.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/docs_dj_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-14 15:08:16.384060 django-dashboards-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.376059 django-dashboards-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.376059 django-dashboards-0.1.1/tests/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.376059 django-dashboards-0.1.1/tests/dashboards/app1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/app1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/app1/dashboards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.376059 django-dashboards-0.1.1/tests/dashboards/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.376059 django-dashboards-0.1.1/tests/dashboards/components/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/tests/dashboards/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/tests/dashboards/dashboard/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/snapshots/snap_test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/snapshots/snap_test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/snapshots/snap_test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/test_model_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/tests/dashboards/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/menu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/menu/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/menu/test_menutags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/tests/dashboards/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/snapshots/snap_test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/snapshots/snap_test_dashboard_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/snapshots/snap_test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/snapshots/snap_test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/test_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/tests/dashboards/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/tests/dashboards/views/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/snapshots/snap_test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/snapshots/snap_test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/snapshots/snap_test_form_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/test_form_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/meta/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/utils.py
```

### Comparing `django-dashboards-0.1.0/LICENSE` & `django-dashboards-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/README.rst` & `django-dashboards-0.1.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ========
 
 * Dashboard view generation with components including stats, tables, charts and more.
 * HTMX driven dashboards and templates for a modern MPA interface.
 
 Supports Django 3.2 to 4.1, on Python 3.9+.
 
-See the `full documentation <https://django-dashboards.readthedocs.io>`_ for details
+See the `full documentation <https://wildfish-django-dashboards.readthedocs.io>`_ for details
 of how django-dashboards works.
 
 .. inclusion-quickstart-do-not-remove
 
 Quickstart
 ==========
```

### Comparing `django-dashboards-0.1.0/dashboards/component/base.py` & `django-dashboards-0.1.1/dashboards/component/base.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/component/chart/chart.py` & `django-dashboards-0.1.1/dashboards/component/chart/chart.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/component/chart/serializers.py` & `django-dashboards-0.1.1/dashboards/component/chart/serializers.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/component/form.py` & `django-dashboards-0.1.1/dashboards/component/form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/component/layout.py` & `django-dashboards-0.1.1/dashboards/component/layout.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/component/map.py` & `django-dashboards-0.1.1/dashboards/component/map.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/component/table/mixins.py` & `django-dashboards-0.1.1/dashboards/component/table/mixins.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/component/table/serializers.py` & `django-dashboards-0.1.1/dashboards/component/table/serializers.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/component/table/table.py` & `django-dashboards-0.1.1/dashboards/component/table/table.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/component/text.py` & `django-dashboards-0.1.1/dashboards/component/text.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/config.py` & `django-dashboards-0.1.1/dashboards/config.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/dashboard.py` & `django-dashboards-0.1.1/dashboards/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/forms.py` & `django-dashboards-0.1.1/dashboards/forms.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/menus/menu.py` & `django-dashboards-0.1.1/dashboards/menus/menu.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/meta/__init__.py` & `django-dashboards-0.1.1/dashboards/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/permissions.py` & `django-dashboards-0.1.1/dashboards/permissions.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/registry.py` & `django-dashboards-0.1.1/dashboards/registry.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/static/dashboards/css/dashboards.css` & `django-dashboards-0.1.1/dashboards/static/dashboards/css/dashboards.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/static/dashboards/css/src/dashboards.css` & `django-dashboards-0.1.1/dashboards/static/dashboards/css/src/dashboards.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/static/dashboards/css/src/grid.css` & `django-dashboards-0.1.1/dashboards/static/dashboards/css/src/grid.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/static/dashboards/css/src/layout.css` & `django-dashboards-0.1.1/dashboards/static/dashboards/css/src/layout.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/static/dashboards/css/src/menu.css` & `django-dashboards-0.1.1/dashboards/static/dashboards/css/src/menu.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/static/dashboards/vendor/css/datatables.min.css` & `django-dashboards-0.1.1/dashboards/static/dashboards/vendor/css/datatables.min.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/static/dashboards/vendor/js/alpine.min.js` & `django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/alpine.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/static/dashboards/vendor/js/datatables.min.js` & `django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/datatables.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/static/dashboards/vendor/js/htmx.min.js` & `django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/static/dashboards/vendor/js/htmx.sse.min.js` & `django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/htmx.sse.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/static/dashboards/vendor/js/jquery.min.js` & `django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/static/dashboards/vendor/js/plotly.min.js` & `django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/plotly.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/templates/dashboards/base.html` & `django-dashboards-0.1.1/dashboards/templates/dashboards/base.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/templates/dashboards/components/chart/chart.html` & `django-dashboards-0.1.1/dashboards/templates/dashboards/components/chart/chart.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/templates/dashboards/components/component.html` & `django-dashboards-0.1.1/dashboards/templates/dashboards/components/component.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/templates/dashboards/components/form/form.html` & `django-dashboards-0.1.1/dashboards/templates/dashboards/components/form/form.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/templates/dashboards/components/map/map.html` & `django-dashboards-0.1.1/dashboards/templates/dashboards/components/map/map.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/templates/dashboards/components/table/basic.html` & `django-dashboards-0.1.1/dashboards/templates/dashboards/components/table/basic.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/templates/dashboards/components/table/index.html` & `django-dashboards-0.1.1/dashboards/templates/dashboards/components/table/index.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/templates/dashboards/components/text/stat.html` & `django-dashboards-0.1.1/dashboards/templates/dashboards/components/text/stat.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/templates/dashboards/dashboard.html` & `django-dashboards-0.1.1/dashboards/templates/dashboards/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/templates/dashboards/layout/components/card.html` & `django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/card.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/templatetags/dashboards.py` & `django-dashboards-0.1.1/dashboards/templatetags/dashboards.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/urls.py` & `django-dashboards-0.1.1/dashboards/urls.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/dashboards/views.py` & `django-dashboards-0.1.1/dashboards/views.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/django_dashboards.egg-info/SOURCES.txt` & `django-dashboards-0.1.1/django_dashboards.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/Makefile` & `django-dashboards-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/conf.py` & `django-dashboards-0.1.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "django-dashboards"
 copyright = "2023, Wildfish"
 author = "Wildfish"
-release = "0.1.0"
+release = "0.1.1"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ["sphinx.ext.autodoc"]
 
 templates_path = ["_templates"]
```

### Comparing `django-dashboards-0.1.0/docs/contributing.rst` & `django-dashboards-0.1.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/async_component.gif` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/async_component.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/components_add_form.png` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/components_add_form.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/components_chart_example.png` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/components_chart_example.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/components_gauge.png` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/components_gauge.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/components_map_examples.png` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/components_map_examples.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/components_table.png` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/components_table.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/demo.gif` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/demo.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/dependent_table_dashboard.gif` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/dependent_table_dashboard.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/layout_basic.png` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/layout_basic.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/layout_complex.png` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/layout_complex.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/quickstart_dashboard.gif` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/quickstart_dashboard.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/quickstart_dashboard.png` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/quickstart_dashboard.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/serializers_chart.png` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/serializers_chart.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/serializers_layout.png` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/serializers_layout.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/templates_custom_component_template.png` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_custom_component_template.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/templates_custom_loading.png` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_custom_loading.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/templates_custom_template.png` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_custom_template.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/_images/templates_style.png` & `django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_style.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/async.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/async.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/components/attributes.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/components/attributes.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/components/custom.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/components/custom.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/components/included.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/components/included.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/components/index.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/components/index.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/dashboards.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/dashboards.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/demo.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/demo.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/dynamic.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/dynamic.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/layout.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/layout.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/menus.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/menus.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/permissions.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/permissions.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/quickstart.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/serializers/chart.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/serializers/chart.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/serializers/table.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/serializers/table.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/settings.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/settings.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/sse.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/sse.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/templates.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/templates.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/howto/views.rst` & `django-dashboards-0.1.1/docs/dashboards/howto/views.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/dashboards/index.rst` & `django-dashboards-0.1.1/docs/dashboards/index.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/docs_dj_settings.py` & `django-dashboards-0.1.1/docs/docs_dj_settings.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/index.rst` & `django-dashboards-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/make.bat` & `django-dashboards-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/docs/requirements.txt` & `django-dashboards-0.1.1/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/setup.cfg` & `django-dashboards-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = django-dashboards
-version = 0.1.0
+version = 0.1.1
 description = Tools for building data dashboards with Django
-long_description = file: README.md
+long_description = file: README.rst
 url = https://github.com/wildfish/django-dashboards
 author = Wildfish
 author_email = developers@wildfish.com
 license = BSD-3-Clause
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Web Environment
```

### Comparing `django-dashboards-0.1.0/tests/conftest.py` & `django-dashboards-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/app1/dashboards.py` & `django-dashboards-0.1.1/tests/dashboards/app1/dashboards.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/components/snapshots/snap_test_base.py` & `django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_base.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/components/snapshots/snap_test_chart.py` & `django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_chart.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/components/snapshots/snap_test_form.py` & `django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/components/snapshots/snap_test_table.py` & `django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_table.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/components/snapshots/snap_test_text.py` & `django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_text.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/components/test_base.py` & `django-dashboards-0.1.1/tests/dashboards/components/test_base.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/components/test_chart.py` & `django-dashboards-0.1.1/tests/dashboards/components/test_chart.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/components/test_form.py` & `django-dashboards-0.1.1/tests/dashboards/components/test_form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/components/test_table.py` & `django-dashboards-0.1.1/tests/dashboards/components/test_table.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/components/test_text.py` & `django-dashboards-0.1.1/tests/dashboards/components/test_text.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/dashboard/snapshots/snap_test_form.py` & `django-dashboards-0.1.1/tests/dashboards/dashboard/snapshots/snap_test_form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/dashboard/snapshots/snap_test_layout.py` & `django-dashboards-0.1.1/tests/dashboards/dashboard/snapshots/snap_test_layout.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/dashboard/test_dashboard.py` & `django-dashboards-0.1.1/tests/dashboards/dashboard/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/dashboard/test_layout.py` & `django-dashboards-0.1.1/tests/dashboards/dashboard/test_layout.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/dashboard/test_model_dashboard.py` & `django-dashboards-0.1.1/tests/dashboards/dashboard/test_model_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/dashboard/test_permissions.py` & `django-dashboards-0.1.1/tests/dashboards/dashboard/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/fixtures.py` & `django-dashboards-0.1.1/tests/dashboards/fixtures.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/menu/test_menu.py` & `django-dashboards-0.1.1/tests/dashboards/menu/test_menu.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/menu/test_menutags.py` & `django-dashboards-0.1.1/tests/dashboards/menu/test_menutags.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/snapshots/snap_test_dashboard_form.py` & `django-dashboards-0.1.1/tests/dashboards/snapshots/snap_test_dashboard_form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/snapshots/snap_test_layout.py` & `django-dashboards-0.1.1/tests/dashboards/snapshots/snap_test_layout.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/snapshots/snap_test_schema.py` & `django-dashboards-0.1.1/tests/dashboards/snapshots/snap_test_schema.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/test_registry.py` & `django-dashboards-0.1.1/tests/dashboards/test_registry.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/test_urls.py` & `django-dashboards-0.1.1/tests/dashboards/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/views/snapshots/snap_test_component.py` & `django-dashboards-0.1.1/tests/dashboards/views/snapshots/snap_test_component.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/views/snapshots/snap_test_dashboard.py` & `django-dashboards-0.1.1/tests/dashboards/views/snapshots/snap_test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/views/test_component.py` & `django-dashboards-0.1.1/tests/dashboards/views/test_component.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/views/test_dashboard.py` & `django-dashboards-0.1.1/tests/dashboards/views/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/dashboards/views/test_form_component.py` & `django-dashboards-0.1.1/tests/dashboards/views/test_form_component.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/meta/test_meta.py` & `django-dashboards-0.1.1/tests/meta/test_meta.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.0/tests/settings.py` & `django-dashboards-0.1.1/tests/settings.py`

 * *Files identical despite different names*

