# Comparing `tmp/django-webdav-ui-0.0.1.tar.gz` & `tmp/django-webdav-ui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webdav-ui-0.0.1.tar", last modified: Fri Apr 14 07:19:25 2023, max compression
+gzip compressed data, was "django-webdav-ui-0.0.2.tar", last modified: Fri Apr 14 07:32:43 2023, max compression
```

## Comparing `django-webdav-ui-0.0.1.tar` & `django-webdav-ui-0.0.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:19:25.030326 django-webdav-ui-0.0.1/
--rw-r--r--   0 chen      (1000) chen      (1000)     1063 2022-05-11 08:29:55.000000 django-webdav-ui-0.0.1/LICENSE
--rw-r--r--   0 chen      (1000) chen      (1000)      144 2023-04-14 07:09:15.000000 django-webdav-ui-0.0.1/MANIFEST.in
--rw-r--r--   0 chen      (1000) chen      (1000)     1937 2023-04-14 07:19:25.030326 django-webdav-ui-0.0.1/PKG-INFO
--rw-r--r--   0 chen      (1000) chen      (1000)     1070 2023-04-14 07:17:16.000000 django-webdav-ui-0.0.1/README.rst
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:19:25.023659 django-webdav-ui-0.0.1/django_webdav_ui.egg-info/
--rw-r--r--   0 chen      (1000) chen      (1000)     1937 2023-04-14 07:19:24.000000 django-webdav-ui-0.0.1/django_webdav_ui.egg-info/PKG-INFO
--rw-r--r--   0 chen      (1000) chen      (1000)     2161 2023-04-14 07:19:24.000000 django-webdav-ui-0.0.1/django_webdav_ui.egg-info/SOURCES.txt
--rw-r--r--   0 chen      (1000) chen      (1000)        1 2023-04-14 07:19:24.000000 django-webdav-ui-0.0.1/django_webdav_ui.egg-info/dependency_links.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       57 2023-04-14 07:19:24.000000 django-webdav-ui-0.0.1/django_webdav_ui.egg-info/requires.txt
--rw-r--r--   0 chen      (1000) chen      (1000)        7 2023-04-14 07:19:24.000000 django-webdav-ui-0.0.1/django_webdav_ui.egg-info/top_level.txt
--rw-r--r--   0 chen      (1000) chen      (1000)      108 2023-04-14 07:13:23.000000 django-webdav-ui-0.0.1/pyproject.toml
--rw-r--r--   0 chen      (1000) chen      (1000)      928 2023-04-14 07:19:25.033659 django-webdav-ui-0.0.1/setup.cfg
--rw-r--r--   0 chen      (1000) chen      (1000)       38 2023-04-14 07:09:55.000000 django-webdav-ui-0.0.1/setup.py
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:19:25.026992 django-webdav-ui-0.0.1/webdav/
--rw-r--r--   0 chen      (1000) chen      (1000)     1038 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.1/webdav/__init__.py
--rw-r--r--   0 chen      (1000) chen      (1000)      886 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.1/webdav/admin.py
--rw-r--r--   0 chen      (1000) chen      (1000)     7242 2022-05-11 10:10:04.000000 django-webdav-ui-0.0.1/webdav/apis.py
--rw-r--r--   0 chen      (1000) chen      (1000)      198 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.1/webdav/apps.py
--rw-r--r--   0 chen      (1000) chen      (1000)    13625 2022-05-11 10:14:26.000000 django-webdav-ui-0.0.1/webdav/client.py
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:19:25.026992 django-webdav-ui-0.0.1/webdav/components/
--rw-r--r--   0 chen      (1000) chen      (1000)       71 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/README.md
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:19:25.030326 django-webdav-ui-0.0.1/webdav/components/components/
--rw-r--r--   0 chen      (1000) chen      (1000)      896 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/ActivityBox.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)      745 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/ActivityLine.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     1087 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/BatchButton.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     2291 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/CommentBox.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)      640 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/CommentLine.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)      653 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/CreateFolderButton.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     2467 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/CreateFolderDialog.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     1833 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/DavBody.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)      882 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/DirectoryBreadcrumbs.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)      618 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/DownloadMenu.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     1837 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/FileActions.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     1667 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/FileDeleteDialog.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)      778 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/FileDeleteMenu.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     2077 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/FileName.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     1800 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/FilePreview.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)      952 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/FileSummary.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     5064 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/FilesTable.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     2731 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/LeftPanel.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)      943 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/Preview.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     2677 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/RenameDialog.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)      890 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/RenameMenu.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     3058 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/ShareBox.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     1711 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/Sidebar.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)      429 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/components/Topbar.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     1480 2023-04-14 07:06:17.000000 django-webdav-ui-0.0.1/webdav/components/components/UploadButton.jsx
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:19:25.030326 django-webdav-ui-0.0.1/webdav/components/context/
--rw-r--r--   0 chen      (1000) chen      (1000)      467 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/context/batch.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)      953 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/context/directory-context.jsx
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:19:25.030326 django-webdav-ui-0.0.1/webdav/components/utils/
--rw-r--r--   0 chen      (1000) chen      (1000)     1295 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.1/webdav/components/utils/utils.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)     1247 2023-04-14 06:58:30.000000 django-webdav-ui-0.0.1/webdav/components/webdav.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)      257 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.1/webdav/filters.py
--rw-r--r--   0 chen      (1000) chen      (1000)      165 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.1/webdav/forms.py
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:19:25.030326 django-webdav-ui-0.0.1/webdav/migrations/
--rw-r--r--   0 chen      (1000) chen      (1000)     2519 2022-05-11 08:36:39.000000 django-webdav-ui-0.0.1/webdav/migrations/0001_initial.py
--rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.1/webdav/migrations/__init__.py
--rw-r--r--   0 chen      (1000) chen      (1000)     1929 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.1/webdav/models.py
--rw-r--r--   0 chen      (1000) chen      (1000)     1156 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.1/webdav/receivers.py
--rw-r--r--   0 chen      (1000) chen      (1000)     2566 2022-05-11 10:25:23.000000 django-webdav-ui-0.0.1/webdav/serializers.py
--rw-r--r--   0 chen      (1000) chen      (1000)      108 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.1/webdav/signals.py
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:19:25.023659 django-webdav-ui-0.0.1/webdav/static/
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:19:25.030326 django-webdav-ui-0.0.1/webdav/static/webdav/
--rw-r--r--   0 chen      (1000) chen      (1000)   206620 2022-05-12 01:20:54.000000 django-webdav-ui-0.0.1/webdav/static/webdav/bulma.min.css
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:19:25.030326 django-webdav-ui-0.0.1/webdav/static/webdav/dist/
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:19:25.030326 django-webdav-ui-0.0.1/webdav/static/webdav/dist/assets/
--rw-r--r--   0 chen      (1000) chen      (1000)   412754 2023-04-14 07:08:19.000000 django-webdav-ui-0.0.1/webdav/static/webdav/dist/assets/webdav-07e1678a.js
--rw-r--r--   0 chen      (1000) chen      (1000)      133 2023-04-14 07:08:19.000000 django-webdav-ui-0.0.1/webdav/static/webdav/dist/manifest.json
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:19:25.023659 django-webdav-ui-0.0.1/webdav/templates/
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:19:25.030326 django-webdav-ui-0.0.1/webdav/templates/webdav/
--rw-r--r--   0 chen      (1000) chen      (1000)     1253 2023-04-14 07:03:34.000000 django-webdav-ui-0.0.1/webdav/templates/webdav/base.html
--rw-r--r--   0 chen      (1000) chen      (1000)      301 2023-04-14 07:00:49.000000 django-webdav-ui-0.0.1/webdav/templates/webdav/index.html
--rw-r--r--   0 chen      (1000) chen      (1000)      436 2022-05-12 01:18:51.000000 django-webdav-ui-0.0.1/webdav/templates/webdav/share.html
--rw-r--r--   0 chen      (1000) chen      (1000)      399 2022-05-12 01:19:34.000000 django-webdav-ui-0.0.1/webdav/templates/webdav/share_auth.html
--rw-r--r--   0 chen      (1000) chen      (1000)      471 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.1/webdav/tests.py
--rw-r--r--   0 chen      (1000) chen      (1000)      206 2022-05-12 02:00:35.000000 django-webdav-ui-0.0.1/webdav/urls.py
--rw-r--r--   0 chen      (1000) chen      (1000)      161 2022-05-11 10:23:32.000000 django-webdav-ui-0.0.1/webdav/utils.py
--rw-r--r--   0 chen      (1000) chen      (1000)     1998 2022-05-12 02:00:11.000000 django-webdav-ui-0.0.1/webdav/views.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:32:43.969771 django-webdav-ui-0.0.2/
+-rw-r--r--   0 chen      (1000) chen      (1000)     1063 2022-05-11 08:29:55.000000 django-webdav-ui-0.0.2/LICENSE
+-rw-r--r--   0 chen      (1000) chen      (1000)      144 2023-04-14 07:09:15.000000 django-webdav-ui-0.0.2/MANIFEST.in
+-rw-r--r--   0 chen      (1000) chen      (1000)     2002 2023-04-14 07:32:43.969771 django-webdav-ui-0.0.2/PKG-INFO
+-rw-r--r--   0 chen      (1000) chen      (1000)     1135 2023-04-14 07:32:28.000000 django-webdav-ui-0.0.2/README.rst
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:32:43.959771 django-webdav-ui-0.0.2/django_webdav_ui.egg-info/
+-rw-r--r--   0 chen      (1000) chen      (1000)     2002 2023-04-14 07:32:43.000000 django-webdav-ui-0.0.2/django_webdav_ui.egg-info/PKG-INFO
+-rw-r--r--   0 chen      (1000) chen      (1000)     2161 2023-04-14 07:32:43.000000 django-webdav-ui-0.0.2/django_webdav_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)        1 2023-04-14 07:32:43.000000 django-webdav-ui-0.0.2/django_webdav_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       57 2023-04-14 07:32:43.000000 django-webdav-ui-0.0.2/django_webdav_ui.egg-info/requires.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)        7 2023-04-14 07:32:43.000000 django-webdav-ui-0.0.2/django_webdav_ui.egg-info/top_level.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)      108 2023-04-14 07:13:23.000000 django-webdav-ui-0.0.2/pyproject.toml
+-rw-r--r--   0 chen      (1000) chen      (1000)      928 2023-04-14 07:32:43.969771 django-webdav-ui-0.0.2/setup.cfg
+-rw-r--r--   0 chen      (1000) chen      (1000)       38 2023-04-14 07:09:55.000000 django-webdav-ui-0.0.2/setup.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:32:43.963105 django-webdav-ui-0.0.2/webdav/
+-rw-r--r--   0 chen      (1000) chen      (1000)     1038 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.2/webdav/__init__.py
+-rw-r--r--   0 chen      (1000) chen      (1000)      886 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.2/webdav/admin.py
+-rw-r--r--   0 chen      (1000) chen      (1000)     7242 2022-05-11 10:10:04.000000 django-webdav-ui-0.0.2/webdav/apis.py
+-rw-r--r--   0 chen      (1000) chen      (1000)      198 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.2/webdav/apps.py
+-rw-r--r--   0 chen      (1000) chen      (1000)    13625 2022-05-11 10:14:26.000000 django-webdav-ui-0.0.2/webdav/client.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:32:43.963105 django-webdav-ui-0.0.2/webdav/components/
+-rw-r--r--   0 chen      (1000) chen      (1000)       71 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/README.md
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:32:43.969771 django-webdav-ui-0.0.2/webdav/components/components/
+-rw-r--r--   0 chen      (1000) chen      (1000)      896 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/ActivityBox.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)      745 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/ActivityLine.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     1087 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/BatchButton.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     2291 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/CommentBox.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)      640 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/CommentLine.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)      653 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/CreateFolderButton.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     2467 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/CreateFolderDialog.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     1833 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/DavBody.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)      882 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/DirectoryBreadcrumbs.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)      618 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/DownloadMenu.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     1837 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/FileActions.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     1667 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/FileDeleteDialog.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)      778 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/FileDeleteMenu.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     2077 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/FileName.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     1800 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/FilePreview.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)      952 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/FileSummary.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     5064 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/FilesTable.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     2731 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/LeftPanel.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)      943 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/Preview.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     2677 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/RenameDialog.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)      890 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/RenameMenu.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     3058 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/ShareBox.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     1711 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/Sidebar.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)      429 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/components/Topbar.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     1480 2023-04-14 07:06:17.000000 django-webdav-ui-0.0.2/webdav/components/components/UploadButton.jsx
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:32:43.969771 django-webdav-ui-0.0.2/webdav/components/context/
+-rw-r--r--   0 chen      (1000) chen      (1000)      467 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/context/batch.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)      953 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/context/directory-context.jsx
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:32:43.969771 django-webdav-ui-0.0.2/webdav/components/utils/
+-rw-r--r--   0 chen      (1000) chen      (1000)     1295 2023-04-14 06:54:38.000000 django-webdav-ui-0.0.2/webdav/components/utils/utils.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)     1247 2023-04-14 06:58:30.000000 django-webdav-ui-0.0.2/webdav/components/webdav.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)      257 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.2/webdav/filters.py
+-rw-r--r--   0 chen      (1000) chen      (1000)      165 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.2/webdav/forms.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:32:43.969771 django-webdav-ui-0.0.2/webdav/migrations/
+-rw-r--r--   0 chen      (1000) chen      (1000)     2519 2022-05-11 08:36:39.000000 django-webdav-ui-0.0.2/webdav/migrations/0001_initial.py
+-rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.2/webdav/migrations/__init__.py
+-rw-r--r--   0 chen      (1000) chen      (1000)     1929 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.2/webdav/models.py
+-rw-r--r--   0 chen      (1000) chen      (1000)     1156 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.2/webdav/receivers.py
+-rw-r--r--   0 chen      (1000) chen      (1000)     2566 2022-05-11 10:25:23.000000 django-webdav-ui-0.0.2/webdav/serializers.py
+-rw-r--r--   0 chen      (1000) chen      (1000)      108 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.2/webdav/signals.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:32:43.956438 django-webdav-ui-0.0.2/webdav/static/
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:32:43.969771 django-webdav-ui-0.0.2/webdav/static/webdav/
+-rw-r--r--   0 chen      (1000) chen      (1000)   206620 2022-05-12 01:20:54.000000 django-webdav-ui-0.0.2/webdav/static/webdav/bulma.min.css
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:32:43.969771 django-webdav-ui-0.0.2/webdav/static/webdav/dist/
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:32:43.969771 django-webdav-ui-0.0.2/webdav/static/webdav/dist/assets/
+-rw-r--r--   0 chen      (1000) chen      (1000)   412754 2023-04-14 07:08:19.000000 django-webdav-ui-0.0.2/webdav/static/webdav/dist/assets/webdav-07e1678a.js
+-rw-r--r--   0 chen      (1000) chen      (1000)      133 2023-04-14 07:08:19.000000 django-webdav-ui-0.0.2/webdav/static/webdav/dist/manifest.json
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:32:43.956438 django-webdav-ui-0.0.2/webdav/templates/
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 07:32:43.969771 django-webdav-ui-0.0.2/webdav/templates/webdav/
+-rw-r--r--   0 chen      (1000) chen      (1000)     1253 2023-04-14 07:03:34.000000 django-webdav-ui-0.0.2/webdav/templates/webdav/base.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      301 2023-04-14 07:00:49.000000 django-webdav-ui-0.0.2/webdav/templates/webdav/index.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      436 2022-05-12 01:18:51.000000 django-webdav-ui-0.0.2/webdav/templates/webdav/share.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      399 2022-05-12 01:19:34.000000 django-webdav-ui-0.0.2/webdav/templates/webdav/share_auth.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      471 2022-05-11 08:26:16.000000 django-webdav-ui-0.0.2/webdav/tests.py
+-rw-r--r--   0 chen      (1000) chen      (1000)      206 2022-05-12 02:00:35.000000 django-webdav-ui-0.0.2/webdav/urls.py
+-rw-r--r--   0 chen      (1000) chen      (1000)      161 2022-05-11 10:23:32.000000 django-webdav-ui-0.0.2/webdav/utils.py
+-rw-r--r--   0 chen      (1000) chen      (1000)     1998 2022-05-12 02:00:11.000000 django-webdav-ui-0.0.2/webdav/views.py
```

### Comparing `django-webdav-ui-0.0.1/LICENSE` & `django-webdav-ui-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/PKG-INFO` & `django-webdav-ui-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webdav-ui
-Version: 0.0.1
+Version: 0.0.2
 Summary: A webdav client app for django.
 Home-page: https://github.com/ChanMo/django-webdav/
 Author: ChanMo
 Author-email: chan.mo@outlook.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -23,14 +23,19 @@
 License-File: LICENSE
 
 Django Webdav Client
 ====================
 
 File Manager like dropbox
 
