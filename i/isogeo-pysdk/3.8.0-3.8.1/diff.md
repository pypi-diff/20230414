# Comparing `tmp/isogeo-pysdk-3.8.0.tar.gz` & `tmp/isogeo-pysdk-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\isogeo-pysdk-3.8.0.tar", last modified: Mon Dec  5 16:24:05 2022, max compression
+gzip compressed data, was "isogeo-pysdk-3.8.1.tar", last modified: Fri Apr 14 15:35:04 2023, max compression
```

## Comparing `isogeo-pysdk-3.8.0.tar` & `isogeo-pysdk-3.8.1.tar`

### file list

```diff
@@ -1,121 +1,159 @@
-drwxrwxrwx   0        0        0        0 2022-12-05 16:24:05.000000 isogeo-pysdk-3.8.0/
--rw-rw-rw-   0        0        0     7817 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/LICENSE
--rw-rw-rw-   0        0        0     4149 2022-12-05 16:24:05.000000 isogeo-pysdk-3.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2878 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/README.md
-drwxrwxrwx   0        0        0        0 2022-12-05 16:24:04.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/
--rw-rw-rw-   0        0        0      714 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/__about__.py
--rw-rw-rw-   0        0        0      738 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-05 16:24:05.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/
--rw-rw-rw-   0        0        0     1508 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/__init__.py
--rw-rw-rw-   0        0        0     5991 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_about.py
--rw-rw-rw-   0        0        0     5945 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_account.py
--rw-rw-rw-   0        0        0    19343 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_application.py
--rw-rw-rw-   0        0        0    22863 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_catalog.py
--rw-rw-rw-   0        0        0     8245 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_condition.py
--rw-rw-rw-   0        0        0     7558 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_conformity.py
--rw-rw-rw-   0        0        0    16653 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_contact.py
--rw-rw-rw-   0        0        0    14009 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_coordinate_systems.py
--rw-rw-rw-   0        0        0    13598 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_datasource.py
--rw-rw-rw-   0        0        0     2819 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_directives.py
--rw-rw-rw-   0        0        0    10559 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_event.py
--rw-rw-rw-   0        0        0    18810 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_feature_attributes.py
--rw-rw-rw-   0        0        0    12852 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_format.py
--rw-rw-rw-   0        0        0    10496 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_invitation.py
--rw-rw-rw-   0        0        0    38302 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_keyword.py
--rw-rw-rw-   0        0        0    15256 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_license.py
--rw-rw-rw-   0        0        0    11164 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_limitation.py
--rw-rw-rw-   0        0        0    25144 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_link.py
--rw-rw-rw-   0        0        0    15535 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_metadata.py
--rw-rw-rw-   0        0        0     6058 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_metadata_bulk.py
--rw-rw-rw-   0        0        0    17200 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_search.py
--rw-rw-rw-   0        0        0    16317 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_service.py
--rw-rw-rw-   0        0        0    17056 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_service_layers.py
--rw-rw-rw-   0        0        0    18310 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_service_operations.py
--rw-rw-rw-   0        0        0    23781 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_share.py
--rw-rw-rw-   0        0        0    14650 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_specification.py
--rw-rw-rw-   0        0        0     4307 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_thesaurus.py
--rw-rw-rw-   0        0        0    12937 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_user.py
--rw-rw-rw-   0        0        0    18202 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_workgroup.py
--rw-rw-rw-   0        0        0     1605 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/api_hooks.py
--rw-rw-rw-   0        0        0    18711 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/checker.py
--rw-rw-rw-   0        0        0     2255 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/decorators.py
-drwxrwxrwx   0        0        0        0 2022-12-05 16:24:05.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/
--rw-rw-rw-   0        0        0     1358 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/__init__.py
--rw-rw-rw-   0        0        0     2106 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/application_types.py
--rw-rw-rw-   0        0        0     2130 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/bulk_actions.py
--rw-rw-rw-   0        0        0     2315 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/bulk_ignore_reasons.py
--rw-rw-rw-   0        0        0     2422 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/bulk_targets.py
--rw-rw-rw-   0        0        0     2861 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/catalog_statistics_tags.py
--rw-rw-rw-   0        0        0     2349 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/contact_roles.py
--rw-rw-rw-   0        0        0     2082 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/contact_types.py
--rw-rw-rw-   0        0        0     2066 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/edition_profiles.py
--rw-rw-rw-   0        0        0     2144 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/event_kinds.py
--rw-rw-rw-   0        0        0     2204 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/keyword_casing.py
--rw-rw-rw-   0        0        0     2591 2022-12-05 16:22:25.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/limitation_restrictions.py
--rw-rw-rw-   0        0        0     2067 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/limitation_types.py
--rw-rw-rw-   0        0        0     2058 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/link_actions.py
--rw-rw-rw-   0        0        0     2470 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/link_kinds.py
--rw-rw-rw-   0        0        0     2026 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/link_types.py
--rw-rw-rw-   0        0        0     2819 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/metadata_subresources.py
--rw-rw-rw-   0        0        0     2518 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/metadata_types.py
--rw-rw-rw-   0        0        0     2466 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/search_filters_georelations.py
--rw-rw-rw-   0        0        0     2215 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/session_status.py
--rw-rw-rw-   0        0        0     2125 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/share_types.py
--rw-rw-rw-   0        0        0     1998 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/user_roles.py
--rw-rw-rw-   0        0        0     3054 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/enums/workgroup_statistics_tags.py
--rw-rw-rw-   0        0        0     1001 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/exceptions.py
--rw-rw-rw-   0        0        0    19870 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/isogeo.py
-drwxrwxrwx   0        0        0        0 2022-12-05 16:24:05.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/
--rw-rw-rw-   0        0        0     1748 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/__init__.py
--rw-rw-rw-   0        0        0    16184 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/application.py
--rw-rw-rw-   0        0        0     4260 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/bulk_report.py
--rw-rw-rw-   0        0        0     6262 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/bulk_request.py
--rw-rw-rw-   0        0        0    10991 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/catalog.py
--rw-rw-rw-   0        0        0     7922 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/condition.py
--rw-rw-rw-   0        0        0     7812 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/conformity.py
--rw-rw-rw-   0        0        0    15867 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/contact.py
--rw-rw-rw-   0        0        0     6213 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/coordinates_system.py
--rw-rw-rw-   0        0        0    10550 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/datasource.py
--rw-rw-rw-   0        0        0     4238 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/directive.py
--rw-rw-rw-   0        0        0     7486 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/event.py
--rw-rw-rw-   0        0        0    17324 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/feature_attributes.py
--rw-rw-rw-   0        0        0     8175 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/format.py
--rw-rw-rw-   0        0        0     9348 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/invitation.py
--rw-rw-rw-   0        0        0     9533 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/keyword.py
--rw-rw-rw-   0        0        0     5635 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/keyword_search.py
--rw-rw-rw-   0        0        0     9004 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/license.py
--rw-rw-rw-   0        0        0     9250 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/limitation.py
--rw-rw-rw-   0        0        0    10510 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/link.py
--rw-rw-rw-   0        0        0    43405 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/metadata.py
--rw-rw-rw-   0        0        0     7856 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/metadata_search.py
--rw-rw-rw-   0        0        0     9701 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/service_layer.py
--rw-rw-rw-   0        0        0     8952 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/service_operation.py
--rw-rw-rw-   0        0        0    15186 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/share.py
--rw-rw-rw-   0        0        0    10004 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/specification.py
--rw-rw-rw-   0        0        0     6780 2022-12-05 16:22:25.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/thesaurus.py
--rw-rw-rw-   0        0        0    11239 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/user.py
--rw-rw-rw-   0        0        0    18470 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/models/workgroup.py
-drwxrwxrwx   0        0        0        0 2022-12-05 16:24:05.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/samples/
--rw-rw-rw-   0        0        0        0 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/samples/__init__.py
--rw-rw-rw-   0        0        0     4258 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/samples/attributes_frequency.py
--rw-rw-rw-   0        0        0     2563 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/samples/download_batch_hosted_data.py
--rw-rw-rw-   0        0        0     2623 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/samples/export_batch_xml19139_sync.py
--rw-rw-rw-   0        0        0     2830 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/samples/get_OpenCatalog.py
--rw-rw-rw-   0        0        0     2293 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/samples/latest_md_modified.py
--rw-rw-rw-   0        0        0     6737 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/samples/related_links.py
--rw-rw-rw-   0        0        0     5378 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/samples/results_parser.py
--rw-rw-rw-   0        0        0     2741 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/samples/search.py
--rw-rw-rw-   0        0        0     3554 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/samples/spatial_search.py
--rw-rw-rw-   0        0        0     6106 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/samples/store_api_responses_read.py
--rw-rw-rw-   0        0        0     7670 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/samples/store_api_responses_rw.py
--rw-rw-rw-   0        0        0     7790 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/translator.py
--rw-rw-rw-   0        0        0      838 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/type_hints_custom.py
--rw-rw-rw-   0        0        0    40710 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/isogeo_pysdk/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-05 16:24:04.000000 isogeo-pysdk-3.8.0/isogeo_pysdk.egg-info/
--rw-rw-rw-   0        0        0     4149 2022-12-05 16:24:04.000000 isogeo-pysdk-3.8.0/isogeo_pysdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3952 2022-12-05 16:24:04.000000 isogeo-pysdk-3.8.0/isogeo_pysdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-05 16:24:04.000000 isogeo-pysdk-3.8.0/isogeo_pysdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2022-12-05 16:24:04.000000 isogeo-pysdk-3.8.0/isogeo_pysdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-12-05 16:24:04.000000 isogeo-pysdk-3.8.0/isogeo_pysdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      965 2022-12-05 16:24:05.000000 isogeo-pysdk-3.8.0/setup.cfg
--rw-rw-rw-   0        0        0     2378 2022-12-05 16:22:24.000000 isogeo-pysdk-3.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.140217 isogeo-pysdk-3.8.1/
+-rw-rw-rw-   0        0        0     7817 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/LICENSE
+-rw-rw-rw-   0        0        0     4149 2023-04-14 15:35:04.140217 isogeo-pysdk-3.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2878 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.062095 isogeo-pysdk-3.8.1/isogeo_pysdk/
+-rw-rw-rw-   0        0        0      714 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/__about__.py
+-rw-rw-rw-   0        0        0      738 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.077716 isogeo-pysdk-3.8.1/isogeo_pysdk/api/
+-rw-rw-rw-   0        0        0     1508 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/__init__.py
+-rw-rw-rw-   0        0        0     5991 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_about.py
+-rw-rw-rw-   0        0        0     5945 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_account.py
+-rw-rw-rw-   0        0        0    19343 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_application.py
+-rw-rw-rw-   0        0        0    22863 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_catalog.py
+-rw-rw-rw-   0        0        0     8245 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_condition.py
+-rw-rw-rw-   0        0        0     7558 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_conformity.py
+-rw-rw-rw-   0        0        0    16653 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_contact.py
+-rw-rw-rw-   0        0        0    14009 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_coordinate_systems.py
+-rw-rw-rw-   0        0        0    13598 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_datasource.py
+-rw-rw-rw-   0        0        0     2819 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_directives.py
+-rw-rw-rw-   0        0        0    10559 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_event.py
+-rw-rw-rw-   0        0        0    19108 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_feature_attributes.py
+-rw-rw-rw-   0        0        0    12852 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_format.py
+-rw-rw-rw-   0        0        0    10496 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_invitation.py
+-rw-rw-rw-   0        0        0    38458 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_keyword.py
+-rw-rw-rw-   0        0        0    15256 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_license.py
+-rw-rw-rw-   0        0        0    11164 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_limitation.py
+-rw-rw-rw-   0        0        0    25144 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_link.py
+-rw-rw-rw-   0        0        0    15535 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_metadata.py
+-rw-rw-rw-   0        0        0     6058 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_metadata_bulk.py
+-rw-rw-rw-   0        0        0    17200 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_search.py
+-rw-rw-rw-   0        0        0    16317 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_service.py
+-rw-rw-rw-   0        0        0    17176 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_service_layers.py
+-rw-rw-rw-   0        0        0    18310 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_service_operations.py
+-rw-rw-rw-   0        0        0    23781 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_share.py
+-rw-rw-rw-   0        0        0    14650 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_specification.py
+-rw-rw-rw-   0        0        0     4307 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_thesaurus.py
+-rw-rw-rw-   0        0        0    12937 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_user.py
+-rw-rw-rw-   0        0        0    18202 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_workgroup.py
+-rw-rw-rw-   0        0        0     1605 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/api_hooks.py
+-rw-rw-rw-   0        0        0    18711 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/checker.py
+-rw-rw-rw-   0        0        0     2255 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/decorators.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.093344 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/
+-rw-rw-rw-   0        0        0     1424 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/__init__.py
+-rw-rw-rw-   0        0        0     2106 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/application_types.py
+-rw-rw-rw-   0        0        0     2130 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/bulk_actions.py
+-rw-rw-rw-   0        0        0     2315 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/bulk_ignore_reasons.py
+-rw-rw-rw-   0        0        0     2422 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/bulk_targets.py
+-rw-rw-rw-   0        0        0     2861 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/catalog_statistics_tags.py
+-rw-rw-rw-   0        0        0     2349 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/contact_roles.py
+-rw-rw-rw-   0        0        0     2082 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/contact_types.py
+-rw-rw-rw-   0        0        0     2066 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/edition_profiles.py
+-rw-rw-rw-   0        0        0     2144 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/event_kinds.py
+-rw-rw-rw-   0        0        0     2204 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/keyword_casing.py
+-rw-rw-rw-   0        0        0     2591 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/limitation_restrictions.py
+-rw-rw-rw-   0        0        0     2067 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/limitation_types.py
+-rw-rw-rw-   0        0        0     2058 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/link_actions.py
+-rw-rw-rw-   0        0        0     2470 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/link_kinds.py
+-rw-rw-rw-   0        0        0     2026 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/link_types.py
+-rw-rw-rw-   0        0        0     2819 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/metadata_subresources.py
+-rw-rw-rw-   0        0        0     2518 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/metadata_types.py
+-rw-rw-rw-   0        0        0     2466 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/search_filters_georelations.py
+-rw-rw-rw-   0        0        0     2128 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/service_layer_types.py
+-rw-rw-rw-   0        0        0     2215 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/session_status.py
+-rw-rw-rw-   0        0        0     2125 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/share_types.py
+-rw-rw-rw-   0        0        0     1998 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/user_roles.py
+-rw-rw-rw-   0        0        0     3054 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/enums/workgroup_statistics_tags.py
+-rw-rw-rw-   0        0        0     1001 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/exceptions.py
+-rw-rw-rw-   0        0        0    19870 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/isogeo.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.108965 isogeo-pysdk-3.8.1/isogeo_pysdk/models/
+-rw-rw-rw-   0        0        0     1748 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/__init__.py
+-rw-rw-rw-   0        0        0    16184 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/application.py
+-rw-rw-rw-   0        0        0     4260 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/bulk_report.py
+-rw-rw-rw-   0        0        0     6262 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/bulk_request.py
+-rw-rw-rw-   0        0        0    10991 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/catalog.py
+-rw-rw-rw-   0        0        0     7922 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/condition.py
+-rw-rw-rw-   0        0        0     7812 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/conformity.py
+-rw-rw-rw-   0        0        0    15867 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/contact.py
+-rw-rw-rw-   0        0        0     6213 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/coordinates_system.py
+-rw-rw-rw-   0        0        0    10550 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/datasource.py
+-rw-rw-rw-   0        0        0     4238 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/directive.py
+-rw-rw-rw-   0        0        0     7486 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/event.py
+-rw-rw-rw-   0        0        0    17324 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/feature_attributes.py
+-rw-rw-rw-   0        0        0     8175 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/format.py
+-rw-rw-rw-   0        0        0     9348 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/invitation.py
+-rw-rw-rw-   0        0        0     9533 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/keyword.py
+-rw-rw-rw-   0        0        0     5635 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/keyword_search.py
+-rw-rw-rw-   0        0        0     9004 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/license.py
+-rw-rw-rw-   0        0        0     9250 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/limitation.py
+-rw-rw-rw-   0        0        0    10510 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/link.py
+-rw-rw-rw-   0        0        0    43405 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/metadata.py
+-rw-rw-rw-   0        0        0     7856 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/metadata_search.py
+-rw-rw-rw-   0        0        0    12874 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/service_layer.py
+-rw-rw-rw-   0        0        0     8952 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/service_operation.py
+-rw-rw-rw-   0        0        0    15186 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/share.py
+-rw-rw-rw-   0        0        0    10004 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/specification.py
+-rw-rw-rw-   0        0        0     6780 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/thesaurus.py
+-rw-rw-rw-   0        0        0    11239 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/user.py
+-rw-rw-rw-   0        0        0    18470 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/models/workgroup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.124592 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/
+-rw-rw-rw-   0        0        0        0 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/__init__.py
+-rw-rw-rw-   0        0        0     4258 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/attributes_frequency.py
+-rw-rw-rw-   0        0        0     2563 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/download_batch_hosted_data.py
+-rw-rw-rw-   0        0        0     2623 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/export_batch_xml19139_sync.py
+-rw-rw-rw-   0        0        0     2830 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/get_OpenCatalog.py
+-rw-rw-rw-   0        0        0     2293 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/latest_md_modified.py
+-rw-rw-rw-   0        0        0     6737 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/related_links.py
+-rw-rw-rw-   0        0        0     5378 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/results_parser.py
+-rw-rw-rw-   0        0        0     2741 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/search.py
+-rw-rw-rw-   0        0        0     3554 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/spatial_search.py
+-rw-rw-rw-   0        0        0     6106 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/store_api_responses_read.py
+-rw-rw-rw-   0        0        0     7670 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/samples/store_api_responses_rw.py
+-rw-rw-rw-   0        0        0     7790 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/translator.py
+-rw-rw-rw-   0        0        0      838 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/type_hints_custom.py
+-rw-rw-rw-   0        0        0    40710 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/isogeo_pysdk/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.062095 isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/
+-rw-rw-rw-   0        0        0     4149 2023-04-14 15:35:03.000000 isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4886 2023-04-14 15:35:04.000000 isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 15:35:03.000000 isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-04-14 15:35:03.000000 isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-14 15:35:03.000000 isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      965 2023-04-14 15:35:04.140217 isogeo-pysdk-3.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     2378 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:35:04.140217 isogeo-pysdk-3.8.1/tests/
+-rw-rw-rw-   0        0        0     3224 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_about.py
+-rw-rw-rw-   0        0        0     4808 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_account.py
+-rw-rw-rw-   0        0        0    14716 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_applications.py
+-rw-rw-rw-   0        0        0     6528 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_authentication.py
+-rw-rw-rw-   0        0        0     7000 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_bulks.py
+-rw-rw-rw-   0        0        0    13494 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_catalogs.py
+-rw-rw-rw-   0        0        0    17511 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_checker.py
+-rw-rw-rw-   0        0        0     8878 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_conditions.py
+-rw-rw-rw-   0        0        0     6847 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_conformity.py
+-rw-rw-rw-   0        0        0    12329 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_contacts.py
+-rw-rw-rw-   0        0        0     9587 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_coordinate_systems.py
+-rw-rw-rw-   0        0        0    11990 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_datasources.py
+-rw-rw-rw-   0        0        0     5479 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_directives.py
+-rw-rw-rw-   0        0        0    10121 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_enums.py
+-rw-rw-rw-   0        0        0    10212 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_events.py
+-rw-rw-rw-   0        0        0    16151 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_feature_attributes.py
+-rw-rw-rw-   0        0        0     7002 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_formats.py
+-rw-rw-rw-   0        0        0    33394 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_keywords.py
+-rw-rw-rw-   0        0        0    13605 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_licenses.py
+-rw-rw-rw-   0        0        0    10637 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_limitations.py
+-rw-rw-rw-   0        0        0    10744 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_links.py
+-rw-rw-rw-   0        0        0    10964 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_metadatas_noGeo.py
+-rw-rw-rw-   0        0        0    10929 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_metadatas_vector.py
+-rw-rw-rw-   0        0        0    13188 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_search.py
+-rw-rw-rw-   0        0        0    16057 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_service_layers.py
+-rw-rw-rw-   0        0        0    11398 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_service_operations.py
+-rw-rw-rw-   0        0        0    14385 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_shares.py
+-rw-rw-rw-   0        0        0    14313 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_specifications.py
+-rw-rw-rw-   0        0        0     5781 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_thesauri.py
+-rw-rw-rw-   0        0        0     3867 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_token.py
+-rw-rw-rw-   0        0        0     5457 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_translator.py
+-rw-rw-rw-   0        0        0     4972 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_users.py
+-rw-rw-rw-   0        0        0    17075 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_utils.py
+-rw-rw-rw-   0        0        0     9312 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_utils_credentials.py
+-rw-rw-rw-   0        0        0     5532 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_utils_uuid.py
+-rw-rw-rw-   0        0        0    12714 2023-04-14 15:34:00.000000 isogeo-pysdk-3.8.1/tests/test_workgroups.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `isogeo-pysdk-3.8.0/LICENSE` & `isogeo-pysdk-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/PKG-INFO` & `isogeo-pysdk-3.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isogeo-pysdk
-Version: 3.8.0
+Version: 3.8.1
 Summary: API wrapper for the Isogeo REST API
 Home-page: https://github.com/isogeo/isogeo-api-py-minsdk/
 Author: Isogeo
 Author-email: contact@isogeo.com
 License: LGPL3
 Project-URL: Docs, https://isogeo-api-pysdk.readthedocs.io/
 Project-URL: Bug Reports, https://github.com/isogeo/isogeo-api-py-minsdk/issues/
```

