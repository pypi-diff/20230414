# Comparing `tmp/terka-1.4.0.tar.gz` & `tmp/terka-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.4.0.tar", last modified: Wed Apr 12 20:26:26 2023, max compression
+gzip compressed data, was "terka-1.5.0.tar", last modified: Thu Apr 13 22:12:04 2023, max compression
```

## Comparing `terka-1.4.0.tar` & `terka-1.5.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.292028 terka-1.4.0/
--rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.4.0/LICENSE
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-12 20:26:26.292028 terka-1.4.0/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.4.0/README.md
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-12 20:26:26.292028 terka-1.4.0/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-12 20:25:42.000000 terka-1.4.0/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.288028 terka-1.4.0/src/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.4.0/src/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.288028 terka-1.4.0/src/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.4.0/src/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    15295 2023-04-12 20:19:39.000000 terka-1.4.0/src/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.4.0/src/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.292028 terka-1.4.0/src/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.4.0/src/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.4.0/src/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    36138 2023-04-12 20:18:40.000000 terka-1.4.0/src/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.4.0/src/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.4.0/src/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.4.0/src/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.4.0/src/domain/event_history.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.4.0/src/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.4.0/src/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     1805 2023-04-05 14:05:47.000000 terka-1.4.0/src/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.4.0/src/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.4.0/src/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.4.0/src/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.4.0/src/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.4.0/src/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.292028 terka-1.4.0/src/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.4.0/src/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     4257 2023-04-08 19:24:05.000000 terka-1.4.0/src/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.292028 terka-1.4.0/src/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.4.0/src/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    27188 2023-04-12 20:20:05.000000 terka-1.4.0/src/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.4.0/src/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.4.0/src/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.4.0/src/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     6929 2023-04-12 19:45:59.000000 terka-1.4.0/src/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.292028 terka-1.4.0/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-12 20:26:26.000000 terka-1.4.0/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-12 20:26:26.000000 terka-1.4.0/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-12 20:26:26.000000 terka-1.4.0/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-12 20:26:26.000000 terka-1.4.0/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-12 20:26:26.000000 terka-1.4.0/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-12 20:26:26.000000 terka-1.4.0/terka.egg-info/top_level.txt
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-12 20:26:26.292028 terka-1.4.0/tests/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.4.0/tests/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.4.0/tests/conftest.py
--rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.4.0/tests/test_commands.py
--rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.4.0/tests/test_orm.py
--rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.4.0/tests/test_task.py
--rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.4.0/tests/test_user.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.4.0/tests/test_utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-13 22:12:04.166894 terka-1.5.0/
+-rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.5.0/LICENSE
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-13 22:12:04.166894 terka-1.5.0/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.5.0/README.md
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-13 22:12:04.166894 terka-1.5.0/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      872 2023-04-13 22:10:56.000000 terka-1.5.0/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-13 22:12:04.162894 terka-1.5.0/src/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.0/src/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-13 22:12:04.162894 terka-1.5.0/src/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.0/src/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    15295 2023-04-12 20:19:39.000000 terka-1.5.0/src/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.5.0/src/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-13 22:12:04.162894 terka-1.5.0/src/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.0/src/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.5.0/src/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    36636 2023-04-13 22:07:45.000000 terka-1.5.0/src/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.5.0/src/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.5.0/src/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.5.0/src/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.5.0/src/domain/event_history.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.5.0/src/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.5.0/src/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     1805 2023-04-05 14:05:47.000000 terka-1.5.0/src/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.5.0/src/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.5.0/src/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.5.0/src/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.5.0/src/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.5.0/src/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-13 22:12:04.162894 terka-1.5.0/src/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.5.0/src/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     4257 2023-04-08 19:24:05.000000 terka-1.5.0/src/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-13 22:12:04.162894 terka-1.5.0/src/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.0/src/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    27914 2023-04-13 22:08:31.000000 terka-1.5.0/src/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.5.0/src/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.5.0/src/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.5.0/src/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     7088 2023-04-13 19:08:12.000000 terka-1.5.0/src/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-13 22:12:04.166894 terka-1.5.0/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-13 22:12:04.000000 terka-1.5.0/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      976 2023-04-13 22:12:04.000000 terka-1.5.0/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-13 22:12:04.000000 terka-1.5.0/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-13 22:12:04.000000 terka-1.5.0/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       37 2023-04-13 22:12:04.000000 terka-1.5.0/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-13 22:12:04.000000 terka-1.5.0/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-13 22:12:04.166894 terka-1.5.0/tests/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.5.0/tests/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.5.0/tests/conftest.py
+-rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.5.0/tests/test_commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.5.0/tests/test_orm.py
+-rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.5.0/tests/test_task.py
+-rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.5.0/tests/test_user.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.5.0/tests/test_utils.py
```

### Comparing `terka-1.4.0/LICENSE` & `terka-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/PKG-INFO` & `terka-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.4.0
+Version: 1.5.0
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.4.0/README.md` & `terka-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/setup.py` & `terka-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.4.0",
+    version="1.5.0",
     description="CLI utility for creating and managing tasks in a terminal",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.4.0/src/adapters/orm.py` & `terka-1.5.0/src/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/adapters/repository.py` & `terka-1.5.0/src/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/domain/collaborators.py` & `terka-1.5.0/src/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/domain/commands.py` & `terka-1.5.0/src/domain/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,15 +199,20 @@
         else:
             entity = None
         if not entity and command not in ("init", "unfocus", "log", "calendar",
                                           "help"):
             raise ValueError(f"Entity *{entity_type}* is not a valid entity")
         command = format_command(command)
         if command == "list":
