# Comparing `tmp/telescoop-backup-0.1.5.tar.gz` & `tmp/telescoop-backup-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telescoop-backup-0.1.5.tar", last modified: Wed Dec  7 14:29:45 2022, max compression
+gzip compressed data, was "telescoop-backup-0.1.6.tar", last modified: Fri Apr 14 14:22:48 2023, max compression
```

## Comparing `telescoop-backup-0.1.5.tar` & `telescoop-backup-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2022-12-07 14:29:45.163577 telescoop-backup-0.1.5/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1548 2022-08-01 08:44:48.000000 telescoop-backup-0.1.5/LICENSE
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2778 2022-12-07 14:29:45.163577 telescoop-backup-0.1.5/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1673 2022-08-01 08:44:48.000000 telescoop-backup-0.1.5/README.md
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1105 2022-12-07 14:29:45.163577 telescoop-backup-0.1.5/setup.cfg
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       38 2022-08-01 08:44:48.000000 telescoop-backup-0.1.5/setup.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2022-12-07 14:29:45.159577 telescoop-backup-0.1.5/telescoop_backup/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       56 2022-08-01 08:44:48.000000 telescoop-backup-0.1.5/telescoop_backup/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      160 2022-08-01 08:44:48.000000 telescoop-backup-0.1.5/telescoop_backup/apps.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     7870 2022-12-07 14:27:34.000000 telescoop-backup-0.1.5/telescoop_backup/backup.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2022-12-07 14:29:45.163577 telescoop-backup-0.1.5/telescoop_backup/management/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-08-01 08:44:48.000000 telescoop-backup-0.1.5/telescoop_backup/management/__init__.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2022-12-07 14:29:45.163577 telescoop-backup-0.1.5/telescoop_backup/management/commands/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-08-01 08:44:48.000000 telescoop-backup-0.1.5/telescoop_backup/management/commands/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1537 2022-08-01 08:44:48.000000 telescoop-backup-0.1.5/telescoop_backup/management/commands/backup_db.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1470 2022-08-01 08:44:48.000000 telescoop-backup-0.1.5/telescoop_backup/managers.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2022-12-07 14:29:45.163577 telescoop-backup-0.1.5/telescoop_backup/migrations/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-08-01 08:44:48.000000 telescoop-backup-0.1.5/telescoop_backup/migrations/__init__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1015 2022-08-01 08:44:48.000000 telescoop-backup-0.1.5/telescoop_backup/serializers.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      822 2022-08-01 08:44:48.000000 telescoop-backup-0.1.5/telescoop_backup/tests.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      233 2022-08-01 08:44:48.000000 telescoop-backup-0.1.5/telescoop_backup/urls.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      653 2022-08-01 08:44:48.000000 telescoop-backup-0.1.5/telescoop_backup/views.py
-drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2022-12-07 14:29:45.163577 telescoop-backup-0.1.5/telescoop_backup.egg-info/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     2778 2022-12-07 14:29:45.000000 telescoop-backup-0.1.5/telescoop_backup.egg-info/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      633 2022-12-07 14:29:45.000000 telescoop-backup-0.1.5/telescoop_backup.egg-info/SOURCES.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2022-12-07 14:29:45.000000 telescoop-backup-0.1.5/telescoop_backup.egg-info/dependency_links.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       40 2022-12-07 14:29:45.000000 telescoop-backup-0.1.5/telescoop_backup.egg-info/requires.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       17 2022-12-07 14:29:45.000000 telescoop-backup-0.1.5/telescoop_backup.egg-info/top_level.txt
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-14 14:22:48.256297 telescoop-backup-0.1.6/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1548 2022-08-01 08:44:48.000000 telescoop-backup-0.1.6/LICENSE
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2778 2023-04-14 14:22:48.256297 telescoop-backup-0.1.6/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1673 2022-08-01 08:44:48.000000 telescoop-backup-0.1.6/README.md
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1105 2023-04-14 14:22:48.256297 telescoop-backup-0.1.6/setup.cfg
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       38 2022-08-01 08:44:48.000000 telescoop-backup-0.1.6/setup.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-14 14:22:48.256297 telescoop-backup-0.1.6/telescoop_backup/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       56 2022-08-01 08:44:48.000000 telescoop-backup-0.1.6/telescoop_backup/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      160 2022-08-01 08:44:48.000000 telescoop-backup-0.1.6/telescoop_backup/apps.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     8198 2023-04-14 14:21:42.000000 telescoop-backup-0.1.6/telescoop_backup/backup.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-14 14:22:48.256297 telescoop-backup-0.1.6/telescoop_backup/management/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-08-01 08:44:48.000000 telescoop-backup-0.1.6/telescoop_backup/management/__init__.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-14 14:22:48.256297 telescoop-backup-0.1.6/telescoop_backup/management/commands/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-08-01 08:44:48.000000 telescoop-backup-0.1.6/telescoop_backup/management/commands/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1537 2022-08-01 08:44:48.000000 telescoop-backup-0.1.6/telescoop_backup/management/commands/backup_db.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1470 2022-08-01 08:44:48.000000 telescoop-backup-0.1.6/telescoop_backup/managers.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-14 14:22:48.256297 telescoop-backup-0.1.6/telescoop_backup/migrations/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        0 2022-08-01 08:44:48.000000 telescoop-backup-0.1.6/telescoop_backup/migrations/__init__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1015 2022-08-01 08:44:48.000000 telescoop-backup-0.1.6/telescoop_backup/serializers.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      822 2022-08-01 08:44:48.000000 telescoop-backup-0.1.6/telescoop_backup/tests.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      233 2022-08-01 08:44:48.000000 telescoop-backup-0.1.6/telescoop_backup/urls.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      653 2022-08-01 08:44:48.000000 telescoop-backup-0.1.6/telescoop_backup/views.py
+drwxrwxr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-14 14:22:48.256297 telescoop-backup-0.1.6/telescoop_backup.egg-info/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     2778 2023-04-14 14:22:48.000000 telescoop-backup-0.1.6/telescoop_backup.egg-info/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      633 2023-04-14 14:22:48.000000 telescoop-backup-0.1.6/telescoop_backup.egg-info/SOURCES.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2023-04-14 14:22:48.000000 telescoop-backup-0.1.6/telescoop_backup.egg-info/dependency_links.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       40 2023-04-14 14:22:48.000000 telescoop-backup-0.1.6/telescoop_backup.egg-info/requires.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       17 2023-04-14 14:22:48.000000 telescoop-backup-0.1.6/telescoop_backup.egg-info/top_level.txt
```

### Comparing `telescoop-backup-0.1.5/LICENSE` & `telescoop-backup-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `telescoop-backup-0.1.5/PKG-INFO` & `telescoop-backup-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telescoop-backup
-Version: 0.1.5
+Version: 0.1.6
 Summary: Django app to backup Sqlite or Postgres database to an S3 Object Storage.
 Home-page: https://gitlab.com/telescoop-public/django-apps/telescoop-backup
 Author: TelesCoop SARL SCOP
 Author-email: contact@telescoop.fr
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `telescoop-backup-0.1.5/README.md` & `telescoop-backup-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `telescoop-backup-0.1.5/setup.cfg` & `telescoop-backup-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = telescoop-backup
-version = 0.1.5
+version = 0.1.6
 description = Django app to backup Sqlite or Postgres database to an S3 Object Storage.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/telescoop-public/django-apps/telescoop-backup
 author = TelesCoop SARL SCOP
 author_email = contact@telescoop.fr
 license = BSD-3-Clause
```