+.. figure:: ./webdav.jpeg
+   :alt: Screenshot
+
+   Screenshot
+
 Features
 --------
 
 -  文件管理
 -  多级目录
 -  分片上传
 -  文件预览
@@ -52,15 +57,15 @@
 -----------
 
 Install
 ~~~~~~~
 
 .. code:: bash
 
-   pip install django-webdav
+   pip install django-webdav-ui
 
 Update Settings.py
 ~~~~~~~~~~~~~~~~~~
 
 .. code:: python
 
    INSTALLED_APPS = [
```

### Comparing `django-webdav-ui-0.0.1/README.rst` & `django-webdav-ui-0.0.2/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 Django Webdav Client
 ====================
 
 File Manager like dropbox
 
+.. figure:: ./webdav.jpeg
+   :alt: Screenshot
+
+   Screenshot
+
 Features
 --------
 
 -  文件管理
 -  多级目录
 -  分片上传
 -  文件预览
@@ -28,15 +33,15 @@
 -----------
 
 Install
 ~~~~~~~
 
 .. code:: bash
 
-   pip install django-webdav
+   pip install django-webdav-ui
 
 Update Settings.py
 ~~~~~~~~~~~~~~~~~~
 
 .. code:: python
 
    INSTALLED_APPS = [
```

### Comparing `django-webdav-ui-0.0.1/django_webdav_ui.egg-info/PKG-INFO` & `django-webdav-ui-0.0.2/django_webdav_ui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webdav-ui
-Version: 0.0.1
+Version: 0.0.2
 Summary: A webdav client app for django.
 Home-page: https://github.com/ChanMo/django-webdav/
 Author: ChanMo
 Author-email: chan.mo@outlook.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -23,14 +23,19 @@
 License-File: LICENSE
 
 Django Webdav Client
 ====================
 
 File Manager like dropbox
 
+.. figure:: ./webdav.jpeg
+   :alt: Screenshot
+
+   Screenshot
+
 Features
 --------
 
 -  文件管理
 -  多级目录
 -  分片上传
 -  文件预览
@@ -52,15 +57,15 @@
 -----------
 
 Install
 ~~~~~~~
 
 .. code:: bash
 
-   pip install django-webdav
+   pip install django-webdav-ui
 
 Update Settings.py
 ~~~~~~~~~~~~~~~~~~
 
 .. code:: python
 
    INSTALLED_APPS = [
```

### Comparing `django-webdav-ui-0.0.1/django_webdav_ui.egg-info/SOURCES.txt` & `django-webdav-ui-0.0.2/django_webdav_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/setup.cfg` & `django-webdav-ui-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-webdav-ui
-version = 0.0.1
+version = 0.0.2
 description = A webdav client app for django.
 long_description = file: README.rst
 url = https://github.com/ChanMo/django-webdav/
 author = ChanMo
 author_email = chan.mo@outlook.com
 license = MIT
 classifiers =
```

### Comparing `django-webdav-ui-0.0.1/webdav/__init__.py` & `django-webdav-ui-0.0.2/webdav/__init__.py`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/admin.py` & `django-webdav-ui-0.0.2/webdav/admin.py`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/apis.py` & `django-webdav-ui-0.0.2/webdav/apis.py`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/client.py` & `django-webdav-ui-0.0.2/webdav/client.py`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/ActivityBox.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/ActivityBox.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/ActivityLine.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/ActivityLine.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/BatchButton.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/BatchButton.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/CommentBox.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/CommentBox.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/CommentLine.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/CommentLine.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/CreateFolderButton.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/CreateFolderButton.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/CreateFolderDialog.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/CreateFolderDialog.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/DavBody.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/DavBody.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/DirectoryBreadcrumbs.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/DirectoryBreadcrumbs.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/DownloadMenu.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/DownloadMenu.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/FileActions.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/FileActions.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/FileDeleteDialog.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/FileDeleteDialog.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/FileDeleteMenu.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/FileDeleteMenu.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/FileName.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/FileName.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/FilePreview.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/FilePreview.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/FileSummary.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/FileSummary.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/FilesTable.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/FilesTable.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/LeftPanel.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/LeftPanel.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/Preview.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/Preview.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/RenameDialog.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/RenameDialog.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/RenameMenu.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/RenameMenu.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/ShareBox.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/ShareBox.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/Sidebar.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/Sidebar.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/components/UploadButton.jsx` & `django-webdav-ui-0.0.2/webdav/components/components/UploadButton.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/context/directory-context.jsx` & `django-webdav-ui-0.0.2/webdav/components/context/directory-context.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/utils/utils.jsx` & `django-webdav-ui-0.0.2/webdav/components/utils/utils.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/components/webdav.jsx` & `django-webdav-ui-0.0.2/webdav/components/webdav.jsx`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/migrations/0001_initial.py` & `django-webdav-ui-0.0.2/webdav/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/models.py` & `django-webdav-ui-0.0.2/webdav/models.py`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/receivers.py` & `django-webdav-ui-0.0.2/webdav/receivers.py`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/serializers.py` & `django-webdav-ui-0.0.2/webdav/serializers.py`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/static/webdav/bulma.min.css` & `django-webdav-ui-0.0.2/webdav/static/webdav/bulma.min.css`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/static/webdav/dist/assets/webdav-07e1678a.js` & `django-webdav-ui-0.0.2/webdav/static/webdav/dist/assets/webdav-07e1678a.js`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/templates/webdav/base.html` & `django-webdav-ui-0.0.2/webdav/templates/webdav/base.html`

 * *Files identical despite different names*

### Comparing `django-webdav-ui-0.0.1/webdav/views.py` & `django-webdav-ui-0.0.2/webdav/views.py`

 * *Files identical despite different names*