-            show_completed = False
+            print_options = printer.PrintOptions(
+                show_tasks=False,
+                show_history=bool(kwargs.get("show_history")),
+                show_commentaries=bool(kwargs.get("show_commentaries")),
+                show_completed=bool(kwargs.get("show_completed"))
+            )
             if entity_type == "tasks":
                 if "status" not in kwargs and "all" not in kwargs:
                     kwargs["status"] = "BACKLOG,TODO,IN_PROGRESS,REVIEW"
                 else:
                     if "all" in kwargs:
                         del kwargs["all"]
                     show_completed = True
@@ -268,39 +273,39 @@
                         )
                         exit()
                 else:
                     self.console.print(
                         f"[red]No tag '{tag_text}' found![/red]")
                     exit()
             entities = self.repo.list(entity, kwargs)
-            if entity_type == "sprints":
-                self.printer.print_sprint(entities=entities,
-                                          repo=self.repo,
-                                          show_tasks=False)
-                exit()
-            if entity_type == "epics":
-                self.printer.print_epic(entities=entities,
-                                        repo=self.repo,
-                                        show_tasks=False)
-                exit()
+            # if entity_type == "sprints":
+            #     self.printer.print_sprint(entities=entities,
+            #                               repo=self.repo,
+            #                               show_tasks=False)
+            #     exit()
+            # if entity_type == "epics":
+            #     self.printer.print_epic(entities=entities,
+            #                             repo=self.repo,
+            #                             show_tasks=False)
+            #     exit()
             if custom_sort == "due_date":
                 entities_with_due_date = []
                 entities_without_due_date = []
                 for entity in entities:
                     if entity.due_date:
                         entities_with_due_date.append(entity)
                 entities_with_due_date.sort(key=lambda c: c.due_date,
                                             reverse=False)
                 entities = entities_with_due_date
             session.commit()
             self.printer.print_entities(entities,
                                         entity_type,
                                         self.repo,
                                         custom_sort,
-                                        show_completed=show_completed)
+                                        print_options=print_options)
             logger.info("<list> %s", entity_type)
             return entities, None, None
         elif command == "help":
             print("""
             available commands: 'list', 'show', 'create', 'update', 'done', 'calendar', 'log', 'edit'
             available entities: 'tasks', 'projects', 'commentaries'
             """)