### Comparing `isogeo-pysdk-3.8.0/README.md` & `isogeo-pysdk-3.8.1/README.md`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/__about__.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 ]
 
 
 __title__ = "Isogeo Python SDK"
 __summary__ = "API wrapper for the Isogeo REST API"
 __uri__ = "https://github.com/isogeo/isogeo-api-py-minsdk/"
 
-__version__ = "3.8.0"
+__version__ = "3.8.1"
 
 __author__ = "Isogeo"
 __email__ = "contact@isogeo.com"
 
 __license__ = "GNU Lesser General Public License v3.0"
 __copyright__ = "2016 - {0}, {1}".format(date.today().year, __author__)
```

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/__init__.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/__init__.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/__init__.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_about.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_about.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_account.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_account.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_application.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_application.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_catalog.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_catalog.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_condition.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_condition.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_conformity.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_conformity.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_contact.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_contact.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_coordinate_systems.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_coordinate_systems.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_datasource.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_datasource.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_directives.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_directives.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_event.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_event.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_feature_attributes.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_feature_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,16 +376,24 @@
                     metadata_source.type, metadata_dest.type
                 )
             )
         else:
             pass
 
         # retrieving attributes in source and destination to compare and adapt
-        attributes_source = self.listing(metadata_source)
+        if (
+            hasattr(metadata_source, "featureAttributes")
+            and isinstance(metadata_source.featureAttributes, list)
+            and len(metadata_source.featureAttributes)
+        ):
+            attributes_source = metadata_source.featureAttributes
+        else:
+            attributes_source = self.listing(metadata_source)
         attributes_dest = self.listing(metadata_dest)
+
         attributes_dest_names = [attr.get("name") for attr in attributes_dest]
         attributes_dest_names_low = [
             attr.get("name").lower() for attr in attributes_dest
         ]
 
         # according to the selected mode
         if mode == "add":
```

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_format.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_format.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_invitation.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_invitation.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_keyword.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_keyword.py`

 * *Files 0% similar despite different names*

```diff
@@ -794,26 +794,28 @@
 
         # check if keyword is already associated
         if check_exists:
             # search for all workgroup's keywords
             workgroup_existing_keywords = self.workgroup(
                 workgroup_id=workgroup._id, whole_results=True
             ).results
