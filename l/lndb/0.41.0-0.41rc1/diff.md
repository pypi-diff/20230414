# Comparing `tmp/lndb-0.41.0.tar.gz` & `tmp/lndb-0.41rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb-0.41.0.tar", last modified: Fri Apr 14 10:41:59 2023, max compression
+gzip compressed data, was "lndb-0.41rc1.tar", last modified: Sat Apr  8 10:30:13 2023, max compression
```

## Comparing `lndb-0.41.0.tar` & `lndb-0.41rc1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     3832 2023-04-10 13:46:35.171473 lndb-0.41.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.41.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.41.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.41.0/.gitignore
--rw-r--r--   0        0        0     1772 2023-01-16 03:13:03.815140 lndb-0.41.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.41.0/LICENSE
--rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.41.0/README.md
--rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.41.0/docs/api.md
--rw-r--r--   0        0        0    45851 2023-04-14 10:41:37.318232 lndb-0.41.0/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.41.0/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.41.0/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-03-22 05:59:33.863010 lndb-0.41.0/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.41.0/docs/faq/index.md
--rw-r--r--   0        0        0     1180 2023-04-05 05:10:26.112382 lndb-0.41.0/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.41.0/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2798 2023-04-05 05:10:26.112662 lndb-0.41.0/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.41.0/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5163 2023-04-10 13:41:10.762652 lndb-0.41.0/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    10679 2023-04-07 09:41:26.324653 lndb-0.41.0/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     5573 2023-03-22 14:56:35.818426 lndb-0.41.0/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     5290 2023-03-09 09:28:04.966850 lndb-0.41.0/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3724 2023-03-22 05:59:33.864269 lndb-0.41.0/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     1496 2023-03-22 05:59:33.864524 lndb-0.41.0/docs/guide/06-info.ipynb
--rw-r--r--   0        0        0     3282 2023-03-22 05:59:33.864793 lndb-0.41.0/docs/guide/07-delete.ipynb
--rw-r--r--   0        0        0      129 2023-02-16 15:52:14.590660 lndb-0.41.0/docs/guide/index.md
--rw-r--r--   0        0        0     3152 2023-03-25 20:23:06.444401 lndb-0.41.0/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.41.0/docs/index.md
--rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.41.0/lamin-project.yaml
--rw-r--r--   0        0        0     1932 2023-04-14 10:41:08.385843 lndb-0.41.0/lndb/__init__.py
--rw-r--r--   0        0        0     4242 2023-02-27 18:35:12.951712 lndb-0.41.0/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.41.0/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-10 10:56:05.782722 lndb-0.41.0/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      216 2023-04-03 04:25:19.341088 lndb-0.41.0/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.41.0/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.41.0/lndb/_delete.py
--rw-r--r--   0        0        0      222 2023-02-16 21:53:37.660919 lndb-0.41.0/lndb/_info.py
--rw-r--r--   0        0        0     5710 2023-04-08 10:27:51.833294 lndb-0.41.0/lndb/_init_instance.py
--rw-r--r--   0        0        0     4192 2023-04-12 21:03:40.398013 lndb-0.41.0/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.41.0/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.41.0/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3469 2023-04-05 12:41:02.533096 lndb-0.41.0/lndb/_migrate/core.py
--rw-r--r--   0        0        0     6303 2023-04-05 05:10:26.114561 lndb-0.41.0/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.41.0/lndb/_migrate/env.py
--rw-r--r--   0        0        0      341 2023-02-16 21:53:37.661843 lndb-0.41.0/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.41.0/lndb/_migrate/utils.py
--rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.41.0/lndb/_schema.py
--rw-r--r--   0        0        0     1493 2023-04-08 10:27:51.833937 lndb-0.41.0/lndb/_set.py
--rw-r--r--   0        0        0     2181 2023-04-07 09:41:26.325000 lndb-0.41.0/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.41.0/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.41.0/lndb/_settings_store.py
--rw-r--r--   0        0        0     4927 2023-04-11 15:29:00.205425 lndb-0.41.0/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-04-08 10:27:51.834128 lndb-0.41.0/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-03-27 17:35:42.591834 lndb-0.41.0/lndb/dev/_clone.py
--rw-r--r--   0        0        0     6226 2023-04-07 09:41:26.325330 lndb-0.41.0/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.41.0/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.41.0/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.41.0/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8429 2023-04-08 10:27:51.834794 lndb-0.41.0/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.41.0/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.41.0/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-07 05:02:28.778847 lndb-0.41.0/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.41.0/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2446 2023-03-21 06:52:10.981980 lndb-0.41.0/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     6996 2023-03-30 17:54:01.453792 lndb-0.41.0/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     4917 2023-04-08 10:27:51.835175 lndb-0.41.0/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-02-24 20:31:36.945684 lndb-0.41.0/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.41.0/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.41.0/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.41.0/lndb/test/_env.py
--rw-r--r--   0        0        0     3856 2023-03-30 17:54:01.454075 lndb-0.41.0/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.41.0/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-02-24 20:31:36.946490 lndb-0.41.0/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.41.0/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-10 13:46:02.409554 lndb-0.41.0/noxfile.py
--rw-r--r--   0        0        0     1378 2023-04-08 10:27:51.835572 lndb-0.41.0/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-10 13:57:46.942655 lndb-0.41.0/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.41.0/tests/test_init_instance.py
--rw-r--r--   0        0        0      385 2023-02-21 15:53:42.076396 lndb-0.41.0/tests/test_notebooks.py
--rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 lndb-0.41.0/PKG-INFO
+-rw-r--r--   0        0        0     3899 2023-04-08 08:06:48.849153 lndb-0.41rc1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.41rc1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.41rc1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.41rc1/.gitignore
+-rw-r--r--   0        0        0     1772 2023-01-16 03:13:03.815140 lndb-0.41rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.41rc1/LICENSE
+-rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.41rc1/README.md
+-rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.41rc1/docs/api.md
+-rw-r--r--   0        0        0    45671 2023-04-08 10:29:49.219972 lndb-0.41rc1/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.41rc1/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.41rc1/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-03-22 05:59:33.863010 lndb-0.41rc1/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.41rc1/docs/faq/index.md
+-rw-r--r--   0        0        0     1180 2023-04-05 05:10:26.112382 lndb-0.41rc1/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.41rc1/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-05 05:10:26.112662 lndb-0.41rc1/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.41rc1/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-03-22 05:59:33.863390 lndb-0.41rc1/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    10679 2023-04-07 09:41:26.324653 lndb-0.41rc1/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     5573 2023-03-22 14:56:35.818426 lndb-0.41rc1/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     5290 2023-03-09 09:28:04.966850 lndb-0.41rc1/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3724 2023-03-22 05:59:33.864269 lndb-0.41rc1/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-03-22 05:59:33.864524 lndb-0.41rc1/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     3282 2023-03-22 05:59:33.864793 lndb-0.41rc1/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-02-16 15:52:14.590660 lndb-0.41rc1/docs/guide/index.md
+-rw-r--r--   0        0        0     3152 2023-03-25 20:23:06.444401 lndb-0.41rc1/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.41rc1/docs/index.md
+-rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.41rc1/lamin-project.yaml
+-rw-r--r--   0        0        0     1933 2023-04-08 10:29:34.569547 lndb-0.41rc1/lndb/__init__.py
+-rw-r--r--   0        0        0     4242 2023-02-27 18:35:12.951712 lndb-0.41rc1/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.41rc1/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1380 2023-04-08 10:27:51.832625 lndb-0.41rc1/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      216 2023-04-03 04:25:19.341088 lndb-0.41rc1/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.41rc1/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.41rc1/lndb/_delete.py
+-rw-r--r--   0        0        0      222 2023-02-16 21:53:37.660919 lndb-0.41rc1/lndb/_info.py
+-rw-r--r--   0        0        0     5710 2023-04-08 10:27:51.833294 lndb-0.41rc1/lndb/_init_instance.py
+-rw-r--r--   0        0        0     3691 2023-04-08 10:27:51.833611 lndb-0.41rc1/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.41rc1/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.41rc1/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3469 2023-04-05 12:41:02.533096 lndb-0.41rc1/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     6303 2023-04-05 05:10:26.114561 lndb-0.41rc1/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.41rc1/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      341 2023-02-16 21:53:37.661843 lndb-0.41rc1/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.41rc1/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.41rc1/lndb/_schema.py
+-rw-r--r--   0        0        0     1493 2023-04-08 10:27:51.833937 lndb-0.41rc1/lndb/_set.py
+-rw-r--r--   0        0        0     2181 2023-04-07 09:41:26.325000 lndb-0.41rc1/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.41rc1/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.41rc1/lndb/_settings_store.py
+-rw-r--r--   0        0        0     5291 2023-03-12 15:04:39.932675 lndb-0.41rc1/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-08 10:27:51.834128 lndb-0.41rc1/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-03-27 17:35:42.591834 lndb-0.41rc1/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-07 09:41:26.325330 lndb-0.41rc1/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.41rc1/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.41rc1/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.41rc1/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8429 2023-04-08 10:27:51.834794 lndb-0.41rc1/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.41rc1/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.41rc1/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-07 05:02:28.778847 lndb-0.41rc1/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.41rc1/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-03-21 06:52:10.981980 lndb-0.41rc1/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     6996 2023-03-30 17:54:01.453792 lndb-0.41rc1/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     4917 2023-04-08 10:27:51.835175 lndb-0.41rc1/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-02-24 20:31:36.945684 lndb-0.41rc1/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.41rc1/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.41rc1/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.41rc1/lndb/test/_env.py
+-rw-r--r--   0        0        0     3856 2023-03-30 17:54:01.454075 lndb-0.41rc1/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.41rc1/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-02-24 20:31:36.946490 lndb-0.41rc1/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.41rc1/lndb/test/nox.py
+-rw-r--r--   0        0        0     1514 2023-03-09 09:28:04.969263 lndb-0.41rc1/noxfile.py
+-rw-r--r--   0        0        0     1378 2023-04-08 10:27:51.835572 lndb-0.41rc1/pyproject.toml
+-rw-r--r--   0        0        0      506 2023-02-12 04:51:38.276939 lndb-0.41rc1/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.41rc1/tests/test_init_instance.py
+-rw-r--r--   0        0        0      385 2023-02-21 15:53:42.076396 lndb-0.41rc1/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 lndb-0.41rc1/PKG-INFO
```

### Comparing `lndb-0.41.0/.github/workflows/build.yml` & `lndb-0.41rc1/.github/workflows/build.yml`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,14 @@
     branches: [main, staging]
   pull_request:
     branches: [main]
 
 jobs:
   build:
     runs-on: ubuntu-22.04
-    env:
-      GITHUB_EVENT_NAME: ${{ github.event_name }}
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.9"]
     timeout-minutes: 20
 
     steps:
@@ -26,51 +24,45 @@
         uses: actions/checkout@v3
         with:
           repository: laminlabs/lndocs
           ssh-key: ${{ secrets.READ_LNDOCS }}
           path: lndocs
           ref: main
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python-version }}
-          cache: "pip"
-          cache-dependency-path: ".github/workflows/build.yml" # See dependencies below
-      - name: Cache nox
-        uses: actions/cache@v3
-        with:
-          path: .nox
-          key: nox-${{ runner.os }}
-      - name: Cache pre-commit
+      - name: Cache pre-commit & nox
         uses: actions/cache@v3
+        env:
+          cache-name: cache-4
         with:
-          path: ~/.cache/pre-commit
-          key: pre-commit-${{ runner.os }}-${{ hashFiles('.pre-commit-config.yaml') }}
+          path: |
+            .nox
+            ~/.cache/pre-commit
+          key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('.pre-commit-config.yaml') }}-${{ hashFiles('pyproject.yaml') }}
       - name: Cache postgres
         id: cache-postgres
         uses: actions/cache@v3
         with:
           path: ~/postgres.tar
           key: cache-postgres-0
       - name: Cache postgres miss
         if: steps.cache-postgres.outputs.cache-hit != 'true'
         run: docker pull postgres:latest && docker image save postgres:latest --output ~/postgres.tar
       - name: Cache postgres use
         if: steps.cache-postgres.outputs.cache-hit == 'true'
         run: docker image load --input ~/postgres.tar
-      - name: Install Python dependencies
+      - name: Install dependencies
         run: |
           python -m pip install -U pip
-          pip install -U laminci
-          pip install -U lamindb
-      - name: Install apt-get dependencies
-        run: |
+          pip install laminci>=0.3.0
+          pip install lamindb
           sudo apt-get -y install graphviz
           sudo apt-get install sqlite3-tools=3.37.2-2
-          sudo apt-get install libpq-dev
       - name: Lint
         run: |
           nox -s lint
       - name: Configure AWS
         uses: aws-actions/configure-aws-credentials@v2
         with:
           aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
@@ -98,14 +90,20 @@
       - name: Read lamin-project.yaml
         if: matrix.python-version == '3.9'
         id: lamin-project
         uses: CumulusDS/get-yaml-paths-action@v0.1.0
         with:
           file: lamin-project.yaml
           project_slug: project_slug
+      - name: Change base URL to project-slug
+        if: github.event_name == 'push' && matrix.python-version == '3.9'
+        run: |
+          mv _build/html _build/${{ steps.lamin-project.outputs.project_slug }}
+          mkdir -p _build/html/docs
+          mv _build/${{ steps.lamin-project.outputs.project_slug }} _build/html/docs
       - name: Deploy docs
         if: matrix.python-version == '3.9'
         id: netlify
         uses: nwtgck/actions-netlify@v1.2
         with:
           publish-dir: "_build/html"
           production-deploy: ${{ github.event_name == 'push' }}
```