@@ -631,19 +636,20 @@
                 else:
                     sprint_task_id = None
                 if story_points := kwargs.get("story_points"):
                     if not sprint_task_id:
                         sprint_task = self.execute("get", "sprint_tasks",
                                                    {"task": task_id})
                         if not sprint_task:
-                            exit(f"Task id {task_id} is not part of any sprint")
+                            exit(
+                                f"Task id {task_id} is not part of any sprint")
                         else:
                             sprint_task_id = sprint_task[0].id
                     self.repo.update(SprintTask, sprint_task_id,
-                                         {"story_points": story_points})
+                                     {"story_points": story_points})
             session.commit()
         elif command == "create":
             kwargs["created_by"] = services.lookup_user_id(
                 self.config.get("user"), self.repo)
             obj = entity(**kwargs)
             if entity in (Task, Project):
                 if (existing_obj := self.repo.list(entity,
@@ -775,24 +781,28 @@
                 task_params = {"id": task.id}
                 if task.status.name == "BACKLOG":
                     task_params.update({"status": "TODO"})
                 if not task.due_date or task.due_date > sprint.end_date:
                     task_params.update({"due_date": sprint.end_date})
                 self.execute("update", "tasks", task_params)
         elif command == "show":
-            show_completed = bool(kwargs.get("show_completed"))
+            print_options = printer.PrintOptions(
+                show_history=bool(kwargs.get("show_history")),
+                show_commentaries=bool(kwargs.get("show_commentaries")),
+                show_completed=bool(kwargs.get("show_completed"))
+            )
             if (task_id := kwargs.get("id")):
                 tasks = get_ids(task_id)
                 for task in tasks:
                     if task.isdigit():
                         entities = self.repo.list(entity, {"id": task})
                     else:
                         entities = self.repo.list(entity, {"name": task})
-                    self.printer.print_entity(entity_type, entities, self.repo,
-                                              show_completed)
+                    self.printer.print_entity(
+                        task, entity_type, entities, self.repo, print_options)
                     logger.info("<show> %s: %s", entity_type, task_id)
                 return entities, None, None
         elif command == "done":
             if entity_type not in ("tasks", "sprints"):
                 raise ValueError("can complete only tasks and sprints")
             elif entity_type == "tasks":
                 kwargs.update({"status": "DONE"})
```

### Comparing `terka-1.4.0/src/domain/commentary.py` & `terka-1.5.0/src/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/domain/epic.py` & `terka-1.5.0/src/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/domain/event_history.py` & `terka-1.5.0/src/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/domain/project.py` & `terka-1.5.0/src/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/domain/sprint.py` & `terka-1.5.0/src/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/domain/story.py` & `terka-1.5.0/src/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/domain/tag.py` & `terka-1.5.0/src/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/domain/task.py` & `terka-1.5.0/src/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/domain/time_tracker.py` & `terka-1.5.0/src/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/domain/user.py` & `terka-1.5.0/src/domain/user.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/entrypoints/cli.py` & `terka-1.5.0/src/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/service_layer/printer.py` & `terka-1.5.0/src/service_layer/printer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 from typing import Any, Dict, List, Tuple
+from dataclasses import dataclass
 
 from collections import defaultdict
 from datetime import datetime, date, timedelta
 import rich
 from rich.console import Console
 from rich.table import Table
 from statistics import mean, median
 
 from src.service_layer import services
 from src.service_layer.ui import TerkaTask
 
 
+@dataclass
+class PrintOptions:
+    show_tasks: bool = True
+    show_history: bool = False
+    show_commentaries: bool = False
+    show_completed: bool = False
+
+
 class Printer:
 
     def __init__(self, repo, box=rich.box.SIMPLE) -> None:
         self.console = Console()
         self.box = box
         self.repo = repo
 
@@ -43,74 +52,79 @@
         for column in ("date", "text"):
             table.add_column(column)
         entities.sort(key=lambda c: c.date, reverse=False)
         for event in entities:
             table.add_row(event.date.strftime("%Y-%m-%d %H:%M"), event.text)
         self.console.print(table)
 
-    def print_entity(self, entity_type, entities, repo, show_completed):
+    def print_entity(self,
+                     task,
+                     entity_type,
+                     entities,
+                     repo,
+                     print_options: PrintOptions = PrintOptions()):
         if entity_type == "sprints":
             if entities:
-                self.print_sprint(entities, repo)
+                self.print_sprint(entities, repo, print_options)
             else:
                 exit(f"No sprint with id '{task}' found!")
         if entity_type == "epics":
             if entities:
-                self.print_epic(entities, repo)
+                self.print_epic(entities, repo, print_options)
             else:
                 exit(f"No epic with id '{task}' found!")
         if entity_type == "stories":
             if entities:
-                self.print_story(entities, repo)
+                self.print_story(entities, repo, print_options)
             else:
                 exit(f"No story with id '{task}' found!")
         if entity_type == "projects":
             if entities:
-                self.print_project(entities,
-                                   show_completed_tasks=show_completed)
+                self.print_project(entities, print_options)
             else:
                 exit(f"No project '{task}' found!")
         if entity_type == "tasks":
             if entities:
-                self.print_task(entities, repo, show_completed=show_completed)
+                self.print_task(entities, repo, print_options)
             else:
                 print(f"No task with id '{task}' found!")
 
-    def print_entities(self,
-                       entities,
-                       type,
-                       repo,
-                       custom_sort,
-                       show_completed=False):
+    def print_entities(self, entities, type, repo, custom_sort, print_options):
         if type == "projects":
             entities.sort(key=self._sort_open_tasks, reverse=True)
-            self.print_project(entities, show_tasks=False)
+            self.print_project(entities, print_options)
         elif type == "tasks":
             if custom_sort:
                 entities.sort(key=lambda c: getattr(c, custom_sort),
                               reverse=False)
             else:
                 entities.sort(key=lambda c:
                               (c.status.value, c.priority.value
                                if hasattr(c.priority, "value") else 0),
                               reverse=True)
             self.print_task(entities=entities,
                             repo=repo,
-                            show_completed=show_completed,
+                            print_options=print_options,
                             custom_sort=custom_sort)
         elif type == "tags":
             self.print_tag(entities=entities)
         elif type == "users":
             self.print_user(entities=entities)
         elif type == "sprints":
-            self.print_sprint(entities=entities, repo=repo)
+            self.print_sprint(entities=entities,
+                              repo=repo,
+                              print_options=print_options)
         elif type == "epics":
-            self.print_epic(entities=entities, repo=repo)
+            self.print_epic(entities=entities,
+                            repo=repo,
+                            print_options=print_options)
         elif type == "stories":
-            self.print_story(entities=entities, repo=repo)
+            self.print_story(entities=entities,
+                             repo=repo,
+                             print_options=print_options)
         else:
             self.print_default_entity(self, entities)
 
     def print_user(self, entities):
         table = Table(box=self.box)
         for column in ("id", "name"):
             table.add_column(column)
@@ -137,15 +151,15 @@
         for column in ("id", "date", "text"):
             table.add_column(column)
         for entity in entities:
             table.add_row(f"[red]{entity.id}[/red]",
                           entity.date.strftime("%Y-%m-%d %H:%M"), entity.text)
         self.console.print(table)
 
-    def print_epic(self, entities, repo, show_tasks=True):
+    def print_epic(self, entities, repo, print_options):
         table = Table(box=self.box, title="EPICS", expand=True)
         for column in ("id", "name", "description", "project", "tasks"):
             table.add_column(column, style="bold")
         for i, entity in enumerate(entities):
             tasks = []
             for epic_task in entity.epic_tasks:
                 task = epic_task.tasks
@@ -155,24 +169,24 @@
                     entity.project, repo)
                 project = project_obj.name
             except:
                 project = None
             table.add_row(f"E{entity.id}", str(entity.name),
                           entity.description, project, str(len(tasks)))
         self.console.print(table)
-        if show_tasks:
+        if print_options.show_tasks:
             self.print_task(entities=tasks,
                             repo=repo,
-                            show_completed=True,
-                            show_window=False,
-                            show_history_comments=False)
-        if i == 0 and (commentaries := entity.commentaries):
+                            print_options=print_options,
+                            show_window=False)
+        if i == 0 and print_options.show_commentaries and (
+                commentaries := entity.commentaries):
             self.print_commentaries(commentaries)
 