-            # fetch all workgroup's keywords' tags
-            workgroup_existing_keywords = [
-                kw.get("_tag")
-                for kw in workgroup_existing_keywords
-                if kw.get("_tag").startswith("keyword:isogeo:")
-                or kw.get("_tag").startswith("keyword:group-theme:")
-            ]
-
-            # then compare
-            if keyword._tag in workgroup_existing_keywords:
-                # return checker as true
-                return True, "already done"
+            if workgroup_existing_keywords is not None:
+                # fetch all workgroup's keywords' tags
+                workgroup_existing_keywords_tag = [
+                    kw.get("_tag")
+                    for kw in workgroup_existing_keywords
+                    if kw.get("_tag").startswith("keyword:isogeo:")
+                    or kw.get("_tag").startswith("keyword:group-theme:")
+                ]
+                # then compare
+                if keyword._tag in workgroup_existing_keywords_tag:
+                    # return checker as true
+                    return True, "already done"
+                else:
+                    pass
             else:
                 pass
         else:
             pass
 
         # URL
         url_keyword_associate_with_workgroup = self.utils.get_request_base_url(
```

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_license.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_license.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_limitation.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_limitation.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_link.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_link.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_metadata.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_metadata.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_metadata_bulk.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_metadata_bulk.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_search.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_search.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_service.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_service.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_service_layers.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_service_layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,14 +349,16 @@
 
         # check dataset metadata type
         if dataset.type not in (
             "rasterDataset",
             "vectorDataset",
             "raster-dataset",
             "vector-dataset",
+            "noGeoDataset",
+            "no-geo-dataset",
         ):
             raise TypeError(
                 "Datasets association with layers routes are only available for metadata of datasets, not: {}".format(
                     dataset.type
                 )
             )
         else:
@@ -444,14 +446,16 @@
 
         # check dataset metadata type
         if dataset.type not in (
             "rasterDataset",
             "vectorDataset",
             "raster-dataset",
             "vector-dataset",
+            "noGeoDataset",
+            "no-geo-dataset",
         ):
             raise TypeError(
                 "Datasets association with layers routes are only available for metadata of datasets, not: {}".format(
                     dataset.type
                 )
             )
         else:
```

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_service_operations.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_service_operations.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_share.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_share.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_specification.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_specification.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_thesaurus.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_thesaurus.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_user.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_user.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api/routes_workgroup.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api/routes_workgroup.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/api_hooks.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/api_hooks.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/checker.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/checker.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/decorators.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/decorators.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/__init__.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 from .limitation_types import LimitationTypes  # noqa: F401
 from .link_actions import LinkActions  # noqa: F401
 from .link_kinds import LinkKinds  # noqa: F401
 from .link_types import LinkTypes  # noqa: F401
 from .metadata_subresources import MetadataSubresources  # noqa: F401
 from .metadata_types import MetadataTypes  # noqa: F401
 from .search_filters_georelations import SearchGeoRelations  # noqa: F401
+from .service_layer_types import ServiceLayerTypes  # noqa: F401
 from .session_status import SessionStatus  # noqa: F401
 from .share_types import ShareTypes  # noqa: F401
 from .user_roles import UserRoles  # noqa: F401
 from .workgroup_statistics_tags import WorkgroupStatisticsTags  # noqa: F401
```

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/application_types.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/application_types.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/bulk_actions.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/bulk_actions.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/bulk_ignore_reasons.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/bulk_ignore_reasons.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/bulk_targets.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/bulk_targets.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/catalog_statistics_tags.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/catalog_statistics_tags.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/contact_roles.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/contact_roles.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/contact_types.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/contact_types.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/edition_profiles.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/edition_profiles.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/event_kinds.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/event_kinds.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/keyword_casing.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/keyword_casing.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/limitation_restrictions.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/limitation_restrictions.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/limitation_types.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/limitation_types.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/link_actions.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/link_actions.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/link_kinds.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/link_kinds.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/link_types.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/link_types.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/metadata_subresources.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/metadata_subresources.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/metadata_types.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/metadata_types.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/search_filters_georelations.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/search_filters_georelations.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/session_status.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/session_status.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/share_types.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/share_types.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/user_roles.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/user_roles.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/enums/workgroup_statistics_tags.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/enums/workgroup_statistics_tags.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/exceptions.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/isogeo.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/isogeo.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/__init__.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/application.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/application.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/bulk_report.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/bulk_report.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/bulk_request.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/bulk_request.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/catalog.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/catalog.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/condition.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/condition.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/conformity.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/conformity.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/contact.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/contact.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/coordinates_system.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/coordinates_system.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/datasource.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/datasource.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/directive.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/directive.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/event.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/event.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/feature_attributes.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/feature_attributes.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/format.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/format.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/invitation.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/invitation.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/keyword.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/keyword.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/keyword_search.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/keyword_search.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/license.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/license.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/limitation.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/limitation.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/link.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/link.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/metadata.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/metadata.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/metadata_search.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/metadata_search.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/service_layer.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/service_operation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: UTF-8 -*-
 #! python3  # noqa E265
 
 """
-    Isogeo API v1 - Model of ServiceLayer entity
+    Isogeo API v1 - Model of ServiceOperation entity
 
-    See: http://help.isogeo.com/api/complete/index.html#definition-serviceLayer
+    See: http://help.isogeo.com/api/complete/index.html#definition-serviceOperation
 """
 
 # #############################################################################
 # ########## Libraries #############
 # ##################################
 
 # standard library
@@ -17,223 +17,194 @@
 # submodels
 # from isogeo_pysdk.models.resource import Resource as Metadata
 
 
 # #############################################################################
 # ########## Classes ###############
 # ##################################
-class ServiceLayer(object):
-    """ServiceLayers are entities defining rules of data creation.
+class ServiceOperation(object):
+    """ServiceOperations are entities defining rules of data creation.
 
     :Example:
 
     .. code-block:: json
 
         {
             "_id": "string (uuid)",
-            "id": "string",
-            "mimeTypes": [
+            "mimeTypesIn": [
                 "string"
             ],
-            "titles": [
-                {
-                    "lang": "string",
-                    "value": "string"
-                }
+            "mimeTypesOut": [
+                "string"
             ],
-            "title": "string"
+            "name": "string",
+            "url": "string",
+            "verb": "string"
         }
     """
 
     ATTR_TYPES = {
         "_id": str,
-        "dataset": dict,
-        "datasets": list,
+        "mimeTypesIn": list,
+        "mimeTypesOut": list,
         "name": str,
-        "mimeTypes": str,
-        "titles": list,
-        "title": str,
+        "url": str,
+        "verb": str,
     }
 
-    ATTR_CREA = {"name": str, "titles": list, "title": str}
+    ATTR_CREA = {"name": str, "verb": str}
 
-    ATTR_MAP = {"name": "id"}
+    ATTR_MAP = {}
 
     def __init__(
         self,
         _id: str = None,
-        dataset: dict = None,
-        datasets: list = None,
-        id: str = None,
-        name: str = None,  # = id in API model but it's a reserved keyword in Python
-        mimeTypes: str = None,
-        titles: list = None,
-        title: str = None,
+        mimeTypesIn: str = None,
+        mimeTypesOut: str = None,
+        name: str = None,
+        url: str = None,
+        verb: str = None,
         # additional parameters
         parent_resource: str = None,
     ):
-        """ServiceLayer model."""
+        """ServiceOperation model."""
 
         # default values for the object attributes/properties
         self.__id = None
-        self._dataset = None
-        self._datasets = None
+        self._mimeTypesIn = None
+        self._mimeTypesOut = None
         self._name = None
-        self._mimeTypes = None
-        self._titles = None
-        self._title = None
+        self._url = None
+        self._verb = None
         # additional parameters
         self.parent_resource = parent_resource
 
         # if values have been passed, so use them as objects attributes.
         # attributes are prefixed by an underscore '_'
         if _id is not None:
             self.__id = _id
-        if id is not None:
-            self._name = id
-        if dataset is not None:
-            self._dataset = dataset
-        if datasets is not None:
-            self._datasets = datasets
+        if mimeTypesIn is not None:
+            self._mimeTypesIn = mimeTypesIn
+        if mimeTypesOut is not None:
+            self._mimeTypesOut = mimeTypesOut
         if name is not None:
             self._name = name
-        if mimeTypes is not None:
-            self._mimeTypes = mimeTypes
-        if titles is not None:
-            self._titles = titles
-        if title is not None:
-            self._title = title
+        if url is not None:
+            self._url = url
+        if verb is not None:
+            self._verb = verb
         # additional parameters
         if parent_resource is not None:
             self._parent_resource = parent_resource
 
     # -- PROPERTIES --------------------------------------------------------------------
     # service layer UUID
     @property
     def _id(self) -> str:
-        """Gets the id of this ServiceLayer.
+        """Gets the id of this ServiceOperation.
 
-        :return: The id of this ServiceLayer.
+        :return: The id of this ServiceOperation.
         :rtype: str
         """
         return self.__id
 
-    # service layer associated dataset
+    # service layer associated mimeTypesIn
     @property
-    def dataset(self) -> dict:
-        """Gets the dataset used for Isogeo filters of this ServiceLayer.
+    def mimeTypesIn(self) -> dict:
+        """Gets the mimeTypesIn used for Isogeo filters of this ServiceOperation.
 
-        :return: The dataset of this ServiceLayer.
+        :return: The mimeTypesIn of this ServiceOperation.
         :rtype: dict
         """
-        return self._dataset
+        return self._mimeTypesIn
 
-    @dataset.setter
-    def dataset(self, dataset: dict):
-        """Sets the dataset used into Isogeo filters of this ServiceLayer.
+    @mimeTypesIn.setter
+    def mimeTypesIn(self, mimeTypesIn: dict):
+        """Sets the mimeTypesIn used into Isogeo filters of this ServiceOperation.
 
-        :param dict dataset: the dataset of this ServiceLayer.
+        :param dict mimeTypesIn: the mimeTypesIn of this ServiceOperation.
         """
 
-        self._dataset = dataset
+        self._mimeTypesIn = mimeTypesIn
 
-    # service layer associated datasets
+    # mimeTypesOut
     @property
-    def datasets(self) -> list:
-        """Gets the datasets used for Isogeo filters of this ServiceLayer.
+    def mimeTypesOut(self) -> str:
+        """Gets the mimeTypesOut of this ServiceOperation.
 
-        :return: The datasets of this ServiceLayer.
-        :rtype: list
+        :return: The mimeTypesOut of this ServiceOperation.
+        :rtype: str
         """
-        return self._datasets
+        return self._mimeTypesOut
 
-    @datasets.setter
-    def datasets(self, datasets: list):
-        """Sets the datasets used into Isogeo filters of this ServiceLayer.
+    @mimeTypesOut.setter
+    def mimeTypesOut(self, mimeTypesOut: str):
+        """Sets the mimeTypesOut of this ServiceOperation.
 
-        :param list datasets: the datasets of this ServiceLayer.
+        :param str mimeTypesOut: The mimeTypesOut of this ServiceOperation.
         """
 
-        self._datasets = datasets
+        self._mimeTypesOut = mimeTypesOut
 
     # service layer name
     @property
     def name(self) -> str:
-        """Gets the name used for Isogeo filters of this ServiceLayer.
+        """Gets the name used for Isogeo filters of this ServiceOperation.
 
-        :return: The name of this ServiceLayer.
+        :return: The name of this ServiceOperation.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name: str):
-        """Sets the name used into Isogeo filters of this ServiceLayer.
+        """Sets the name used into Isogeo filters of this ServiceOperation.
 
-        :param str name: the name of this ServiceLayer.
+        :param str name: the name of this ServiceOperation.
         """
 
         self._name = name
 
-    # mimeTypes
-    @property
-    def mimeTypes(self) -> str:
-        """Gets the mimeTypes of this ServiceLayer.
-
-        :return: The mimeTypes of this ServiceLayer.
-        :rtype: str
-        """
-        return self._mimeTypes
-
-    @mimeTypes.setter
-    def mimeTypes(self, mimeTypes: str):
-        """Sets the mimeTypes of this ServiceLayer.
-
-        :param str mimeTypes: The mimeTypes of this ServiceLayer.
-        """
-
-        self._mimeTypes = mimeTypes
-
-    # titles
+    # url
     @property
-    def titles(self) -> list:
-        """Gets the titles of this ServiceLayer.
+    def url(self) -> list:
+        """Gets the url of this ServiceOperation.
 
-        :return: The titles of this ServiceLayer.
+        :return: The url of this ServiceOperation.
         :rtype: list
         """
-        return self._titles
+        return self._url
 
-    @titles.setter
-    def titles(self, titles: list):
-        """Sets the titles of this ServiceLayer.
+    @url.setter
+    def url(self, url: list):
+        """Sets the url of this ServiceOperation.
 
-        :param list titles: The titles of this ServiceLayer.
+        :param list url: The url of this ServiceOperation.
         """
 
-        self._titles = titles
+        self._url = url
 
-    # title
+    # verb
     @property
-    def title(self) -> str:
-        """Gets the title of this ServiceLayer.
+    def verb(self) -> list:
+        """Gets the verb of this ServiceOperation.
 
-        :return: The title of this ServiceLayer.
-        :rtype: str
+        :return: The verb of this ServiceOperation.
+        :rtype: list
         """
-        return self._title
+        return self._verb
 
-    @title.setter
-    def title(self, title: str):
-        """Sets the title of this ServiceLayer.
+    @verb.setter
+    def verb(self, verb: list):
+        """Sets the verb of this ServiceOperation.
 
-        :param str title: The title of this ServiceLayer.
+        :param list verb: The verb of this ServiceOperation.
         """
 
-        self._title = title
+        self._verb = verb
 
     # -- METHODS -----------------------------------------------------------------------
     def to_dict(self) -> dict:
         """Returns the model properties as a dict."""
         result = {}
 
         for attr, _ in self.ATTR_TYPES.items():
@@ -251,15 +222,15 @@
                         if hasattr(item[1], "to_dict")
                         else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(ServiceLayer, dict):
+        if issubclass(ServiceOperation, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_dict_creation(self) -> dict:
         """Returns the model properties as a dict structured for creation purpose (POST)"""
@@ -284,15 +255,15 @@
                         if hasattr(item[1], "to_dict")
                         else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(ServiceLayer, dict):
+        if issubclass(ServiceOperation, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self) -> str:
         """Returns the string representation of the model."""
@@ -300,29 +271,29 @@
 
     def __repr__(self) -> str:
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other) -> bool:
         """Returns true if both objects are equal."""
-        if not isinstance(other, ServiceLayer):
+        if not isinstance(other, ServiceOperation):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other) -> bool:
         """Returns true if both objects are not equal."""
         return not self == other
 
 
 # ##############################################################################
 # ##### Stand alone program ########
 # ##################################
 if __name__ == "__main__":
     """standalone execution."""
-    test_model = ServiceLayer()
+    test_model = ServiceOperation()
     print(test_model.__dict__)
     print(test_model._id)
     print(test_model.__dict__.get("_id"))
     print(hasattr(test_model, "_id"))
     print(test_model.to_dict_creation())
     # print(test_model.to_str()
```

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/service_operation.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/specification.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,210 +1,257 @@
 # -*- coding: UTF-8 -*-
 #! python3  # noqa E265
 
 """
-    Isogeo API v1 - Model of ServiceOperation entity
+    Isogeo API v1 - Model of Specification entity
+
+    See: http://help.isogeo.com/api/complete/index.html#definition-specification
 
-    See: http://help.isogeo.com/api/complete/index.html#definition-serviceOperation
 """
 
 # #############################################################################
 # ########## Libraries #############
 # ##################################
 
 # standard library
 import pprint
 
-# submodels
-# from isogeo_pysdk.models.resource import Resource as Metadata
-
 
 # #############################################################################
 # ########## Classes ###############
 # ##################################
-class ServiceOperation(object):
-    """ServiceOperations are entities defining rules of data creation.
+class Specification(object):
+    """Specifications are entities defining rules of data creation.
 
     :Example:
 
     .. code-block:: json
 
         {
-            "_id": "string (uuid)",
-            "mimeTypesIn": [
-                "string"
-            ],
-            "mimeTypesOut": [
-                "string"
-            ],
-            "name": "string",
-            "url": "string",
-            "verb": "string"
+            '_abilities': [],
+            '_id': 'string (uuid)',
+            '_tag': 'specification:isogeo:string (uuid)',
+            'count': int,
+            'link': string,
+            'name': string,
+            'published': '2016-06-30T00:00:00'
         }
     """
 
     ATTR_TYPES = {
+        "_abilities": str,
         "_id": str,
-        "mimeTypesIn": list,
-        "mimeTypesOut": list,
+        "_tag": str,
+        "count": int,
+        "link": str,
         "name": str,
-        "url": str,
-        "verb": str,
+        "owner": dict,
+        "published": str,
     }
 
-    ATTR_CREA = {"name": str, "verb": str}
+    ATTR_CREA = {"link": str, "name": str, "published": str}
 
     ATTR_MAP = {}
 
     def __init__(
         self,
+        _abilities: list = None,
         _id: str = None,
-        mimeTypesIn: str = None,
-        mimeTypesOut: str = None,
+        _tag: str = None,
+        count: int = None,
+        link: str = None,
         name: str = None,
-        url: str = None,
-        verb: str = None,
-        # additional parameters
-        parent_resource: str = None,
+        owner: dict = None,
+        published: str = None,
     ):
-        """ServiceOperation model."""
+        """Specification model."""
 
         # default values for the object attributes/properties
+        self.__abilities = None
         self.__id = None
-        self._mimeTypesIn = None
-        self._mimeTypesOut = None
+        self.__tag = None
+        self._count = None
+        self._link = None
         self._name = None
-        self._url = None
-        self._verb = None
-        # additional parameters
-        self.parent_resource = parent_resource
+        self._owner = None
+        self._published = None
 
         # if values have been passed, so use them as objects attributes.
         # attributes are prefixed by an underscore '_'
+        if _abilities is not None:
+            self.__abilities = _abilities
         if _id is not None:
             self.__id = _id
-        if mimeTypesIn is not None:
-            self._mimeTypesIn = mimeTypesIn
-        if mimeTypesOut is not None:
-            self._mimeTypesOut = mimeTypesOut
+        if _tag is not None:
+            self.__tag = _tag
+        if count is not None:
+            self._count = count
+        if link is not None:
+            self._link = link
         if name is not None:
             self._name = name
-        if url is not None:
-            self._url = url
-        if verb is not None:
-            self._verb = verb
-        # additional parameters
-        if parent_resource is not None:
-            self._parent_resource = parent_resource
+        if owner is not None:
+            self._owner = owner
+        if published is not None:
+            self._published = published
 
     # -- PROPERTIES --------------------------------------------------------------------
-    # service layer UUID
+    # abilities of the user related to the metadata
+    @property
+    def _abilities(self) -> str:
+        """Gets the abilities of this Catalog.
+
+        :return: The abilities of this Catalog.
+        :rtype: str
+        """
+        return self.__abilities
+
+    # specification UUID
     @property
     def _id(self) -> str:
-        """Gets the id of this ServiceOperation.
+        """Gets the id of this Specification.
 
-        :return: The id of this ServiceOperation.
+        :return: The id of this Specification.
         :rtype: str
         """
         return self.__id
 
-    # service layer associated mimeTypesIn
+    @_id.setter
+    def _id(self, _id: str):
+        """Sets the id of this Specification.
+
+        :param str id: The id of this Specification.
+        """
+
+        self.__id = _id
+
+    # specification UUID
+    @property
+    def _tag(self) -> str:
+        """Gets the tag used for Isogeo filters of this Specification.
+
+        :return: The tag of this Specification.
+        :rtype: str
+        """
+        return self.__tag
+
+    @_tag.setter
+    def _tag(self, _tag: str):
+        """Sets the tag used into Isogeo filters of this Specification.
+
+        :param str _tag: the tag of this Specification.
+        """
+
+        self.__tag = _tag
+
+    # count of resource linked to the specification
     @property
-    def mimeTypesIn(self) -> dict:
-        """Gets the mimeTypesIn used for Isogeo filters of this ServiceOperation.
+    def count(self) -> int:
+        """Gets the id of this Specification.
 
-        :return: The mimeTypesIn of this ServiceOperation.
-        :rtype: dict
+        :return: The id of this Specification.
+        :rtype: str
         """
-        return self._mimeTypesIn
+        return self._count
 
-    @mimeTypesIn.setter
-    def mimeTypesIn(self, mimeTypesIn: dict):
-        """Sets the mimeTypesIn used into Isogeo filters of this ServiceOperation.
+    @count.setter
+    def count(self, count: int):
+        """Sets the count of this Specification.
 
-        :param dict mimeTypesIn: the mimeTypesIn of this ServiceOperation.
+        :param int count: count of associated resources to the Specification
         """
 
-        self._mimeTypesIn = mimeTypesIn
+        self._count = count
 
-    # mimeTypesOut
+    # link
     @property
-    def mimeTypesOut(self) -> str:
-        """Gets the mimeTypesOut of this ServiceOperation.
+    def link(self) -> str:
+        """Gets the link (URL) of this Specification.
 
-        :return: The mimeTypesOut of this ServiceOperation.
+        :return: The link (URL) of this Specification.
         :rtype: str
         """
-        return self._mimeTypesOut
+        return self._link
 
-    @mimeTypesOut.setter
-    def mimeTypesOut(self, mimeTypesOut: str):
-        """Sets the mimeTypesOut of this ServiceOperation.
+    @link.setter
+    def link(self, link: str):
+        """Sets the id of this Specification.
 
-        :param str mimeTypesOut: The mimeTypesOut of this ServiceOperation.
+        :param str XX: The id of this Specification.
         """
 
-        self._mimeTypesOut = mimeTypesOut
+        self._link = link
 
-    # service layer name
+    # name
     @property
     def name(self) -> str:
-        """Gets the name used for Isogeo filters of this ServiceOperation.
+        """Gets the id of this Specification.
 
-        :return: The name of this ServiceOperation.
+        :return: The id of this Specification.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name: str):
-        """Sets the name used into Isogeo filters of this ServiceOperation.
+        """Sets the id of this Specification.
 