### Comparing `lndb-0.41.0/.github/workflows/latest-changes.yml` & `lndb-0.41rc1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/.gitignore` & `lndb-0.41rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/.pre-commit-config.yaml` & `lndb-0.41rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/LICENSE` & `lndb-0.41rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/changelog.md` & `lndb-0.41rc1/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-🔊 Clarify access based on locally cached instance metadata | [354](https://github.com/laminlabs/lndb/pull/354) | [falexwolf](https://github.com/falexwolf) | 2023-04-11 | 0.41.0
 🎨 Move setup checks from lamindb here | [352](https://github.com/laminlabs/lndb/pull/352) | [falexwolf](https://github.com/falexwolf) | 2023-04-08 | 0.41rc1
 🔧 Increase configure-aws-credentials version from v1 to v2 | [344](https://github.com/laminlabs/lndb/pull/344) | [Zethson](https://github.com/Zethson) | 2023-04-07 |
 🚸 Expose `id` in `StorageSettings` | [351](https://github.com/laminlabs/lndb/pull/351) | [falexwolf](https://github.com/falexwolf) | 2023-04-07 | 0.40.2
 ➕ Add cloudpathlib back | [350](https://github.com/laminlabs/lndb/pull/350) | [falexwolf](https://github.com/falexwolf) | 2023-04-07 | 0.40.1
 🚸 Rename settings directory to `.lamin` | [349](https://github.com/laminlabs/lndb/pull/349) | [falexwolf](https://github.com/falexwolf) | 2023-04-07 | 0.40.0
 🚸 Expose storage in settings | [348](https://github.com/laminlabs/lndb/pull/348) | [falexwolf](https://github.com/falexwolf) | 2023-04-07 |
 ♻️ Move storage related code to lndb_storage | [338](https://github.com/laminlabs/lndb/pull/338) | [Koncopd](https://github.com/Koncopd) | 2023-04-05 |
```

### Comparing `lndb-0.41.0/docs/faq/check-synchronization.ipynb` & `lndb-0.41rc1/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/faq/clone.ipynb` & `lndb-0.41rc1/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/faq/edge-cases-login-init.ipynb` & `lndb-0.41rc1/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/faq/manage-migrations.ipynb` & `lndb-0.41rc1/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/faq/switch-environment.ipynb` & `lndb-0.41rc1/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/faq/test-migrations-e2e.ipynb` & `lndb-0.41rc1/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/faq/test-migrations-unit.ipynb` & `lndb-0.41rc1/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/guide/01-setup-user.ipynb` & `lndb-0.41rc1/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/guide/02-init-instance.ipynb` & `lndb-0.41rc1/docs/guide/02-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/guide/03-load-instance.ipynb` & `lndb-0.41rc1/docs/guide/03-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/guide/04-set-storage.ipynb` & `lndb-0.41rc1/docs/guide/04-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/guide/05-schema-modules.ipynb` & `lndb-0.41rc1/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/guide/06-info.ipynb` & `lndb-0.41rc1/docs/guide/06-info.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/guide/07-delete.ipynb` & `lndb-0.41rc1/docs/guide/07-delete.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/docs/guide/migrate.md` & `lndb-0.41rc1/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/__init__.py` & `lndb-0.41rc1/lndb/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.41.0"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.41rc1"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
```

### Comparing `lndb-0.41.0/lndb/__main__.py` & `lndb-0.41rc1/lndb/__main__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/_check_instance_setup.py` & `lndb-0.41rc1/lndb/_check_instance_setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,17 +21,17 @@
                     usettings=settings.user, isettings=settings.instance
                 )
             # set the check to true
             return True
         except Exception:
             # user will get more detailed traceback once they run the CLI
             raise RuntimeError(
-                "Current instance cannot be reached, close it: `lamin close`\n"
-                "Alternatively, init or load a connectable instance on the"
-                " command line: `lamin load <instance>` or `lamin init <...>`"
+                "Your current instance cannot be reached.\nInit or load a connectable"
+                " instance on the command line: `lamin load <instance>` or `lamin init"
+                " <...>`"
             )
     else:
         logger.warning(
             "You haven't yet setup an instance using the CLI: Please call"
             " `ln.setup.init()` or `ln.setup.load()`"
         )
         return False
```

### Comparing `lndb-0.41.0/lndb/_close.py` & `lndb-0.41rc1/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/_delete.py` & `lndb-0.41rc1/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/_init_instance.py` & `lndb-0.41rc1/lndb/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/_load_instance.py` & `lndb-0.41rc1/lndb/_load_instance.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,44 +29,33 @@
         - migrate-unnecessary if migration was not required
     """
     owner, name = get_owner_name_from_identifier(identifier)
 
     hub_result = load_instance_from_hub(
         owner=owner, name=name, _access_token=_access_token
     )
-    # if hub_result is not a string, it means it made a request
-    # that successfully returned metadata
     if not isinstance(hub_result, str):
         instance, storage = hub_result
         isettings = InstanceSettings(
             owner=owner,
             name=name,
             storage_root=storage.root,
             storage_region=storage.region,
             db=instance.db,
             schema=instance.schema_str,
         )
     else:
-        logger.info(
-            f"Instance {owner}/{name} not loadable from hub with message:"
-            f" '{hub_result}'"
-        )
         settings_file = instance_settings_file(name, owner)
         if settings_file.exists():
-            logger.info(
-                "Loading instance through locally cached instance metadata"
-                f" {settings_file}"
-            )
             isettings = load_instance_settings(settings_file)
         else:
             if _log_error_message:
                 logger.error(
-                    f"Instance {owner}/{name} neither loadable from hub nor local"
-                    " cache. Check whether instance exists and you have access:"
-                    f" https://lamin.ai/{owner}/{name}?tab=collaborators"
+                    "Instance not reachable. Check your access permissions or whether"
+                    " the instance exists."
                 )
             return "instance-not-reachable"
 
     check, msg = isettings._is_db_setup()
     if not check:
         if _log_error_message:
             raise RuntimeError(msg)
```

### Comparing `lndb-0.41.0/lndb/_migrate/alembic.ini` & `lndb-0.41rc1/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/_migrate/core.py` & `lndb-0.41rc1/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/_migrate/deploy.py` & `lndb-0.41rc1/lndb/_migrate/deploy.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/_migrate/env.py` & `lndb-0.41rc1/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/_migrate/utils.py` & `lndb-0.41rc1/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/_schema.py` & `lndb-0.41rc1/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/_set.py` & `lndb-0.41rc1/lndb/_set.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/_settings.py` & `lndb-0.41rc1/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/_setup_user.py` & `lndb-0.41rc1/lndb/_setup_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Union
 
 from lamin_logger import logger
 from lnhub_rest._signup_signin import sign_in_hub, sign_up_hub
 from sqlalchemy import create_engine
 
+from ._schema import schema
 from ._settings import settings
 from .dev._db import upsert
 from .dev._settings_load import load_or_create_user_settings, load_user_settings
 from .dev._settings_save import save_user_settings
 from .dev._settings_store import user_settings_file_email, user_settings_file_handle
 
 
@@ -114,14 +115,20 @@
         if settings.instance.dialect == "sqlite":
             # let's check whether the sqlite file is actually available
             if not settings.instance._sqlite_file.exists():
                 # if the file doesn't exist, there is no need to
                 # log in the user
                 # hence, simply end log in here
                 return None
+            # if the file exists but does not have a user table, raise a warning
+            if "core.user" not in schema.list_entities():
+                logger.warning(
+                    f"An SQLite file {settings.instance._sqlite_file} exists but does not have a user table. "  # noqa
+                )
+                return None
         else:  # let's check whether we can connect to the instance DB
             db = settings.instance.db
             engine = create_engine(db)
             try:
                 engine.connect()
             except Exception:
                 logger.warning(
```

### Comparing `lndb-0.41.0/lndb/dev/__init__.py` & `lndb-0.41rc1/lndb/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/dev/_clone.py` & `lndb-0.41rc1/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/dev/_db.py` & `lndb-0.41rc1/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/dev/_deprecated.py` & `lndb-0.41rc1/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/dev/_exclusion.py` & `lndb-0.41rc1/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/dev/_settings_instance.py` & `lndb-0.41rc1/lndb/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/dev/_settings_load.py` & `lndb-0.41rc1/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/dev/_settings_save.py` & `lndb-0.41rc1/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/dev/_settings_store.py` & `lndb-0.41rc1/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/dev/_settings_user.py` & `lndb-0.41rc1/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/dev/_setup_knowledge.py` & `lndb-0.41rc1/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/dev/_setup_schema.py` & `lndb-0.41rc1/lndb/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/dev/_storage.py` & `lndb-0.41rc1/lndb/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/dev/upath.py` & `lndb-0.41rc1/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/test/_migrations_e2e.py` & `lndb-0.41rc1/lndb/test/_migrations_e2e.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/lndb/test/_migrations_unit.py` & `lndb-0.41rc1/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/pyproject.toml` & `lndb-0.41rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/tests/test_init_instance.py` & `lndb-0.41rc1/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.41.0/PKG-INFO` & `lndb-0.41rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lndb
-Version: 0.41.0
+Version: 0.41rc1
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.7.2
 Requires-Dist: laminci>=0.3.0
 Requires-Dist: lnschema_core>=0.28.0
 Requires-Dist: lamin_logger>=0.2.3
```