-    def print_story(self, entities, repo, show_tasks=True):
+    def print_story(self, entities, repo, print_options):
         table = Table(box=self.box, title="STORIES", expand=True)
         for column in ("id", "name", "description", "project", "tasks"):
             table.add_column(column, style="bold")
         for i, entity in enumerate(entities):
             tasks = []
             for story_task in entity.story_tasks:
                 task = story_task.tasks
@@ -182,24 +196,24 @@
                     entity.project, repo)
                 project = project_obj.name
             except:
                 project = None
             table.add_row(f"S{entity.id}", str(entity.name),
                           entity.description, project, str(len(tasks)))
         self.console.print(table)
-        if show_tasks and tasks:
+        if print_options.show_tasks and tasks:
             self.print_task(entities=tasks,
                             repo=repo,
-                            show_completed=True,
-                            show_window=False,
-                            show_history_comments=False)
-        if i == 0 and (commentaries := entity.commentaries):
+                            print_options=print_options,
+                            show_window=False)
+        if i == 0 and print_options.show_commentaries and (
+                commentaries := entity.commentaries):
             self.print_commentaries(commentaries)
 
-    def print_sprint(self, entities, repo, show_tasks=True):
+    def print_sprint(self, entities, repo, print_options):
         table = Table(box=rich.box.SQUARE_DOUBLE_HEAD)
         for column in ("id", "start_date", "end_date", "goal", "status",
                        "open tasks", "tasks", "velocity", "collaborators",
                        "time_spent"):
             table.add_column(column)
         for i, entity in enumerate(entities):
             story_points = []