-        :param str name: the name of this ServiceOperation.
+        :param str XX: The id of this Specification.
         """
 
         self._name = name
 
-    # url
+    # workgroup owner
     @property
-    def url(self) -> list:
-        """Gets the url of this ServiceOperation.
+    def owner(self):
+        """Gets the owner of this Specification.
 
-        :return: The url of this ServiceOperation.
-        :rtype: list
+        :return: The owner of this Specification.
+        :rtype: Workgroup
         """
-        return self._url
+        return self._owner
 
-    @url.setter
-    def url(self, url: list):
-        """Sets the url of this ServiceOperation.
+    # published
+    @property
+    def published(self) -> str:
+        """Gets the zip (postal) code of this Specification.
 
-        :param list url: The url of this ServiceOperation.
+        :return: The zip (postal) code of this Specification.
+        :rtype: str
         """
+        return self._published
 
-        self._url = url
-
-    # verb
-    @property
-    def verb(self) -> list:
-        """Gets the verb of this ServiceOperation.
+    @published.setter
+    def published(self, published: str):
+        """Sets the zip (postal) code of this Specification.
 
-        :return: The verb of this ServiceOperation.
-        :rtype: list
+        :param str published: The zip (postal) code of this Specification.
         """
-        return self._verb
 
-    @verb.setter
-    def verb(self, verb: list):
-        """Sets the verb of this ServiceOperation.
+        self._published = published
 
-        :param list verb: The verb of this ServiceOperation.
-        """
+    # -- SPECIFIC TO IMPLEMENTATION ----------------------------------------------------
+    @property
+    def isLocked(self) -> bool or None:
+        """Shortcut to know if the Specification is owned by Isogeo or a workgroup.
 
-        self._verb = verb
+        :returns:
+            - None if tag is None too
+            - True if the specification is owned by Isogeo = locked
+            - False if the specification is owned by a workgroup = not locked
+        """
+        # if tag is not set, return None as well
+        if self._tag is None:
+            return None
+
+        # if tag is set, have a look
+        if ":isogeo:" in self._tag:
+            return True
+        else:
+            return False
 
     # -- METHODS -----------------------------------------------------------------------
     def to_dict(self) -> dict:
         """Returns the model properties as a dict."""
         result = {}
 
         for attr, _ in self.ATTR_TYPES.items():