### Comparing `telescoop-backup-0.1.5/telescoop_backup/backup.py` & `telescoop-backup-0.1.6/telescoop_backup/backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import shutil
 import subprocess
 
 from django.conf import settings
 
 import boto
+import boto.s3.connection
 from boto.s3.key import Key
 
 IS_POSTGRES = "postgresql" in settings.DATABASES["default"]["ENGINE"]
 
 DATE_FORMAT = "%Y-%m-%dT%H:%M"
 DEFAULT_AUTH_VERSION = 2
 DEFAULT_CONTAINER_NAME = "db-backups"
@@ -31,15 +32,22 @@
 if host is None:
     region = getattr(settings, "BACKUP_REGION", "eu-west-3")
     host = f"s3.{region}.amazonaws.com"
 LAST_BACKUP_FILE = os.path.join(settings.BASE_DIR, ".telescoop_backup_last_backup")
 
 
 def boto_connexion():
-    """Connect to AWS S3."""
+    """Connect to S3."""
+    if host.endswith("clever-cloud.com"):
+        return boto.s3.connection.S3Connection(
+            aws_access_key_id=settings.BACKUP_ACCESS,
+            aws_secret_access_key=settings.BACKUP_SECRET,
+            host=host,
+            calling_format=boto.s3.connection.OrdinaryCallingFormat(),
+        )
     return boto.connect_s3(
         settings.BACKUP_ACCESS,
         settings.BACKUP_SECRET,
         host=host,
     )
```

### Comparing `telescoop-backup-0.1.5/telescoop_backup/management/commands/backup_db.py` & `telescoop-backup-0.1.6/telescoop_backup/management/commands/backup_db.py`

 * *Files identical despite different names*

### Comparing `telescoop-backup-0.1.5/telescoop_backup/managers.py` & `telescoop-backup-0.1.6/telescoop_backup/managers.py`

 * *Files identical despite different names*

### Comparing `telescoop-backup-0.1.5/telescoop_backup/serializers.py` & `telescoop-backup-0.1.6/telescoop_backup/serializers.py`

 * *Files identical despite different names*

### Comparing `telescoop-backup-0.1.5/telescoop_backup/tests.py` & `telescoop-backup-0.1.6/telescoop_backup/tests.py`

 * *Files identical despite different names*

### Comparing `telescoop-backup-0.1.5/telescoop_backup/views.py` & `telescoop-backup-0.1.6/telescoop_backup/views.py`

 * *Files identical despite different names*

### Comparing `telescoop-backup-0.1.5/telescoop_backup.egg-info/PKG-INFO` & `telescoop-backup-0.1.6/telescoop_backup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telescoop-backup
-Version: 0.1.5
+Version: 0.1.6
 Summary: Django app to backup Sqlite or Postgres database to an S3 Object Storage.
 Home-page: https://gitlab.com/telescoop-public/django-apps/telescoop-backup
 Author: TelesCoop SARL SCOP
 Author-email: contact@telescoop.fr
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `telescoop-backup-0.1.5/telescoop_backup.egg-info/SOURCES.txt` & `telescoop-backup-0.1.6/telescoop_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