@@ -232,31 +246,33 @@
                 for entry in task.time_spent
             ])
 
             time_spent = self._format_time_spent(time_spent_sum)
             table.add_row(str(entity.id), str(entity.start_date),
                           str(entity.end_date), entity.goal,
                           entity.status.name, str(len(open_tasks)),
-                          str(len(tasks)), str(round(sum(story_points), 2)),
-                          collaborators_string, str(time_spent))
+                          str(len(tasks)), str(round(sum(story_points),
+                                                     2)), collaborators_string,
+                          str(time_spent))
         self.console.print(table)
-        if show_tasks:
+        if print_options.show_tasks:
             self.print_sprint_task(entities=tasks,
                                    repo=repo,
-                                   show_completed=True,
+                                   show_completed=print_options.show_completed,
                                    story_points=story_points)
-        if i == 0 and (commentaries := entity.commentaries):
+        if i == 0 and print_options.show_commentaries and (
+                commentaries := entity.commentaries):
             self.print_commentaries(commentaries)
 
-    def print_project(self,
-                      entities,
-                      zero_tasks: bool = False,
-                      zero_tasks_only: bool = False,
-                      show_tasks: bool = True,
-                      show_completed_tasks: bool = False):
+    def print_project(
+        self,
+        entities,
+        # zero_tasks: bool = False,
+        # zero_tasks_only: bool = False,
+        print_options):
         table = Table(box=rich.box.SQUARE_DOUBLE_HEAD, expand=True)
         non_active_projects = Table(box=rich.box.SQUARE_DOUBLE_HEAD)
         for column in ("id", "name", "description", "status", "open_tasks",
                        "overdue", "backlog", "todo", "in_progress", "review",
                        "done", "median_task_age"):
             table.add_column(column)
         for column in ("id", "name", "description", "status", "open_tasks"):