@@ -222,15 +269,15 @@
                         if hasattr(item[1], "to_dict")
                         else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(ServiceOperation, dict):
+        if issubclass(Specification, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_dict_creation(self) -> dict:
         """Returns the model properties as a dict structured for creation purpose (POST)"""
@@ -255,15 +302,15 @@
                         if hasattr(item[1], "to_dict")
                         else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(ServiceOperation, dict):
+        if issubclass(Specification, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self) -> str:
         """Returns the string representation of the model."""
@@ -271,29 +318,29 @@
 
     def __repr__(self) -> str:
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other) -> bool:
         """Returns true if both objects are equal."""
-        if not isinstance(other, ServiceOperation):
+        if not isinstance(other, Specification):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other) -> bool:
         """Returns true if both objects are not equal."""
         return not self == other
 
 
 # ##############################################################################
 # ##### Stand alone program ########
 # ##################################
 if __name__ == "__main__":
     """standalone execution."""
-    test_model = ServiceOperation()
-    print(test_model.__dict__)
-    print(test_model._id)
-    print(test_model.__dict__.get("_id"))
-    print(hasattr(test_model, "_id"))
-    print(test_model.to_dict_creation())
-    # print(test_model.to_str()
+    ct = Specification()
+    print(ct.__dict__)
+    print(ct._id)
+    print(ct.__dict__.get("_id"))
+    print(hasattr(ct, "_id"))
+    print(ct.to_dict_creation())
+    # print(ct.to_str()
```

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/share.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/share.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/specification.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/user.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,257 +1,301 @@
 # -*- coding: UTF-8 -*-
 #! python3  # noqa E265
 
 """
-    Isogeo API v1 - Model of Specification entity
-
-    See: http://help.isogeo.com/api/complete/index.html#definition-specification
+    Isogeo API v1 - Model of User entity
 
+    See: http://help.isogeo.com/api/complete/index.html#definition-user
 """
 
 # #############################################################################
 # ########## Libraries #############
 # ##################################
 
 # standard library
 import pprint
 
+# submodels
+from isogeo_pysdk.models.contact import Contact
+
 
 # #############################################################################
 # ########## Classes ###############
 # ##################################
-class Specification(object):
-    """Specifications are entities defining rules of data creation.
+class User(object):
+    """Users in Isogeo platform.
 
     :Example:
 
     .. code-block:: json
 
         {
-            '_abilities': [],
-            '_id': 'string (uuid)',
-            '_tag': 'specification:isogeo:string (uuid)',
-            'count': int,
-            'link': string,
-            'name': string,
-            'published': '2016-06-30T00:00:00'
+            "_abilities": [
+                "string"
+            ],
+            "_created": "string (date-time)",
+            "_id": "string (uuid)",
+            "_modified": "string (date-time)",
+            "contact": {
+                "_created": "string (date-time)",
+                "_id": "string (uuid)",
+                "_modified": "string (date-time)",
+                "addressLine1": "string",
+                "addressLine2": "string",
+                "addressLine3": "string",
+                "available": "string",
+                "city": "string",
+                "count": "integer (int32)",
+                "countryCode": "string",
+                "email": "string",
+                "fax": "string",
+                "hash": "string",
+                "name": "string",
+                "organization": "string",
+                "phone": "string",
+                "type": "string",
+                "zipCode": "string"
+            },
+            "language": "string",
+            "staff": "boolean",
+            "timezone": "string"
         }
     """
 
     ATTR_TYPES = {
-        "_abilities": str,
+        "_abilities": list,
+        "_created": str,
         "_id": str,
-        "_tag": str,
-        "count": int,
-        "link": str,
-        "name": str,
-        "owner": dict,
-        "published": str,
+        "_modified": str,
+        "contact": Contact,
+        "language": str,
+        "mailchimp": dict,
+        "staff": bool,
+        "timezone": str,
     }
 
-    ATTR_CREA = {"link": str, "name": str, "published": str}
+    ATTR_CREA = {
+        "contact": Contact,
+        "language": str,
+        "mailchimp": str,
+        "staff": bool,
+        "timezone": str,
+    }
 
-    ATTR_MAP = {}
+    ATTR_MAP = {
+        # "staff": "IsOgeo"
+    }
 
     def __init__(
         self,
         _abilities: list = None,
+        _created: str = None,
         _id: str = None,
-        _tag: str = None,
-        count: int = None,
-        link: str = None,
-        name: str = None,
-        owner: dict = None,
-        published: str = None,
+        _modified: str = None,
+        contact: Contact = None,
+        language: str = None,
+        mailchimp: dict = None,
+        memberships: dict = None,
+        staff: bool = None,
+        timezone: str = None,
     ):
-        """Specification model."""
+        """User model."""
 
         # default values for the object attributes/properties
         self.__abilities = None
+        self.__created = None
         self.__id = None
-        self.__tag = None
-        self._count = None
-        self._link = None
-        self._name = None
-        self._owner = None
-        self._published = None
+        self.__modified = None
+        self._contact = Contact
+        self._language = None
+        self._mailchimp = None
+        self._memberships = None
+        self._staff = None
+        self._timezone = None
 
         # if values have been passed, so use them as objects attributes.
         # attributes are prefixed by an underscore '_'
         if _abilities is not None:
             self.__abilities = _abilities
+        if _created is not None:
+            self.__created = _created
         if _id is not None:
             self.__id = _id
-        if _tag is not None:
-            self.__tag = _tag
-        if count is not None:
-            self._count = count
-        if link is not None:
-            self._link = link
-        if name is not None:
-            self._name = name
-        if owner is not None:
-            self._owner = owner
-        if published is not None:
-            self._published = published
+        if _modified is not None:
+            self.__modified = _modified
+        if contact is not None:
+            self._contact = Contact(**contact)
+        if language is not None:
+            self._language = language
+        if mailchimp is not None:
+            self._mailchimp = mailchimp
+        if staff is not None:
+            self._staff = staff
+        if timezone is not None:
+            self._timezone = timezone
 
     # -- PROPERTIES --------------------------------------------------------------------
-    # abilities of the user related to the metadata
+    # abilities
     @property
-    def _abilities(self) -> str:
-        """Gets the abilities of this Catalog.
+    def _abilities(self):
+        """Gets the abilities of this User.  # noqa: E501.
 
-        :return: The abilities of this Catalog.
-        :rtype: str
+        :return: The abilities of this User.  # noqa: E501
+        :rtype: Abilities
         """
         return self.__abilities
 
-    # specification UUID
+    # creation date
+    @property
+    def _created(self) -> str:
+        """Gets the created used for Isogeo filters of this User.
+
+        :return: The created of this User.
+        :rtype: str
+        """
+        return self.__created
+
+    # user UUID
     @property
     def _id(self) -> str:
-        """Gets the id of this Specification.
+        """Gets the id of this User.
 
-        :return: The id of this Specification.
+        :return: The id of this User.
         :rtype: str
         """
         return self.__id
 
-    @_id.setter
-    def _id(self, _id: str):
-        """Sets the id of this Specification.
+    # last update
+    @property
+    def _modified(self) -> str:
+        """Gets the modified used for Isogeo filters of this User.
 
-        :param str id: The id of this Specification.
+        :return: The modified of this User.
+        :rtype: str
         """
+        return self.__modified
 
-        self.__id = _id
-
-    # specification UUID
+    # contact
     @property
-    def _tag(self) -> str:
-        """Gets the tag used for Isogeo filters of this Specification.
+    def contact(self) -> Contact:
+        """Gets the contact of this user.
 
-        :return: The tag of this Specification.
-        :rtype: str
+        :return: The contact of this user.
+        :rtype: Contact
         """
-        return self.__tag
+        return self._contact
 
-    @_tag.setter
-    def _tag(self, _tag: str):
-        """Sets the tag used into Isogeo filters of this Specification.
+    @contact.setter
+    def contact(self, contact: Contact):
+        """Sets the contact of this user.
 
-        :param str _tag: the tag of this Specification.
+        :param dict contact: The contact of this user.
         """
 
-        self.__tag = _tag
+        if contact is None:
+            raise ValueError("Invalid value for `contact`, must not be `None`")
 
-    # count of resource linked to the specification
+        self._contact = Contact(**contact)
+
+    # language
     @property
-    def count(self) -> int:
-        """Gets the id of this Specification.
+    def language(self) -> str:
+        """Gets the id of this User.
 
-        :return: The id of this Specification.
+        :return: The id of this User.
         :rtype: str
         """
-        return self._count
+        return self._language
 
-    @count.setter
-    def count(self, count: int):
-        """Sets the count of this Specification.
+    @language.setter
+    def language(self, language: str):
+        """Sets the first line of the address of this User.
 
-        :param int count: count of associated resources to the Specification
+        :param str language: The first address line of this User.
         """
 
-        self._count = count
+        self._language = language
 
-    # link
+    # mailchimp subscriptions
     @property
-    def link(self) -> str:
-        """Gets the link (URL) of this Specification.
+    def mailchimp(self) -> str:
+        """Gets the id of this User.
 
-        :return: The link (URL) of this Specification.
+        :return: The second address line of this User.
         :rtype: str
         """
-        return self._link
+        return self._mailchimp
 
-    @link.setter
-    def link(self, link: str):
-        """Sets the id of this Specification.
+    @mailchimp.setter
+    def mailchimp(self, mailchimp: str):
+        """Sets the id of this User.
 
-        :param str XX: The id of this Specification.
+        :param str mailchimp: The second address line of this User.
         """
 
-        self._link = link
+        self._mailchimp = mailchimp
 
-    # name
+    # staff status
     @property
-    def name(self) -> str:
-        """Gets the id of this Specification.
+    def staff(self) -> bool:
+        """Staff status for the User.
 
-        :return: The id of this Specification.
-        :rtype: str
+        :return: the staff status of the User
+        :rtype: bool
         """
-        return self._name
+        return self._staff
 
-    @name.setter
-    def name(self, name: str):
-        """Sets the id of this Specification.
+    @staff.setter
+    def staff(self, staff: bool):
+        """Sets the staff status of this User.
 
-        :param str XX: The id of this Specification.
+        :param bool staff: The new staff status for the User.
         """
 
-        self._name = name
-
-    # workgroup owner
-    @property
-    def owner(self):
-        """Gets the owner of this Specification.
-
-        :return: The owner of this Specification.
-        :rtype: Workgroup
-        """
-        return self._owner
+        self._staff = staff
 
-    # published
+    # timezone
     @property
-    def published(self) -> str:
-        """Gets the zip (postal) code of this Specification.
+    def timezone(self) -> str:
+        """Gets the timezone of this User.
 
-        :return: The zip (postal) code of this Specification.
+        :return: The timezone of this User.
         :rtype: str
         """
-        return self._published
+        return self._timezone
 
-    @published.setter
-    def published(self, published: str):
-        """Sets the zip (postal) code of this Specification.
+    @timezone.setter
+    def timezone(self, timezone: str):
+        """Sets the timezone of this User.
 
-        :param str published: The zip (postal) code of this Specification.
+        :param str timezone: The timezone of this User.
         """
 
-        self._published = published
+        self._timezone = timezone
 
     # -- SPECIFIC TO IMPLEMENTATION ----------------------------------------------------
     @property
-    def isLocked(self) -> bool or None:
-        """Shortcut to know if the Specification is owned by Isogeo or a workgroup.
-
-        :returns:
-            - None if tag is None too
-            - True if the specification is owned by Isogeo = locked
-            - False if the specification is owned by a workgroup = not locked
-        """
-        # if tag is not set, return None as well
-        if self._tag is None:
+    def name(self) -> str:
+        """Shortcut to get the name from the contact data linked to the user."""
+        if isinstance(self._contact, dict):
+            return self._contact.get("name")
+        elif isinstance(self._contact, Contact):
+            return self._contact.name
+        else:
             return None
 
-        # if tag is set, have a look
-        if ":isogeo:" in self._tag:
-            return True
+    @property
+    def email(self) -> str:
+        """Shortcut to get the email from the contact data linked to the user."""
+        if isinstance(self._contact, dict):
+            return self._contact.get("email")
+        elif isinstance(self.contact, Contact):
+            return self.contact.email
         else:
-            return False
+            return None
 
     # -- METHODS -----------------------------------------------------------------------
     def to_dict(self) -> dict:
         """Returns the model properties as a dict."""
         result = {}
 
         for attr, _ in self.ATTR_TYPES.items():
@@ -269,15 +313,15 @@
                         if hasattr(item[1], "to_dict")
                         else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(Specification, dict):
+        if issubclass(User, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_dict_creation(self) -> dict:
         """Returns the model properties as a dict structured for creation purpose (POST)"""
@@ -302,15 +346,15 @@
                         if hasattr(item[1], "to_dict")
                         else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(Specification, dict):
+        if issubclass(User, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self) -> str:
         """Returns the string representation of the model."""
@@ -318,29 +362,24 @@
 
     def __repr__(self) -> str:
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other) -> bool:
         """Returns true if both objects are equal."""
-        if not isinstance(other, Specification):
+        if not isinstance(other, User):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other) -> bool:
         """Returns true if both objects are not equal."""
         return not self == other
 
 
 # ##############################################################################
 # ##### Stand alone program ########
 # ##################################
 if __name__ == "__main__":
     """standalone execution."""
-    ct = Specification()
-    print(ct.__dict__)
-    print(ct._id)
-    print(ct.__dict__.get("_id"))
-    print(hasattr(ct, "_id"))
-    print(ct.to_dict_creation())
-    # print(ct.to_str()
+    obj = User()
+    print(obj)
```

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/thesaurus.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/thesaurus.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/models/workgroup.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/models/workgroup.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/samples/attributes_frequency.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/attributes_frequency.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/samples/download_batch_hosted_data.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/download_batch_hosted_data.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/samples/export_batch_xml19139_sync.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/export_batch_xml19139_sync.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/samples/get_OpenCatalog.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/get_OpenCatalog.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/samples/latest_md_modified.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/latest_md_modified.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/samples/related_links.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/related_links.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/samples/results_parser.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/results_parser.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/samples/search.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/search.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/samples/spatial_search.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/spatial_search.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/samples/store_api_responses_read.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/store_api_responses_read.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/samples/store_api_responses_rw.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/samples/store_api_responses_rw.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/translator.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/translator.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/type_hints_custom.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/type_hints_custom.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk/utils.py` & `isogeo-pysdk-3.8.1/isogeo_pysdk/utils.py`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk.egg-info/PKG-INFO` & `isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isogeo-pysdk
-Version: 3.8.0
+Version: 3.8.1
 Summary: API wrapper for the Isogeo REST API
 Home-page: https://github.com/isogeo/isogeo-api-py-minsdk/
 Author: Isogeo
 Author-email: contact@isogeo.com
 License: LGPL3
 Project-URL: Docs, https://isogeo-api-pysdk.readthedocs.io/
 Project-URL: Bug Reports, https://github.com/isogeo/isogeo-api-py-minsdk/issues/
```

