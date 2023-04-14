# Comparing `tmp/groupdocs-annotation-cloud-22.2.tar.gz` & `tmp/groupdocs-annotation-cloud-23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\groupdocs-annotation-cloud-22.2.tar", last modified: Thu Feb  3 07:52:05 2022, max compression
+gzip compressed data, was "dist\groupdocs-annotation-cloud-23.4.tar", last modified: Fri Apr 14 05:55:50 2023, max compression
```

## Comparing `groupdocs-annotation-cloud-22.2.tar` & `groupdocs-annotation-cloud-23.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2022-02-03 07:52:05.000000 groupdocs-annotation-cloud-22.2/
--rw-rw-rw-   0        0        0     1105 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/LICENSE
--rw-rw-rw-   0        0        0     2943 2022-02-03 07:52:05.000000 groupdocs-annotation-cloud-22.2/PKG-INFO
--rw-rw-rw-   0        0        0     2053 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/README.md
-drwxrwxrwx   0        0        0        0 2022-02-03 07:52:05.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/
--rw-rw-rw-   0        0        0     3294 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/__init__.py
--rw-rw-rw-   0        0        0    26237 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/api_client.py
--rw-rw-rw-   0        0        0     2674 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/api_exception.py
-drwxrwxrwx   0        0        0        0 2022-02-03 07:52:05.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/
--rw-rw-rw-   0        0        0      539 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/__init__.py
--rw-rw-rw-   0        0        0    24794 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/annotate_api.py
--rw-rw-rw-   0        0        0    38663 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/file_api.py
--rw-rw-rw-   0        0        0    36273 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/folder_api.py
--rw-rw-rw-   0        0        0    11979 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/info_api.py
--rw-rw-rw-   0        0        0     6597 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/license_api.py
--rw-rw-rw-   0        0        0    14074 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/preview_api.py
--rw-rw-rw-   0        0        0    26585 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/storage_api.py
--rw-rw-rw-   0        0        0     3307 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/auth.py
--rw-rw-rw-   0        0        0     7681 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/configuration.py
-drwxrwxrwx   0        0        0        0 2022-02-03 07:52:05.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/
--rw-rw-rw-   0        0        0     2118 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/__init__.py
--rw-rw-rw-   0        0        0     9859 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/annotate_options.py
--rw-rw-rw-   0        0        0     3738 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/annotation_api_link.py
--rw-rw-rw-   0        0        0    30622 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/annotation_info.py
--rw-rw-rw-   0        0        0     9223 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/annotation_reply_info.py
--rw-rw-rw-   0        0        0     5129 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/consumption_result.py
--rw-rw-rw-   0        0        0     5187 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/disc_usage.py
--rw-rw-rw-   0        0        0     8742 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/document_info.py
--rw-rw-rw-   0        0        0     6291 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/error.py
--rw-rw-rw-   0        0        0     4905 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/error_details.py
--rw-rw-rw-   0        0        0     6354 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/file_info.py
--rw-rw-rw-   0        0        0     5413 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/file_version.py
--rw-rw-rw-   0        0        0     4151 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/file_versions.py
--rw-rw-rw-   0        0        0     4171 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/files_list.py
--rw-rw-rw-   0        0        0     4884 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     4900 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/format.py
--rw-rw-rw-   0        0        0     4208 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/formats_result.py
--rw-rw-rw-   0        0        0     7511 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/link.py
--rw-rw-rw-   0        0        0     4110 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/link_element.py
--rw-rw-rw-   0        0        0     5178 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/object_exist.py
--rw-rw-rw-   0        0        0     4507 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/page_image.py
--rw-rw-rw-   0        0        0     5212 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/page_images.py
--rw-rw-rw-   0        0        0     5829 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/page_info.py
--rw-rw-rw-   0        0        0     4851 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/point.py
--rw-rw-rw-   0        0        0    12352 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/preview_options.py
--rw-rw-rw-   0        0        0     6633 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/rectangle.py
--rw-rw-rw-   0        0        0     5937 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/remove_options.py
--rw-rw-rw-   0        0        0     4276 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     7173 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/storage_file.py
--rw-rw-rw-   0        0        0    13739 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/rest.py
-drwxrwxrwx   0        0        0        0 2022-02-03 07:52:05.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud.egg-info/
--rw-rw-rw-   0        0        0     2943 2022-02-03 07:52:04.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2771 2022-02-03 07:52:04.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-03 07:52:04.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2022-02-03 07:52:04.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2022-02-03 07:52:04.000000 groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-02-03 07:52:05.000000 groupdocs-annotation-cloud-22.2/setup.cfg
--rw-rw-rw-   0        0        0     1670 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-02-03 07:52:05.000000 groupdocs-annotation-cloud-22.2/test/
--rw-rw-rw-   0        0        0        0 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/__init__.py
-drwxrwxrwx   0        0        0        0 2022-02-03 07:52:05.000000 groupdocs-annotation-cloud-22.2/test/annotate/
--rw-rw-rw-   0        0        0        0 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/annotate/__init__.py
--rw-rw-rw-   0        0        0     4775 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/annotate/test_annotate_api.py
--rw-rw-rw-   0        0        0     4603 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/annotate/test_annotate_api_many_pages.py
-drwxrwxrwx   0        0        0        0 2022-02-03 07:52:05.000000 groupdocs-annotation-cloud-22.2/test/info/
--rw-rw-rw-   0        0        0        0 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/info/__init__.py
--rw-rw-rw-   0        0        0     2837 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/info/test_info_api.py
-drwxrwxrwx   0        0        0        0 2022-02-03 07:52:05.000000 groupdocs-annotation-cloud-22.2/test/preview/
--rw-rw-rw-   0        0        0        0 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/preview/__init__.py
--rw-rw-rw-   0        0        0     2413 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/preview/test_preview_api.py
-drwxrwxrwx   0        0        0        0 2022-02-03 07:52:05.000000 groupdocs-annotation-cloud-22.2/test/storage/
--rw-rw-rw-   0        0        0        0 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/storage/__init__.py
--rw-rw-rw-   0        0        0     3009 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/storage/test_auth_api.py
--rw-rw-rw-   0        0        0     3793 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/storage/test_file_api.py
--rw-rw-rw-   0        0        0     3139 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/storage/test_folder_api.py
--rw-rw-rw-   0        0        0     2733 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/storage/test_storage_api.py
--rw-rw-rw-   0        0        0     4937 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/test_context.py
--rw-rw-rw-   0        0        0     8066 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/test_file.py
--rw-rw-rw-   0        0        0     1702 2022-02-03 07:13:36.000000 groupdocs-annotation-cloud-22.2/test/test_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:55:50.000000 groupdocs-annotation-cloud-23.4/
+-rw-rw-rw-   0        0        0     1105 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/LICENSE
+-rw-rw-rw-   0        0        0     2902 2023-04-14 05:55:50.000000 groupdocs-annotation-cloud-23.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2053 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 05:55:50.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/
+-rw-rw-rw-   0        0        0     3294 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/__init__.py
+-rw-rw-rw-   0        0        0    26237 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/api_client.py
+-rw-rw-rw-   0        0        0     2674 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/api_exception.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:55:50.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/
+-rw-rw-rw-   0        0        0      539 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/__init__.py
+-rw-rw-rw-   0        0        0    24794 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/annotate_api.py
+-rw-rw-rw-   0        0        0    38663 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/file_api.py
+-rw-rw-rw-   0        0        0    36273 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/folder_api.py
+-rw-rw-rw-   0        0        0    11979 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/info_api.py
+-rw-rw-rw-   0        0        0     6597 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/license_api.py
+-rw-rw-rw-   0        0        0    14074 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/preview_api.py
+-rw-rw-rw-   0        0        0    26585 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/storage_api.py
+-rw-rw-rw-   0        0        0     3307 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/auth.py
+-rw-rw-rw-   0        0        0     7681 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/configuration.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:55:50.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/
+-rw-rw-rw-   0        0        0     2118 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/__init__.py
+-rw-rw-rw-   0        0        0     9859 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/annotate_options.py
+-rw-rw-rw-   0        0        0     3738 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/annotation_api_link.py
+-rw-rw-rw-   0        0        0    30622 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/annotation_info.py
+-rw-rw-rw-   0        0        0     9223 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/annotation_reply_info.py
+-rw-rw-rw-   0        0        0     5129 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/consumption_result.py
+-rw-rw-rw-   0        0        0     5187 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0     8742 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/document_info.py
+-rw-rw-rw-   0        0        0     6291 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/error.py
+-rw-rw-rw-   0        0        0     4905 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/error_details.py
+-rw-rw-rw-   0        0        0     6354 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/file_info.py
+-rw-rw-rw-   0        0        0     5413 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/file_version.py
+-rw-rw-rw-   0        0        0     4151 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     4171 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/files_list.py
+-rw-rw-rw-   0        0        0     4884 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     4900 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/format.py
+-rw-rw-rw-   0        0        0     4208 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/formats_result.py
+-rw-rw-rw-   0        0        0     7511 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/link.py
+-rw-rw-rw-   0        0        0     4110 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/link_element.py
+-rw-rw-rw-   0        0        0     5178 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/object_exist.py
+-rw-rw-rw-   0        0        0     4507 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/page_image.py
+-rw-rw-rw-   0        0        0     5212 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/page_images.py
+-rw-rw-rw-   0        0        0     5829 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/page_info.py
+-rw-rw-rw-   0        0        0     4851 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/point.py
+-rw-rw-rw-   0        0        0    12352 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/preview_options.py
+-rw-rw-rw-   0        0        0     6633 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/rectangle.py
+-rw-rw-rw-   0        0        0     5937 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/remove_options.py
+-rw-rw-rw-   0        0        0     4276 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     7173 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/storage_file.py
+-rw-rw-rw-   0        0        0    13739 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/rest.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:55:50.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud.egg-info/
+-rw-rw-rw-   0        0        0     2902 2023-04-14 05:55:49.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2771 2023-04-14 05:55:49.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 05:55:49.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-14 05:55:49.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-14 05:55:49.000000 groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 05:55:50.000000 groupdocs-annotation-cloud-23.4/setup.cfg
+-rw-rw-rw-   0        0        0     1670 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:55:50.000000 groupdocs-annotation-cloud-23.4/test/
+-rw-rw-rw-   0        0        0        0 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:55:50.000000 groupdocs-annotation-cloud-23.4/test/annotate/
+-rw-rw-rw-   0        0        0        0 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/annotate/__init__.py
+-rw-rw-rw-   0        0        0     4775 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/annotate/test_annotate_api.py
+-rw-rw-rw-   0        0        0     4603 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/annotate/test_annotate_api_many_pages.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:55:50.000000 groupdocs-annotation-cloud-23.4/test/info/
+-rw-rw-rw-   0        0        0        0 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/info/__init__.py
+-rw-rw-rw-   0        0        0     2837 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/info/test_info_api.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:55:50.000000 groupdocs-annotation-cloud-23.4/test/preview/
+-rw-rw-rw-   0        0        0        0 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/preview/__init__.py
+-rw-rw-rw-   0        0        0     2413 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/preview/test_preview_api.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:55:50.000000 groupdocs-annotation-cloud-23.4/test/storage/
+-rw-rw-rw-   0        0        0        0 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/storage/__init__.py
+-rw-rw-rw-   0        0        0     3009 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/storage/test_auth_api.py
+-rw-rw-rw-   0        0        0     3793 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/storage/test_file_api.py
+-rw-rw-rw-   0        0        0     3139 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/storage/test_folder_api.py
+-rw-rw-rw-   0        0        0     2733 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/storage/test_storage_api.py
+-rw-rw-rw-   0        0        0     4937 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/test_context.py
+-rw-rw-rw-   0        0        0     8066 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/test_file.py
+-rw-rw-rw-   0        0        0     1702 2023-04-14 05:55:28.000000 groupdocs-annotation-cloud-23.4/test/test_settings.py
```

### Comparing `groupdocs-annotation-cloud-22.2/LICENSE` & `groupdocs-annotation-cloud-23.4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2003-2021 Aspose Pty Ltd
+Copyright (c) 2003-2023 Aspose Pty Ltd
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `groupdocs-annotation-cloud-22.2/PKG-INFO` & `groupdocs-annotation-cloud-23.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: groupdocs-annotation-cloud
-Version: 22.2
+Version: 23.4
 Summary: GroupDocs.Annotation Cloud Python SDK
 Home-page: http://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
-License: UNKNOWN
 Keywords: groupdocs,annotation,cloud,python,sdk
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -80,9 +78,7 @@
 +[**Documentation**](https://docs.groupdocs.cloud/annotation/)
 +[**Free Support Forum**](https://forum.groupdocs.cloud/c/annotation)
 +[**Blog**](https://blog.groupdocs.cloud/category/annotation)
 
 ## Contact Us
 
 Your feedback is very important to us. Please feel free to contact us using our [Support Forums](https://forum.groupdocs.cloud/c/annotation).
-
-
```

