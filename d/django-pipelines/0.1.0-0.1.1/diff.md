# Comparing `tmp/django-pipelines-0.1.0.tar.gz` & `tmp/django-pipelines-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pipelines-0.1.0.tar", last modified: Fri Apr 14 15:00:56 2023, max compression
+gzip compressed data, was "django-pipelines-0.1.1.tar", last modified: Fri Apr 14 15:07:29 2023, max compression
```

## Comparing `django-pipelines-0.1.0.tar` & `django-pipelines-0.1.1.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.994333 django-pipelines-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-04-14 15:00:55.994333 django-pipelines-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.982333 django-pipelines-0.1.0/django_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-04-14 15:00:55.000000 django-pipelines-0.1.0/django_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-14 15:00:55.000000 django-pipelines-0.1.0/django_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:00:55.000000 django-pipelines-0.1.0/django_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-14 15:00:55.000000 django-pipelines-0.1.0/django_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 15:00:55.000000 django-pipelines-0.1.0/django_pipelines.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.986333 django-pipelines-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.986333 django-pipelines-0.1.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.admin.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.apps.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.baker_recipes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.forms.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.log.rst
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.management.commands.clear_tasks_and_logs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.management.commands.pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.management.commands.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.management.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.meta.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.registry.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.reporters.base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.reporters.logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.reporters.orm.rst
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.reporters.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.results.base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.results.helpers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.results.orm.rst
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.results.rst
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.runners.base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.runners.celery.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.runners.celery.runner.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.runners.celery.tasks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.runners.eager.rst
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.runners.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.status.rst
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.tasks.base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.tasks.registry.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.tasks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.templatetags.pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.templatetags.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.urls.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/api/pipelines.views.rst
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/docs_dj_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.986333 django-pipelines-0.1.0/docs/pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.990333 django-pipelines-0.1.0/docs/pipelines/howto/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.990333 django-pipelines-0.1.0/docs/pipelines/howto/_images/
--rw-r--r--   0 runner    (1001) docker     (123)    74041 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/pipelines/howto/_images/quickstart_pipeline_executions.png
--rw-r--r--   0 runner    (1001) docker     (123)   168253 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/pipelines/howto/_images/quickstart_pipeline_results.png
--rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/pipelines/howto/_images/quickstart_pipelines.png
--rw-r--r--   0 runner    (1001) docker     (123)   282531 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/pipelines/howto/_images/quickstart_pipelines_command.gif
--rw-r--r--   0 runner    (1001) docker     (123)    76820 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/pipelines/howto/_images/quickstart_running_pipeline.gif
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/pipelines/howto/management-commands.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/pipelines/howto/pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/pipelines/howto/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/pipelines/howto/reporters.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/pipelines/howto/results.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/pipelines/howto/runners.rst
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/pipelines/howto/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/pipelines/howto/tasks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/docs/pipelines/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.990333 django-pipelines-0.1.0/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/baker_recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.990333 django-pipelines-0.1.0/pipelines/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.990333 django-pipelines-0.1.0/pipelines/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/management/commands/clear_tasks_and_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/management/commands/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.990333 django-pipelines-0.1.0/pipelines/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.994333 django-pipelines-0.1.0/pipelines/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0002_rename_last_run_pipelineexecution_started_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0003_alter_pipelineexecution_reporter_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0004_alter_pipelineexecution_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0004_alter_pipelineexecution_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0005_merge_20230103_1354.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0006_rename_pipelineexecution_pipelineresult_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0007_pipelineexecution_taskexecution_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0008_auto_20230116_1208.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0009_remove_pipelineresult_pipeline_id_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0010_remove_taskexecution_pipeline_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0011_alter_taskresult_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0012_remove_taskresult_pipeline_task_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0013_pipelineexecution_completed_pipelineresult_completed_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0014_remove_pipelineresult_input_data_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0015_delete_tasklog_pipelinelog_context_id_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0016_alter_pipelineexecution_run_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0017_alter_pipelineexecution_run_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0018_rename_pipelineexecution_ormpipelineexecution_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0019_alter_ormpipelineexecution_completed_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/0020_delete_valuestore_alter_pipelinelog_context_type.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16699 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.994333 django-pipelines-0.1.0/pipelines/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/reporters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/reporters/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/reporters/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.994333 django-pipelines-0.1.0/pipelines/results/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/results/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/results/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/results/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.994333 django-pipelines-0.1.0/pipelines/runners/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/runners/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.994333 django-pipelines-0.1.0/pipelines/runners/celery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/runners/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/runners/celery/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/runners/celery/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/runners/eager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.994333 django-pipelines-0.1.0/pipelines/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/tasks/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.982333 django-pipelines-0.1.0/pipelines/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.994333 django-pipelines-0.1.0/pipelines/templates/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templates/pipelines/_log_filter.html
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templates/pipelines/_log_list.html
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templates/pipelines/_results_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templates/pipelines/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.994333 django-pipelines-0.1.0/pipelines/templates/pipelines/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templates/pipelines/includes/pipeline-result-listing.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.994333 django-pipelines-0.1.0/pipelines/templates/pipelines/includes/static/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templates/pipelines/includes/static/js.html
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templates/pipelines/includes/static/style.html
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templates/pipelines/includes/task-execution-listing.html
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templates/pipelines/includes/task-result-listing.html
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templates/pipelines/pipeline.html
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templates/pipelines/pipeline_execution_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templates/pipelines/pipeline_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templates/pipelines/pipeline_start.html
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templates/pipelines/results_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.994333 django-pipelines-0.1.0/pipelines/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/templatetags/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pipelines/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-14 15:00:55.998333 django-pipelines-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.994333 django-pipelines-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:55.994333 django-pipelines-0.1.0/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/tests/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/tests/meta/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-14 15:00:50.000000 django-pipelines-0.1.0/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.232514 django-pipelines-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-04-14 15:07:29.232514 django-pipelines-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.204513 django-pipelines-0.1.1/django_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-04-14 15:07:29.000000 django-pipelines-0.1.1/django_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-14 15:07:29.000000 django-pipelines-0.1.1/django_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:07:29.000000 django-pipelines-0.1.1/django_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-14 15:07:29.000000 django-pipelines-0.1.1/django_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 15:07:29.000000 django-pipelines-0.1.1/django_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.204513 django-pipelines-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.212513 django-pipelines-0.1.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.admin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.apps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.baker_recipes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.forms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.log.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.management.commands.clear_tasks_and_logs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.management.commands.pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.management.commands.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.management.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.meta.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.registry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.reporters.base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.reporters.logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.reporters.orm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.reporters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.results.base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.results.helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.results.orm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.results.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.runners.base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.runners.celery.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.runners.celery.runner.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.runners.celery.tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.runners.eager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.runners.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.status.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.tasks.base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.tasks.registry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.templatetags.pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.templatetags.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.urls.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/api/pipelines.views.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/docs_dj_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.212513 django-pipelines-0.1.1/docs/pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.212513 django-pipelines-0.1.1/docs/pipelines/howto/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.212513 django-pipelines-0.1.1/docs/pipelines/howto/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    74041 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/pipelines/howto/_images/quickstart_pipeline_executions.png
+-rw-r--r--   0 runner    (1001) docker     (123)   168253 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/pipelines/howto/_images/quickstart_pipeline_results.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/pipelines/howto/_images/quickstart_pipelines.png
+-rw-r--r--   0 runner    (1001) docker     (123)   282531 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/pipelines/howto/_images/quickstart_pipelines_command.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    76820 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/pipelines/howto/_images/quickstart_running_pipeline.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/pipelines/howto/management-commands.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/pipelines/howto/pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/pipelines/howto/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/pipelines/howto/reporters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/pipelines/howto/results.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/pipelines/howto/runners.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/pipelines/howto/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/pipelines/howto/tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/docs/pipelines/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.216513 django-pipelines-0.1.1/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/baker_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.216513 django-pipelines-0.1.1/pipelines/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.216513 django-pipelines-0.1.1/pipelines/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/management/commands/clear_tasks_and_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/management/commands/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.216513 django-pipelines-0.1.1/pipelines/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.220513 django-pipelines-0.1.1/pipelines/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0002_rename_last_run_pipelineexecution_started_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0003_alter_pipelineexecution_reporter_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0004_alter_pipelineexecution_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0004_alter_pipelineexecution_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0005_merge_20230103_1354.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0006_rename_pipelineexecution_pipelineresult_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0007_pipelineexecution_taskexecution_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0008_auto_20230116_1208.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0009_remove_pipelineresult_pipeline_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0010_remove_taskexecution_pipeline_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0011_alter_taskresult_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0012_remove_taskresult_pipeline_task_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0013_pipelineexecution_completed_pipelineresult_completed_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0014_remove_pipelineresult_input_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0015_delete_tasklog_pipelinelog_context_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0016_alter_pipelineexecution_run_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0017_alter_pipelineexecution_run_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0018_rename_pipelineexecution_ormpipelineexecution_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0019_alter_ormpipelineexecution_completed_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/0020_delete_valuestore_alter_pipelinelog_context_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16699 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.220513 django-pipelines-0.1.1/pipelines/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/reporters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/reporters/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/reporters/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.224513 django-pipelines-0.1.1/pipelines/results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/results/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/results/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/results/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.224513 django-pipelines-0.1.1/pipelines/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/runners/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.224513 django-pipelines-0.1.1/pipelines/runners/celery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/runners/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/runners/celery/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/runners/celery/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/runners/eager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.224513 django-pipelines-0.1.1/pipelines/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/tasks/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.200513 django-pipelines-0.1.1/pipelines/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.228513 django-pipelines-0.1.1/pipelines/templates/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templates/pipelines/_log_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templates/pipelines/_log_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templates/pipelines/_results_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templates/pipelines/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.228513 django-pipelines-0.1.1/pipelines/templates/pipelines/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templates/pipelines/includes/pipeline-result-listing.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.228513 django-pipelines-0.1.1/pipelines/templates/pipelines/includes/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templates/pipelines/includes/static/js.html
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templates/pipelines/includes/static/style.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templates/pipelines/includes/task-execution-listing.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templates/pipelines/includes/task-result-listing.html
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templates/pipelines/pipeline.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templates/pipelines/pipeline_execution_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templates/pipelines/pipeline_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templates/pipelines/pipeline_start.html
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templates/pipelines/results_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.228513 django-pipelines-0.1.1/pipelines/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/templatetags/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pipelines/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-14 15:07:29.236514 django-pipelines-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.228513 django-pipelines-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:29.228513 django-pipelines-0.1.1/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/tests/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/tests/meta/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-14 15:07:25.000000 django-pipelines-0.1.1/tests/urls.py
```

### Comparing `django-pipelines-0.1.0/LICENSE` & `django-pipelines-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/PKG-INFO` & `django-pipelines-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pipelines
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for building data pipelines with Django
 Home-page: https://github.com/wildfish/django-pipelines
 Author: Wildfish
 Author-email: developers@wildfish.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-pipelines-0.1.0/README.rst` & `django-pipelines-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/django_pipelines.egg-info/PKG-INFO` & `django-pipelines-0.1.1/django_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pipelines
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for building data pipelines with Django
 Home-page: https://github.com/wildfish/django-pipelines
 Author: Wildfish
 Author-email: developers@wildfish.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-pipelines-0.1.0/django_pipelines.egg-info/SOURCES.txt` & `django-pipelines-0.1.1/django_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/Makefile` & `django-pipelines-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/api/pipelines.rst` & `django-pipelines-0.1.1/docs/api/pipelines.rst`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/conf.py` & `django-pipelines-0.1.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "django-pipelines"
 copyright = "2023, Wildfish"
 author = "Wildfish"
-release = "0.1.0"
+release = "0.1.1"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ["sphinx.ext.autodoc"]
 
 templates_path = ["_templates"]
```