### Comparing `isogeo-pysdk-3.8.0/isogeo_pysdk.egg-info/SOURCES.txt` & `isogeo-pysdk-3.8.1/isogeo_pysdk.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 isogeo_pysdk/enums/limitation_types.py
 isogeo_pysdk/enums/link_actions.py
 isogeo_pysdk/enums/link_kinds.py
 isogeo_pysdk/enums/link_types.py
 isogeo_pysdk/enums/metadata_subresources.py
 isogeo_pysdk/enums/metadata_types.py
 isogeo_pysdk/enums/search_filters_georelations.py
+isogeo_pysdk/enums/service_layer_types.py
 isogeo_pysdk/enums/session_status.py
 isogeo_pysdk/enums/share_types.py
 isogeo_pysdk/enums/user_roles.py
 isogeo_pysdk/enums/workgroup_statistics_tags.py
 isogeo_pysdk/models/__init__.py
 isogeo_pysdk/models/application.py
 isogeo_pysdk/models/bulk_report.py
@@ -106,8 +107,44 @@
 isogeo_pysdk/samples/get_OpenCatalog.py
 isogeo_pysdk/samples/latest_md_modified.py
 isogeo_pysdk/samples/related_links.py
 isogeo_pysdk/samples/results_parser.py
 isogeo_pysdk/samples/search.py
 isogeo_pysdk/samples/spatial_search.py
 isogeo_pysdk/samples/store_api_responses_read.py