### Comparing `groupdocs-annotation-cloud-22.2/README.md` & `groupdocs-annotation-cloud-23.4/README.md`

 * *Files identical despite different names*

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/__init__.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/api_client.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="api_client.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -70,20 +70,20 @@
     }
 
     def __init__(self, configuration, header_name=None, header_value=None,
                  cookie=None):
         self.configuration = configuration
         self.pool = None
         self.rest_client = rest.RESTClientObject(configuration)
-        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '22.2'}
+        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '23.4'}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'python sdk 22.2'
+        self.user_agent = 'python sdk 23.4'
 
     def __del__(self):
         if self.pool is not None:
             self.pool.close()
             self.pool.join()
 
     @property
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/api_exception.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/api_exception.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="api_exception.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/__init__.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/annotate_api.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/annotate_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -453,15 +453,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="annotate_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -489,15 +489,15 @@
     def __init__(self, options):
         """Initializes new instance of AnnotateRequest."""  # noqa: E501
         self.options = options
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="annotate_direct_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -525,15 +525,15 @@
     def __init__(self, options):
         """Initializes new instance of AnnotateDirectRequest."""  # noqa: E501
         self.options = options
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="extract_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -561,15 +561,15 @@
     def __init__(self, file_info):
         """Initializes new instance of ExtractRequest."""  # noqa: E501
         self.file_info = file_info
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="remove_annotations_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/file_api.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/file_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -634,15 +634,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="copy_file_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -678,15 +678,15 @@
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="delete_file_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -718,15 +718,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="download_file_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -758,15 +758,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="move_file_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -802,15 +802,15 @@
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="upload_file_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/folder_api.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/folder_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -610,15 +610,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="copy_folder_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -652,15 +652,15 @@
         self.dest_path = dest_path
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="create_folder_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -690,15 +690,15 @@
         """Initializes new instance of CreateFolderRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="delete_folder_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -730,15 +730,15 @@
         self.path = path
         self.storage_name = storage_name
         self.recursive = recursive
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_files_list_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -768,15 +768,15 @@
         """Initializes new instance of GetFilesListRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="move_folder_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/info_api.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/info_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -265,15 +265,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_info_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/license_api.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/license_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/preview_api.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/preview_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -271,15 +271,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="delete_pages_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -307,15 +307,15 @@
     def __init__(self, file_info):
         """Initializes new instance of DeletePagesRequest."""  # noqa: E501
         self.file_info = file_info
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_pages_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/apis/storage_api.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/apis/storage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -471,15 +471,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_disc_usage_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -507,15 +507,15 @@
     def __init__(self, storage_name=None):
         """Initializes new instance of GetDiscUsageRequest."""  # noqa: E501
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_file_versions_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -545,15 +545,15 @@
         """Initializes new instance of GetFileVersionsRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="object_exists_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -585,15 +585,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="storage_exists_request.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/auth.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="auth.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/configuration.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="configuration.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -198,10 +198,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 22.2\n"\
-               "SDK Package Version: 22.2".\
+               "Version of the API: 23.4\n"\
+               "SDK Package Version: 23.4".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/__init__.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/annotate_options.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/annotate_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="AnnotateOptions.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/annotation_api_link.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/annotation_api_link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="AnnotationApiLink.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/annotation_info.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/annotation_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="AnnotationInfo.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/annotation_reply_info.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/annotation_reply_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="AnnotationReplyInfo.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/consumption_result.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/consumption_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ConsumptionResult.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/disc_usage.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/disc_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DiscUsage.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/document_info.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/document_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DocumentInfo.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/error.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Error.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/error_details.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/error_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ErrorDetails.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/file_info.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/file_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileInfo.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/file_version.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/file_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileVersion.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/file_versions.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/file_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileVersions.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/files_list.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/files_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FilesList.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/files_upload_result.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/files_upload_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FilesUploadResult.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/format.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Format.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/formats_result.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/formats_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FormatsResult.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/link.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Link.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/link_element.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/link_element.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="LinkElement.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/object_exist.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/object_exist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ObjectExist.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/page_image.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/page_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PageImage.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/page_images.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/page_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PageImages.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/page_info.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/page_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PageInfo.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/point.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Point.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/preview_options.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/preview_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PreviewOptions.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/rectangle.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/rectangle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Rectangle.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/remove_options.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/remove_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="RemoveOptions.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/storage_exist.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/storage_exist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="StorageExist.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/models/storage_file.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/models/storage_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="StorageFile.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud/rest.py` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="rest.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud.egg-info/PKG-INFO` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: groupdocs-annotation-cloud
-Version: 22.2
+Version: 23.4
 Summary: GroupDocs.Annotation Cloud Python SDK
 Home-page: http://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
-License: UNKNOWN
 Keywords: groupdocs,annotation,cloud,python,sdk
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -80,9 +78,7 @@
 +[**Documentation**](https://docs.groupdocs.cloud/annotation/)
 +[**Free Support Forum**](https://forum.groupdocs.cloud/c/annotation)
 +[**Blog**](https://blog.groupdocs.cloud/category/annotation)
 
 ## Contact Us
 
 Your feedback is very important to us. Please feel free to contact us using our [Support Forums](https://forum.groupdocs.cloud/c/annotation).
-
-
```

### Comparing `groupdocs-annotation-cloud-22.2/groupdocs_annotation_cloud.egg-info/SOURCES.txt` & `groupdocs-annotation-cloud-23.4/groupdocs_annotation_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `groupdocs-annotation-cloud-22.2/setup.py` & `groupdocs-annotation-cloud-23.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 import datetime
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "groupdocs-annotation-cloud"
-VERSION = "22.2"
+VERSION = "23.4"
 
 # Append current time to the version when publishing to test environment
 if "--test" in sys.argv:
     VERSION += "." + datetime.datetime.now().strftime("%Y%m%d%H%M")
     sys.argv.remove("--test")
 
 # To install the library, run the following
```

### Comparing `groupdocs-annotation-cloud-22.2/test/annotate/test_annotate_api.py` & `groupdocs-annotation-cloud-23.4/test/annotate/test_annotate_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/test/annotate/test_annotate_api_many_pages.py` & `groupdocs-annotation-cloud-23.4/test/annotate/test_annotate_api_many_pages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/test/info/test_info_api.py` & `groupdocs-annotation-cloud-23.4/test/info/test_info_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/test/preview/test_preview_api.py` & `groupdocs-annotation-cloud-23.4/test/preview/test_preview_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/test/storage/test_auth_api.py` & `groupdocs-annotation-cloud-23.4/test/storage/test_auth_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_auth_api.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/test/storage/test_file_api.py` & `groupdocs-annotation-cloud-23.4/test/storage/test_file_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/test/storage/test_folder_api.py` & `groupdocs-annotation-cloud-23.4/test/storage/test_folder_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/test/storage/test_storage_api.py` & `groupdocs-annotation-cloud-23.4/test/storage/test_storage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/test/test_context.py` & `groupdocs-annotation-cloud-23.4/test/test_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_context.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/test/test_file.py` & `groupdocs-annotation-cloud-23.4/test/test_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_file.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-annotation-cloud-22.2/test/test_settings.py` & `groupdocs-annotation-cloud-23.4/test/test_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_context.py">
-#   Copyright (c) 2003-2021 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