### Comparing `django-pipelines-0.1.0/docs/contributing.rst` & `django-pipelines-0.1.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/docs_dj_settings.py` & `django-pipelines-0.1.1/docs/docs_dj_settings.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/index.rst` & `django-pipelines-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/make.bat` & `django-pipelines-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/pipelines/howto/_images/quickstart_pipeline_executions.png` & `django-pipelines-0.1.1/docs/pipelines/howto/_images/quickstart_pipeline_executions.png`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/pipelines/howto/_images/quickstart_pipeline_results.png` & `django-pipelines-0.1.1/docs/pipelines/howto/_images/quickstart_pipeline_results.png`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/pipelines/howto/_images/quickstart_pipelines.png` & `django-pipelines-0.1.1/docs/pipelines/howto/_images/quickstart_pipelines.png`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/pipelines/howto/_images/quickstart_pipelines_command.gif` & `django-pipelines-0.1.1/docs/pipelines/howto/_images/quickstart_pipelines_command.gif`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/pipelines/howto/_images/quickstart_running_pipeline.gif` & `django-pipelines-0.1.1/docs/pipelines/howto/_images/quickstart_running_pipeline.gif`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/pipelines/howto/management-commands.rst` & `django-pipelines-0.1.1/docs/pipelines/howto/management-commands.rst`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/pipelines/howto/pipelines.rst` & `django-pipelines-0.1.1/docs/pipelines/howto/pipelines.rst`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/pipelines/howto/reporters.rst` & `django-pipelines-0.1.1/docs/pipelines/howto/reporters.rst`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/pipelines/howto/results.rst` & `django-pipelines-0.1.1/docs/pipelines/howto/results.rst`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/pipelines/howto/runners.rst` & `django-pipelines-0.1.1/docs/pipelines/howto/runners.rst`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/pipelines/howto/settings.rst` & `django-pipelines-0.1.1/docs/pipelines/howto/settings.rst`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/pipelines/howto/tasks.rst` & `django-pipelines-0.1.1/docs/pipelines/howto/tasks.rst`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/docs/pipelines/index.rst` & `django-pipelines-0.1.1/docs/pipelines/index.rst`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/admin.py` & `django-pipelines-0.1.1/pipelines/admin.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/baker_recipes.py` & `django-pipelines-0.1.1/pipelines/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/base.py` & `django-pipelines-0.1.1/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/config.py` & `django-pipelines-0.1.1/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/forms.py` & `django-pipelines-0.1.1/pipelines/forms.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/management/commands/clear_tasks_and_logs.py` & `django-pipelines-0.1.1/pipelines/management/commands/clear_tasks_and_logs.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/management/commands/pipelines.py` & `django-pipelines-0.1.1/pipelines/management/commands/pipelines.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/meta/__init__.py` & `django-pipelines-0.1.1/pipelines/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0001_initial.py` & `django-pipelines-0.1.1/pipelines/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0002_rename_last_run_pipelineexecution_started_and_more.py` & `django-pipelines-0.1.1/pipelines/migrations/0002_rename_last_run_pipelineexecution_started_and_more.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0003_alter_pipelineexecution_reporter_and_more.py` & `django-pipelines-0.1.1/pipelines/migrations/0003_alter_pipelineexecution_reporter_and_more.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0004_alter_pipelineexecution_options_and_more.py` & `django-pipelines-0.1.1/pipelines/migrations/0004_alter_pipelineexecution_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0004_alter_pipelineexecution_status.py` & `django-pipelines-0.1.1/pipelines/migrations/0004_alter_pipelineexecution_status.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0007_pipelineexecution_taskexecution_and_more.py` & `django-pipelines-0.1.1/pipelines/migrations/0007_pipelineexecution_taskexecution_and_more.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0008_auto_20230116_1208.py` & `django-pipelines-0.1.1/pipelines/migrations/0008_auto_20230116_1208.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0009_remove_pipelineresult_pipeline_id_and_more.py` & `django-pipelines-0.1.1/pipelines/migrations/0009_remove_pipelineresult_pipeline_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0010_remove_taskexecution_pipeline_and_more.py` & `django-pipelines-0.1.1/pipelines/migrations/0010_remove_taskexecution_pipeline_and_more.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0011_alter_taskresult_status.py` & `django-pipelines-0.1.1/pipelines/migrations/0011_alter_taskresult_status.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0012_remove_taskresult_pipeline_task_and_more.py` & `django-pipelines-0.1.1/pipelines/migrations/0012_remove_taskresult_pipeline_task_and_more.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0013_pipelineexecution_completed_pipelineresult_completed_and_more.py` & `django-pipelines-0.1.1/pipelines/migrations/0013_pipelineexecution_completed_pipelineresult_completed_and_more.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0014_remove_pipelineresult_input_data_and_more.py` & `django-pipelines-0.1.1/pipelines/migrations/0014_remove_pipelineresult_input_data_and_more.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0015_delete_tasklog_pipelinelog_context_id_and_more.py` & `django-pipelines-0.1.1/pipelines/migrations/0015_delete_tasklog_pipelinelog_context_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0018_rename_pipelineexecution_ormpipelineexecution_and_more.py` & `django-pipelines-0.1.1/pipelines/migrations/0018_rename_pipelineexecution_ormpipelineexecution_and_more.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0019_alter_ormpipelineexecution_completed_and_more.py` & `django-pipelines-0.1.1/pipelines/migrations/0019_alter_ormpipelineexecution_completed_and_more.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/migrations/0020_delete_valuestore_alter_pipelinelog_context_type.py` & `django-pipelines-0.1.1/pipelines/migrations/0020_delete_valuestore_alter_pipelinelog_context_type.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/models.py` & `django-pipelines-0.1.1/pipelines/models.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/registry.py` & `django-pipelines-0.1.1/pipelines/registry.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/reporters/base.py` & `django-pipelines-0.1.1/pipelines/reporters/base.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/reporters/orm.py` & `django-pipelines-0.1.1/pipelines/reporters/orm.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/results/base.py` & `django-pipelines-0.1.1/pipelines/results/base.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/results/helpers.py` & `django-pipelines-0.1.1/pipelines/results/helpers.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/results/orm.py` & `django-pipelines-0.1.1/pipelines/results/orm.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/runners/base.py` & `django-pipelines-0.1.1/pipelines/runners/base.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/runners/celery/runner.py` & `django-pipelines-0.1.1/pipelines/runners/celery/runner.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/runners/celery/tasks.py` & `django-pipelines-0.1.1/pipelines/runners/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/runners/eager.py` & `django-pipelines-0.1.1/pipelines/runners/eager.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/status.py` & `django-pipelines-0.1.1/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/tasks/base.py` & `django-pipelines-0.1.1/pipelines/tasks/base.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/tasks/registry.py` & `django-pipelines-0.1.1/pipelines/tasks/registry.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/templates/pipelines/base.html` & `django-pipelines-0.1.1/pipelines/templates/pipelines/base.html`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/templates/pipelines/includes/pipeline-result-listing.html` & `django-pipelines-0.1.1/pipelines/templates/pipelines/includes/pipeline-result-listing.html`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/templates/pipelines/includes/task-execution-listing.html` & `django-pipelines-0.1.1/pipelines/templates/pipelines/includes/task-execution-listing.html`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/templates/pipelines/includes/task-result-listing.html` & `django-pipelines-0.1.1/pipelines/templates/pipelines/includes/task-result-listing.html`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/templates/pipelines/pipeline_execution_list.html` & `django-pipelines-0.1.1/pipelines/templates/pipelines/pipeline_execution_list.html`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/templates/pipelines/pipeline_list.html` & `django-pipelines-0.1.1/pipelines/templates/pipelines/pipeline_list.html`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/templates/pipelines/pipeline_start.html` & `django-pipelines-0.1.1/pipelines/templates/pipelines/pipeline_start.html`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/templatetags/pipelines.py` & `django-pipelines-0.1.1/pipelines/templatetags/pipelines.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/urls.py` & `django-pipelines-0.1.1/pipelines/urls.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/utils.py` & `django-pipelines-0.1.1/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/pipelines/views.py` & `django-pipelines-0.1.1/pipelines/views.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/setup.cfg` & `django-pipelines-0.1.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-pipelines
-version = 0.1.0
+version = 0.1.1
 description = Tools for building data pipelines with Django
 long_description = file: README.rst
 url = https://github.com/wildfish/django-pipelines
 author = Wildfish
 author_email = developers@wildfish.com
 license = BSD-3-Clause
 classifiers =
```

### Comparing `django-pipelines-0.1.0/tests/conftest.py` & `django-pipelines-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/tests/meta/test_meta.py` & `django-pipelines-0.1.1/tests/meta/test_meta.py`

 * *Files identical despite different names*

### Comparing `django-pipelines-0.1.0/tests/settings.py` & `django-pipelines-0.1.1/tests/settings.py`

 * *Files identical despite different names*