@@ -278,15 +294,15 @@
                 backlog = self._count_task_status(entity.tasks, "BACKLOG")
                 todo = self._count_task_status(entity.tasks, "TODO")
                 in_progress = self._count_task_status(entity.tasks,
                                                       "IN_PROGRESS")
                 review = self._count_task_status(entity.tasks, "REVIEW")
                 done = self._count_task_status(entity.tasks, "DONE")
 
-                if zero_tasks or len(overdue_tasks) > 0:
+                if overdue_tasks:
                     entity_id = f"[red]{entity.id}[/red]"
                 else:
                     entity_id = f"[green]{entity.id}[/green]"
                 table.add_row(f"{entity_id}", entity.name, entity.description,
                               entity.status.name, str(open_tasks),
                               str(len(overdue_tasks)), str(backlog), str(todo),
                               str(in_progress), str(review), str(done),
@@ -297,30 +313,30 @@
                                             entity.status.name,
                                             str(open_tasks))
 
         self.console.print(table)
         if non_active_projects.row_count:
             self.console.print("[green]Inactive projects[/green]")
             self.console.print(non_active_projects)
-        if show_tasks:
+        if print_options.show_tasks:
             if epics := entity.epics:
                 self.console.print("")
-                self.print_epic(epics, self.repo, show_tasks=False)
+                self.print_epic(epics, self.repo, print_options)
             if stories := entity.stories:
                 self.console.print("")
-                self.print_story(stories, self.repo, show_tasks=False)
+                self.print_story(stories, self.repo, print_options)
             if tasks := entity.tasks:
                 self.print_task(entities=tasks,
                                 repo=self.repo,
-                                show_completed=show_completed_tasks,
-                                show_window=False,
-                                show_history_comments=False)
-        if commentaries := entity.commentaries:
+                                print_options=print_options,
+                                show_window=False)
+        if print_options.show_commentaries and (commentaries :=
+                                                entity.commentaries):
             self.print_commentaries(commentaries)
-        if history := entity.history:
+        if print_options.show_history and (history := entity.history):
             self.print_history(history)
 
     def print_sprint_task(self,
                           entities,
                           repo,
                           show_completed=False,
                           history=None,
@@ -441,18 +457,17 @@
                               str(entity.due_date), tag_string,
                               collaborator_string, str(time_spent))
             self.console.print(table)
 
     def print_task(self,
                    entities,
                    repo,
-                   show_completed=False,
+                   print_options,
                    custom_sort=None,
-                   show_window=True,
-                   show_history_comments=True):
+                   show_window=True):
         table = Table(box=self.box, title="TASKS")
         default_columns = ("id", "name", "description", "status", "priority",
                            "project", "due_date", "tags", "collaborators",
                            "time_spent")
         #TODO: Add printing for only a single task
         # if (entities[0].status.name == "DONE"):
         #     console.print(f"[green]task is completed on [/green]")
@@ -497,34 +512,36 @@
             priority = entity.priority.name if hasattr(entity.priority,
                                                        "name") else "UNKNOWN"
             time_spent = self._calculate_time_spent(entity)
             if entity.status.name in ("DELETED", "DONE"):
                 completed_tasks.append(entity)
                 continue
             printable_entities += 1
-            entity_name = f"{entity.name}"
+            entity_name = f"{entity.name}" if not comments else f"{entity.name} [blue][{len(comments)}][/blue]"
             if entity.due_date and entity.due_date <= date.today():