-isogeo_pysdk/samples/store_api_responses_rw.py
+isogeo_pysdk/samples/store_api_responses_rw.py
+tests/test_about.py
+tests/test_account.py
+tests/test_applications.py
+tests/test_authentication.py
+tests/test_bulks.py
+tests/test_catalogs.py
+tests/test_checker.py
+tests/test_conditions.py
+tests/test_conformity.py
+tests/test_contacts.py
+tests/test_coordinate_systems.py
+tests/test_datasources.py
+tests/test_directives.py
+tests/test_enums.py
+tests/test_events.py
+tests/test_feature_attributes.py
+tests/test_formats.py
+tests/test_keywords.py
+tests/test_licenses.py
+tests/test_limitations.py
+tests/test_links.py
+tests/test_metadatas_noGeo.py
+tests/test_metadatas_vector.py
+tests/test_search.py
+tests/test_service_layers.py
+tests/test_service_operations.py
+tests/test_shares.py
+tests/test_specifications.py
+tests/test_thesauri.py
+tests/test_token.py
+tests/test_translator.py
+tests/test_users.py
+tests/test_utils.py
+tests/test_utils_credentials.py
+tests/test_utils_uuid.py
+tests/test_workgroups.py
```

### Comparing `isogeo-pysdk-3.8.0/setup.cfg` & `isogeo-pysdk-3.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `isogeo-pysdk-3.8.0/setup.py` & `isogeo-pysdk-3.8.1/setup.py`

 * *Files identical despite different names*