-                table.add_row(f"[red]{entity.id}[/red]", entity_name,
-                              entity.description, entity.status.name, priority,
-                              project, str(entity.due_date), tag_string,
-                              collaborator_string, str(time_spent))
-            else:
-                table.add_row(str(entity.id), entity_name, entity.description,
-                              entity.status.name, priority, project,
-                              str(entity.due_date), tag_string,
-                              collaborator_string, str(time_spent))
+                entity_id = f"[red]{entity.id}[/red]"
+            elif (event_history := entity.history) and entity.status.name in (
+                    "TODO", "IN_PROGRESS", "REVIEW"):
+                if max([event.date for event in event_history]) < (datetime.today() - timedelta(days=5)):
+                    entity_id = f"[yellow]{entity.id}[/yellow]"
+            else:
+                entity_id = str(entity.id)
+            table.add_row(entity_id, entity_name, entity.description,
+                          entity.status.name, priority, project,
+                          str(entity.due_date), tag_string,
+                          collaborator_string, str(time_spent))
         if printable_entities:
             if printable_entities == 1 and show_window:
                 app = TerkaTask(entity=entity,
                                 project=project,
                                 history=history,
                                 commentaries=comments)
                 app.run()
             self.console.print(table)
-        if show_completed and completed_tasks:
+        if print_options.show_completed and completed_tasks:
             table = Table(box=self.box)
             for column in default_columns:
                 table.add_column(column)
             self.console.print(f"[green]****COMPLETED TASKS*****[/green]")
             for entity in completed_tasks:
                 time_spent = self._calculate_time_spent(entity)
                 table.add_row(str(entity.id), entity.name, entity.description,
@@ -537,19 +554,19 @@
             app = TerkaTask(entity=entities[0],
                             project=project,
                             is_completed=True,
                             history=history,
                             commentaries=comments)
             app.run()
             exit()
-        if show_history_comments:
-            if commentaries := entity.commentaries:
-                self.print_commentaries(commentaries)
-            if history := entity.history:
-                self.print_history(history)
+        if print_options.show_commentaries and (commentaries :=
+                                                entity.commentaries):
+            self.print_commentaries(commentaries)
+        if print_options.show_history and (history := entity.history):
+            self.print_history(history)
 
     def _get_attributes(self, obj) -> List[Tuple[str, str]]:
         import inspect
         attributes = []
         for name, value in inspect.getmembers(obj):
             if not name.startswith("_") and not inspect.ismethod(value):
                 if not value:
```

### Comparing `terka-1.4.0/src/service_layer/services.py` & `terka-1.5.0/src/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/service_layer/ui.py` & `terka-1.5.0/src/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/service_layer/vertical_layout.css` & `terka-1.5.0/src/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/src/utils.py` & `terka-1.5.0/src/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
             convert_date(new_dict.get("end-date")),
             "sprint_id": new_dict.get("to-sprint") or new_dict.get("from-sprint") or new_dict.get("sprint"),
             "story_id": new_dict.get("to-story") or new_dict.get("from-story") or new_dict.get("story"),
             "epic_id": new_dict.get("to-epic") or new_dict.get("from-epic") or new_dict.get("epic"),
             "story_points": new_dict.get("story-points"),
             "hours": new_dict.get("H"),
             "minutes": new_dict.get("M"),
+            "show_history": new_dict.get("show-history"),
+            "show_commentaries": new_dict.get("show-commentaries") or new_dict.get("show-comments"),
         }
         if "--show-completed" in kwargs:
             task_dict.update({"show_completed": True})
         if "--sort" in kwargs:
             sort_statement = kwargs[kwargs.index("--sort"):]
             task_dict.update(create_task_dict(sort_statement))
     elif len(kwargs) == 1:
```

### Comparing `terka-1.4.0/terka.egg-info/PKG-INFO` & `terka-1.5.0/terka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.4.0
+Version: 1.5.0
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.4.0/terka.egg-info/SOURCES.txt` & `terka-1.5.0/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/tests/test_orm.py` & `terka-1.5.0/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/tests/test_task.py` & `terka-1.5.0/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `terka-1.4.0/tests/test_user.py` & `terka-1.5.0/tests/test_user.py`

 * *Files identical despite different names*

