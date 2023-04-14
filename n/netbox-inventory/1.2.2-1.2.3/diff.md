# Comparing `tmp/netbox-inventory-1.2.2.tar.gz` & `tmp/netbox-inventory-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-inventory-1.2.2.tar", last modified: Sun Apr  9 17:57:54 2023, max compression
+gzip compressed data, was "netbox-inventory-1.2.3.tar", last modified: Fri Apr 14 11:39:57 2023, max compression
```

## Comparing `netbox-inventory-1.2.2.tar` & `netbox-inventory-1.2.3.tar`

### file list

```diff
@@ -1,103 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.173767 netbox-inventory-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-04-09 17:57:54.173767 netbox-inventory-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.165767 netbox-inventory-1.2.2/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/analyzers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.165767 netbox-inventory-1.2.2/netbox_inventory/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.165767 netbox-inventory-1.2.2/netbox_inventory/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/forms/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/forms/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/forms/bulk_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/forms/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/forms/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.169767 netbox-inventory-1.2.2/netbox_inventory/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/migrations/0001_initial_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/migrations/0002_alter_asset_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.161767 netbox-inventory-1.2.2/netbox_inventory/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.169767 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset.html
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset_assign.html
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset_create.html
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.169767 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/purchase.html
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/supplier.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.169767 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.169767 netbox-inventory-1.2.2/netbox_inventory/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.169767 netbox-inventory-1.2.2/netbox_inventory/tests/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/asset/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/asset/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/asset/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.169767 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_group/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_group/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.173767 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_type/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_type/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.173767 netbox-inventory-1.2.2/netbox_inventory/tests/purchase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/purchase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/purchase/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/purchase/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.173767 netbox-inventory-1.2.2/netbox_inventory/tests/supplier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/supplier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/supplier/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/supplier/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.173767 netbox-inventory-1.2.2/netbox_inventory/views/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/asset_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/asset_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/inventoryitem_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/inventoryitem_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/purchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/netbox_inventory/views/tabs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:57:54.165767 netbox-inventory-1.2.2/netbox_inventory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-04-09 17:57:54.000000 netbox-inventory-1.2.2/netbox_inventory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-09 17:57:54.000000 netbox-inventory-1.2.2/netbox_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:57:54.000000 netbox-inventory-1.2.2/netbox_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-09 17:57:54.000000 netbox-inventory-1.2.2/netbox_inventory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-09 17:57:45.000000 netbox-inventory-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 17:57:54.173767 netbox-inventory-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.870301 netbox-inventory-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-04-14 11:39:57.866301 netbox-inventory-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.854301 netbox-inventory-1.2.3/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.858301 netbox-inventory-1.2.3/netbox_inventory/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.858301 netbox-inventory-1.2.3/netbox_inventory/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17266 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/bulk_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/forms/reassign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.858301 netbox-inventory-1.2.3/netbox_inventory/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/migrations/0001_initial_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/migrations/0002_alter_asset_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.850301 netbox-inventory-1.2.3/netbox_inventory/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.862301 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_assign.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_reassign.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.862301 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_tenant.html
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/purchase.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/supplier.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.862301 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.862301 netbox-inventory-1.2.3/netbox_inventory/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.866301 netbox-inventory-1.2.3/netbox_inventory/tests/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_views_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_views_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.866301 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_group/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_group/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.866301 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_type/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_type/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.866301 netbox-inventory-1.2.3/netbox_inventory/tests/purchase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/purchase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/purchase/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/purchase/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.866301 netbox-inventory-1.2.3/netbox_inventory/tests/supplier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/supplier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/supplier/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/supplier/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.866301 netbox-inventory-1.2.3/netbox_inventory/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/asset_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/asset_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/asset_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/inventoryitem_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/inventoryitem_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/purchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/netbox_inventory/views/tabs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:39:57.854301 netbox-inventory-1.2.3/netbox_inventory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-04-14 11:39:57.000000 netbox-inventory-1.2.3/netbox_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-14 11:39:57.000000 netbox-inventory-1.2.3/netbox_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:39:57.000000 netbox-inventory-1.2.3/netbox_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 11:39:57.000000 netbox-inventory-1.2.3/netbox_inventory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-14 11:39:49.000000 netbox-inventory-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 11:39:57.870301 netbox-inventory-1.2.3/setup.cfg
```

### Comparing `netbox-inventory-1.2.2/LICENSE` & `netbox-inventory-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/PKG-INFO` & `netbox-inventory-1.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.2.2
+Version: 1.2.3
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,26 +20,36 @@
 ## Features
 
 Keep track of your hardware, whether it is installed or in storage. You can
 define assets that represent hardware that can be used as a device, module or
 inventory item in NetBox.
 
 Each asset can have a storage location defined, when not in use. You can assign
-an asset to a device or module. The plugin can keep serial number and asset tag
-between asset and device or module in sync if enabled in settings.
+an asset to a device, module or inventory item. The plugin can keep serial number
+and asset tag between asset and device, module or inventory item in sync if
+enabled in settings.
+
+On Site and Location detail views there is a new tab Assets that can show assets
+that are stored or installed at that location or both. Rack details view also has
+a tab for installed Assets. This provides a unified view of all assets at a given
+location.
 
 To properly support inventory items (that are used in NetBox to model SFP and
 similar modules) the plugin defines inventory item types that are equivalent to
 device types and module types. 
 
 Inventory item types can be assigned into inventory item groups. On a group detail
 view you have an overview of the number of contained assets broken down by asset
 status or inventory item type and status. This way you can quickly see how many
 of a certain type of hardware you still have spare.
 
+Inventory item groups can be nested, so you can for example model all pluggables
+as one top-level group with child groups for SFP+ modules, SFP28 modules and so
+on.
+
 ### Automatic management of asset status
 
 Each asset has a status attribute that can indicate use of the asset. These
 statuses can be set as needed by each NetBox installation.
 
 Two statuses can have a special meaning. One to indicate asset is in storage and one
 to indicate asset is in use.
@@ -151,14 +161,15 @@
 | `used_status_name` | `'used'`| Status that indicates asset is in use. See "Automatic management of asset status" below for more info on this setting.
 | `stored_status_name` | `'stored'`| Status that indicates asset is in storage. See "Automatic management of asset status" below for more info on this setting.
 | `sync_hardware_serial_asset_tag` | `False` | When an asset is assigned or unassigned to a device, module or inventory item, update its serial number and asset tag to be in sync with the asset? |
 | `asset_import_create_purchase` | `False` | When importing assets, automatically create purchase (and supplier) if it doesn't exist |
 | `asset_import_create_device_type` | `False` | When importing a device type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_module_type` | `False` | When importing a module type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_inventoryitem_type` | `False` | When importing an inventory type asset, automatically create manufacturer and/or device type if it doesn't exist |
+| `asset_import_create_tenant` | `False` | When importing an asset, with owner or tenant, automatically create tenant if it doesn't exist |
 | `asset_disable_editing_fields_for_tags` | `{}` | A dictionary of tags and fields that should be disabled for editing. This is useful if you want to prevent editing of certain fields for certain assets. The dictionary is in the form of `{tag: [field1, field2]}`. Example: `{'no-edit': ['serial_number', 'asset_tag']}`. This only affects the UI, the API can still be used to edit the fields. |
 | `asset_disable_deletion_for_tags` | `[]` | List of tags that will disable deletion of assets. This only affects the UI, not the API. |
 
 You can extend or define your own status choices for Asset, via [`FIELD_CHOICES`](https://docs.netbox.dev/en/stable/configuration/data-validation/#field_choices) setting in Netbox:
 
 ```
 FIELD_CHOICES = {
```

### Comparing `netbox-inventory-1.2.2/README.md` & `netbox-inventory-1.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,36 @@
 ## Features
 
 Keep track of your hardware, whether it is installed or in storage. You can
 define assets that represent hardware that can be used as a device, module or
 inventory item in NetBox.
 
 Each asset can have a storage location defined, when not in use. You can assign
-an asset to a device or module. The plugin can keep serial number and asset tag
-between asset and device or module in sync if enabled in settings.
+an asset to a device, module or inventory item. The plugin can keep serial number
+and asset tag between asset and device, module or inventory item in sync if
+enabled in settings.
+
+On Site and Location detail views there is a new tab Assets that can show assets
+that are stored or installed at that location or both. Rack details view also has
+a tab for installed Assets. This provides a unified view of all assets at a given
+location.
 
 To properly support inventory items (that are used in NetBox to model SFP and
 similar modules) the plugin defines inventory item types that are equivalent to
 device types and module types. 
 
 Inventory item types can be assigned into inventory item groups. On a group detail
 view you have an overview of the number of contained assets broken down by asset
 status or inventory item type and status. This way you can quickly see how many
 of a certain type of hardware you still have spare.
 
+Inventory item groups can be nested, so you can for example model all pluggables
+as one top-level group with child groups for SFP+ modules, SFP28 modules and so
+on.
+
 ### Automatic management of asset status
 
 Each asset has a status attribute that can indicate use of the asset. These
 statuses can be set as needed by each NetBox installation.
 
 Two statuses can have a special meaning. One to indicate asset is in storage and one
 to indicate asset is in use.
@@ -136,14 +146,15 @@
 | `used_status_name` | `'used'`| Status that indicates asset is in use. See "Automatic management of asset status" below for more info on this setting.
 | `stored_status_name` | `'stored'`| Status that indicates asset is in storage. See "Automatic management of asset status" below for more info on this setting.
 | `sync_hardware_serial_asset_tag` | `False` | When an asset is assigned or unassigned to a device, module or inventory item, update its serial number and asset tag to be in sync with the asset? |
 | `asset_import_create_purchase` | `False` | When importing assets, automatically create purchase (and supplier) if it doesn't exist |
 | `asset_import_create_device_type` | `False` | When importing a device type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_module_type` | `False` | When importing a module type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_inventoryitem_type` | `False` | When importing an inventory type asset, automatically create manufacturer and/or device type if it doesn't exist |
+| `asset_import_create_tenant` | `False` | When importing an asset, with owner or tenant, automatically create tenant if it doesn't exist |
 | `asset_disable_editing_fields_for_tags` | `{}` | A dictionary of tags and fields that should be disabled for editing. This is useful if you want to prevent editing of certain fields for certain assets. The dictionary is in the form of `{tag: [field1, field2]}`. Example: `{'no-edit': ['serial_number', 'asset_tag']}`. This only affects the UI, the API can still be used to edit the fields. |
 | `asset_disable_deletion_for_tags` | `[]` | List of tags that will disable deletion of assets. This only affects the UI, not the API. |
 
 You can extend or define your own status choices for Asset, via [`FIELD_CHOICES`](https://docs.netbox.dev/en/stable/configuration/data-validation/#field_choices) setting in Netbox:
 
 ```
 FIELD_CHOICES = {
```

### Comparing `netbox-inventory-1.2.2/netbox_inventory/__init__.py` & `netbox-inventory-1.2.3/netbox_inventory/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         'used_status_name': 'used',
         'stored_status_name': 'stored',
         'sync_hardware_serial_asset_tag': False,
         'asset_import_create_purchase': False,
         'asset_import_create_device_type': False,
         'asset_import_create_module_type': False,
         'asset_import_create_inventoryitem_type': False,
+        'asset_import_create_tenant': False,
         'asset_disable_editing_fields_for_tags': {},
         'asset_disable_deletion_for_tags': [],
     }
 
     def ready(self):
         super().ready()
         import netbox_inventory.signals
```

### Comparing `netbox-inventory-1.2.2/netbox_inventory/analyzers.py` & `netbox-inventory-1.2.3/netbox_inventory/analyzers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/api/nested_serializers.py` & `netbox-inventory-1.2.3/netbox_inventory/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/api/serializers.py` & `netbox-inventory-1.2.3/netbox_inventory/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/api/urls.py` & `netbox-inventory-1.2.3/netbox_inventory/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/api/views.py` & `netbox-inventory-1.2.3/netbox_inventory/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/filtersets.py` & `netbox-inventory-1.2.3/netbox_inventory/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/forms/assign.py` & `netbox-inventory-1.2.3/netbox_inventory/forms/assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/forms/bulk.py` & `netbox-inventory-1.2.3/netbox_inventory/forms/bulk.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dcim.models import DeviceType, Manufacturer, ModuleType, Location, Site
 from netbox.forms import NetBoxModelBulkEditForm, NetBoxModelImportForm
 from utilities.forms import (
     add_blank_choice, ChoiceField, CommentField, CSVChoiceField,
     CSVModelChoiceField, DynamicModelChoiceField
 )
-from tenancy.models import Tenant
+from tenancy.models import Contact, Tenant
 from ..choices import AssetStatusChoices, HardwareKindChoices
 from ..models import Asset, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 from ..utils import get_plugin_setting
 
 __all__ = (
     'AssetBulkEditForm',
     'AssetImportForm',
@@ -111,15 +111,15 @@
         queryset=Manufacturer.objects.all(),
         to_field_name='name',
         required=True,
         help_text='Hardware manufacturer.'
     )
     model_name = forms.CharField(
         required=True,
-        help_text='Model of this device/module/inventory item type. See "Import settings" below for more info.',
+        help_text='Model of this device/module/inventory item type. See "Import settings" for more info.',
     )
     part_number = forms.CharField(
         required=False,
         help_text='Discrete part number for model. Only used if creating new model.',
     )
     model_comments = forms.CharField(
         required=False,
@@ -146,36 +146,48 @@
         to_field_name='name',
         help_text='Tenant that owns this asset. It must exist before import.',
         required=False,
     )
     purchase = CSVModelChoiceField(
         queryset=Purchase.objects.all(),
         to_field_name='name',
-        help_text='Purchase through which this asset was purchased. See "Import settings" below for more info.',
+        help_text='Purchase through which this asset was purchased. See "Import settings" for more info.',
         required=False,
     )
     purchase_date = forms.DateField(
         help_text='Date when this purchase was made.',
         required=False,
     )
     supplier = CSVModelChoiceField(
         queryset=Supplier.objects.all(),
         to_field_name='name',
         help_text='Legal entity this purchase was made from. Required if a new purchase was given.',
         required=False,
     )
+    tenant = CSVModelChoiceField(
+        queryset=Tenant.objects.all(),
+        to_field_name='name',
+        help_text='Tenant using this asset. See "Import settings" for more info.',
+        required=False,
+    )
+    contact = CSVModelChoiceField(
+        queryset=Contact.objects.all(),
+        to_field_name='name',
+        help_text='Contact using this asset. It must exist before import.',
+        required=False,
+    )
 
     class Meta:
         model = Asset
         fields = (
             'name', 'asset_tag', 'serial', 'status',
             'hardware_kind', 'manufacturer', 'model_name', 'part_number',
             'model_comments', 'storage_site', 'storage_location',
             'owner', 'purchase', 'purchase_date', 'supplier',
-            'warranty_start', 'warranty_end', 'comments',
+            'warranty_start', 'warranty_end', 'comments', 'tenant', 'contact',
         )
 
     def clean_model_name(self):
         hardware_kind = self.cleaned_data.get('hardware_kind')
         manufacturer = self.cleaned_data.get('manufacturer')
         model = self.cleaned_data.get('model_name')
         if not hardware_kind or not manufacturer:
@@ -234,80 +246,88 @@
         """
         try:
             # handle creating related resources if they don't exist and enabled in settings
             if (get_plugin_setting('asset_import_create_purchase')
                 and self.data.get('purchase') and self.data.get('supplier')):
                 Purchase.objects.get_or_create(
                     name=self.data.get('purchase'),
-                    supplier=self._get_or_create_supplier(),
+                    supplier=self._get_or_create_related('supplier'),
                     defaults={'date': self._get_clean_value('purchase_date')}
                 )
             if (get_plugin_setting('asset_import_create_device_type')
                 and self.data.get('hardware_kind') == 'device'):
                 DeviceType.objects.get_or_create(
                     model__iexact=self.data.get('model_name'),
-                    manufacturer=self._get_or_create_manufacturer(),
+                    manufacturer=self._get_or_create_related('manufacturer'),
                     defaults={
                         'model': self.data.get('model_name'),
                         'slug': slugify(self.data.get('model_name')),
                         'part_number': self._get_clean_value('part_number'),
                         'comments': self._get_clean_value('model_comments'),
                     },
                 )
             if (get_plugin_setting('asset_import_create_module_type')
                 and self.data.get('hardware_kind') == 'module'):
                 ModuleType.objects.get_or_create(
                     model__iexact=self.data.get('model_name'),
-                    manufacturer=self._get_or_create_manufacturer(),
+                    manufacturer=self._get_or_create_related('manufacturer'),
                     defaults={
                         'model': self.data.get('model_name'),
                         'part_number': self._get_clean_value('part_number'),
                         'comments': self._get_clean_value('model_comments'),
                     },
                 )
             if (get_plugin_setting('asset_import_create_inventoryitem_type')
                 and self.data.get('hardware_kind') == 'inventoryitem'):
                 InventoryItemType.objects.get_or_create(
                     model__iexact=self.data.get('model_name'),
-                    manufacturer=self._get_or_create_manufacturer(),
+                    manufacturer=self._get_or_create_related('manufacturer'),
                     defaults={
                         'model': self.data.get('model_name'),
                         'slug': slugify(self.data.get('model_name')),
                         'part_number': self._get_clean_value('part_number'),
                         'comments': self._get_clean_value('model_comments'),
                     },
                 )
+            if (get_plugin_setting('asset_import_create_tenant')
+                and self.data.get('tenant')):
+                self._get_or_create_related('tenant')
+            if (get_plugin_setting('asset_import_create_tenant')
+                and self.data.get('owner')):
+                self._get_or_create_related('owner')
         except forms.ValidationError as e:
             # ValidationErrors are raised by _clean_fields() method
             # this will be called later in the code and will be bound
             # to correct field. So we skiup this kinds of errors here.
             pass
         except Exception as e:
             # any other errors we add to non-field specific form errors
             self.add_error(None, e)
 
-    def _get_or_create_manufacturer(self):
-        manufacturer, _ = Manufacturer.objects.get_or_create(
-            name__iexact=self.data.get('manufacturer'),
-            defaults={
-                'name': self.data.get('manufacturer'),
-                'slug': slugify(self.data.get('manufacturer'))
-            },
-        )
-        return manufacturer
-
-    def _get_or_create_supplier(self):
-        supplier, _ = Supplier.objects.get_or_create(
-            name__iexact=self.data.get('supplier'),
-            defaults={
-                'name': self.data.get('supplier'),
-                'slug': slugify(self.data.get('supplier'))
-            }
+    def _get_or_create_related(self, field_name):
+        """
+        Create instance of related object if it doesn't exist.
+        Supports specifiying related object by name or slug.
+        """
+        klass = self.fields[field_name].queryset.model
+        # user could have specified alternative field (tenant name or tenant slug)
+        to_field_name = self.fields[field_name].to_field_name
+        # create sensible default data if we'll need to create object
+        instance_defaults = {
+            'name': self.data.get(field_name),
+            'slug': slugify(self.data.get(field_name)),
+        }
+        # whatever field was in import data is used as is
+        instance_defaults.update({to_field_name: self.data.get(field_name)})
+        instance, _ = klass.objects.get_or_create(
+            # filter on field specified in column header
+            **{to_field_name+'__iexact':self.data.get(field_name)},
+            defaults=instance_defaults
         )
-        return supplier
+        return instance
 
     def _get_clean_value(self, field_name):
         """
         Returns cleaned value for a given field from self.data
         Used when creating additional related objects on import, since the values
         are otherwise not validated by forms.
         Used for DateTime, Boolean and similar fields. If used on ModelField and
```

### Comparing `netbox-inventory-1.2.2/netbox_inventory/forms/create.py` & `netbox-inventory-1.2.3/netbox_inventory/forms/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         if self.instance.assigned_asset:
             asset = self.instance.assigned_asset
             self.fields['serial'].disabled = True
             self.fields['asset_tag'].disabled = True
             self.fields['part_id'].disabled = True
             self.initial['serial'] = asset.serial
             self.initial['asset_tag'] = asset.asset_tag if asset.asset_tag else None
-            self.initial['part_id'] = asset.inventoryitem_type.part_number
+            self.initial['part_id'] = asset.inventoryitem_type.part_number or asset.inventoryitem_type.model
 
             self.fields['manufacturer'].widget = StaticSelect(attrs={'readonly':True, 'disabled':True})
             self.fields['manufacturer'].choices = [(asset.inventoryitem_type.manufacturer.pk, asset.inventoryitem_type.manufacturer)]
 
     def clean(self):
         super().clean()
         component_set = None
```

### Comparing `netbox-inventory-1.2.2/netbox_inventory/forms/filters.py` & `netbox-inventory-1.2.3/netbox_inventory/forms/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/forms/models.py` & `netbox-inventory-1.2.3/netbox_inventory/forms/models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/migrations/0001_initial_prod.py` & `netbox-inventory-1.2.3/netbox_inventory/migrations/0001_initial_prod.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/migrations/0003_add_inventoryitemgroup.py` & `netbox-inventory-1.2.3/netbox_inventory/migrations/0003_add_inventoryitemgroup.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py` & `netbox-inventory-1.2.3/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/models.py` & `netbox-inventory-1.2.3/netbox_inventory/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.contrib.contenttypes.fields import GenericRelation
 from django.db import models
 from django.forms import ValidationError
 from django.urls import reverse
 
 from netbox.models import NetBoxModel, NestedGroupModel
 from .choices import HardwareKindChoices, AssetStatusChoices
-from .utils import asset_clear_old_hw, get_prechange_field, get_plugin_setting, get_status_for
+from .utils import asset_clear_old_hw, asset_set_new_hw, get_prechange_field, get_plugin_setting, get_status_for
 
 
 class Asset(NetBoxModel):
     """
     An Asset represents a piece of hardware we want to keep track of. It has a
     make (model, part number) that is one of: Device Type, Module Type or
     InventoryItem Type.
@@ -265,16 +265,16 @@
 
     def clean(self):
         self.validate_hardware_types()
         self.validate_hardware()
         self.update_status()
         return super().clean()
 
-    def save(self, *args, **kwargs):
-        self.update_hardware_used()
+    def save(self, clear_old_hw=True, *args, **kwargs):
+        self.update_hardware_used(clear_old_hw)
         return super().save(*args, **kwargs)
 
     def validate_hardware_types(self):
         """Ensure only one device/module_type/inventoryitem_type is set at a time."""
         if sum(map(bool, [self.device_type, self.module_type, self.inventoryitem_type])) > 1:
             raise ValidationError('Only one of device type, module type and inventory item type can be set for the same asset.')
         if not self.device_type and not self.module_type and not self.inventoryitem_type:
@@ -310,52 +310,37 @@
             # status has also been changed manually, don't change it automatically
             return
         if used_status and new_hw and not old_hw:
             self.status = used_status
         elif stored_status and not new_hw and old_hw:
             self.status = stored_status
 
-    def update_hardware_used(self):
+    def update_hardware_used(self, clear_old_hw=True):
         """ If assigning as device, module or inventoryitem set serial and
             asset_tag on it. Also remove them if unasigning.
         """
         if not get_plugin_setting('sync_hardware_serial_asset_tag'):
             return None
         old_hw = get_prechange_field(self, self.kind)
         new_hw = getattr(self, self.kind)
         old_serial = get_prechange_field(self, 'serial')
         old_asset_tag = get_prechange_field(self, 'asset_tag')
-        # device, module... needs None for unset asset_tag to enforce uniqness at DB level
-        new_asset_tag = self.asset_tag if self.asset_tag else None
-        # device, module... does not allow serial to be null
-        new_serial = self.serial if self.serial else ''
-        if not new_hw and old_hw:
-            # unassigned
+        if not new_hw and old_hw and clear_old_hw:
+            # unassigned existing asset, nothing asssigned now
             asset_clear_old_hw(old_hw)
         elif new_hw and old_hw != new_hw:
-            # assigned something, set its serial
-            if old_hw:
+            # assigned something new
+            if old_hw and clear_old_hw:
                 # but first clear previous hw data
                 asset_clear_old_hw(old_hw)
-            # if new_hw already has correct values, don't save it again
-            new_hw_save = False
-            if new_hw.serial != new_serial:
-                new_hw.serial = new_serial
-                new_hw_save = True
-            if new_hw.asset_tag != new_asset_tag:
-                new_hw.asset_tag = new_asset_tag
-                new_hw_save = True
-            if new_hw_save:
-                new_hw.save()
+            asset_set_new_hw(asset=self, hw=new_hw)
         elif self.serial != old_serial or self.asset_tag != old_asset_tag:
             # just changed asset's serial or asset_tag, update assigned hw
             if new_hw:
-                new_hw.serial = new_serial
-                new_hw.asset_tag = new_asset_tag
-                new_hw.save()
+                asset_set_new_hw(asset=self, hw=new_hw)
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_inventory:asset', args=[self.pk])
 
     def get_status_color(self):
         return AssetStatusChoices.colors.get(self.status)
```

### Comparing `netbox-inventory-1.2.2/netbox_inventory/navigation.py` & `netbox-inventory-1.2.3/netbox_inventory/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/search.py` & `netbox-inventory-1.2.3/netbox_inventory/search.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/signals.py` & `netbox-inventory-1.2.3/netbox_inventory/signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,9 +60,9 @@
     except Asset.DoesNotExist:
         return
     asset.snapshot()
     asset.status = stored_status
     # also unassign that item from asset
     setattr(asset, asset.kind, None)
     asset.full_clean()
-    asset.save()
+    asset.save(clear_old_hw=False)
     logger.info(f'Asset marked as stored {asset}')
```

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tables.py` & `netbox-inventory-1.2.3/netbox_inventory/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset.html` & `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html` & `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html` & `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,19 @@
                                         <td><code>asset_import_create_inventoryitem_type</code></td>
                                     </tr>
                                     <tr>
                                         <td>Supplier & Purchase</td>
                                         <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_purchase %}</td>
                                         <td><code>asset_import_create_purchase</code></td>
                                     </tr>
+                                    <tr>
+                                        <td>Owner & Tenant</td>
+                                        <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_tenant %}</td>
+                                        <td><code>asset_import_create_tenant</code></td>
+                                    </tr>
                                 </table>
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
```

#### html2text {}

```diff
@@ -12,8 +12,10 @@
 & Module Type settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_module_type %}
 Manufacturer  {% checkmark
 &             settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_inventoryitem_type asset_import_create_inventoryitem_type
 InventoryItem %}
 Type
 Supplier &    {% checkmark                                                                    asset_import_create_purchase
 Purchase      settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_purchase %}
+Owner &       {% checkmark                                                                    asset_import_create_tenant
+Tenant        settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_tenant %}
 {% endblock content %}
```

### Comparing `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html` & `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html` & `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html` & `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html` & `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,18 @@
               <th scope="row">Part number</th>
               <td>{{ object.part_number }}</td>
             </tr>
             <tr>
               <th scope="row">Group</th>
               <td>{{ object.inventoryitem_group|linkify|placeholder }}</td>
             </tr>
+            <tr>
+              <th scope="row">Assets</th>
+              <td><a href="{% url 'plugins:netbox_inventory:asset_list' %}?inventoryitem_type_id={{ object.pk }}">{{ asset_count }}</a></td>
+            </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/tags.html' %}
```

#### html2text {}

```diff
@@ -6,11 +6,12 @@
  Add_asset
  {% endif %} {% endblock extra_controls %} {% block content %}
 ** Inventory Item Type **
 Manufacturer {{ object.manufacturer|linkify }}
 Model        {{ object.model }}
 Part number  {{ object.part_number }}
 Group        {{ object.inventoryitem_group|linkify|placeholder }}
+Assets       {{_asset_count_}}
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% include 'inc/panels/image_attachments.html' %}
 {% endblock content %}
```

### Comparing `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/purchase.html` & `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/purchase.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/supplier.html` & `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/supplier.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html` & `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html` & `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html` & `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html` & `netbox-inventory-1.2.3/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tests/asset/test_api.py` & `netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tests/asset/test_models.py` & `netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tests/asset/test_views.py` & `netbox-inventory-1.2.3/netbox_inventory/tests/asset/test_views_reassign.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,187 +1,44 @@
 from django.contrib.contenttypes.models import ContentType
 from django.test import override_settings
 
 from dcim.models import Manufacturer, DeviceType, DeviceRole, Device, InventoryItem, Module, ModuleBay, ModuleType, Site
+from extras.choices import ObjectChangeActionChoices
+from extras.models import ObjectChange
 from users.models import ObjectPermission
-from utilities.testing import post_data, ViewTestCases
+from utilities.testing import ViewTestCases
+from utilities.testing.utils import post_data
 
 from netbox_inventory.tests.custom import ModelViewTestCase
 from netbox_inventory.models import Asset, InventoryItemType
-from ..settings import CONFIG_SYNC_ON, CONFIG_ALLOW_CREATE_DEVICE_TYPE
+from ..settings import CONFIG_SYNC_ON
 
 
-class AssetTestCase(
-    ModelViewTestCase,
-    ViewTestCases.PrimaryObjectViewTestCase,
-):
-
-    model = Asset
-
-    @classmethod
-    def setUpTestData(cls):
-        site1 = Site.objects.create(
-            name='site1',
-            slug='site1',
-            status='active',
-        )
-        manufacturer1 = Manufacturer.objects.create(
-            name='manufacturer1',
-            slug='manufacturer1',
-        )
-        device_type1 = DeviceType.objects.create(
-            model='device_type1',
-            slug='device_type1',
-            manufacturer=manufacturer1,
-            u_height=1,
-        )
-        device_role1 = DeviceRole.objects.create(
-            name='device_role1',
-            slug='device_role1',
-            color='9e9e9e',
-        )
-        asset1 = Asset.objects.create(
-            status='stored',
-            serial='123',
-            device_type=device_type1,
-        )
-        asset2 = Asset.objects.create(
-            status='stored',
-            serial='223',
-            device_type=device_type1,
-        )
-        asset3 = Asset.objects.create(
-            status='stored',
-            serial='323',
-            device_type=device_type1,
-        )
-
-        cls.form_data = {
-            'status': 'stored',
-            'serial': '124',
-            'device_type': device_type1.pk,
-        }
-        cls.csv_data = (
-            'serial,status,hardware_kind,manufacturer,model_name',
-            'csv1,stored,device,manufacturer1,device_type1',
-            'csv2,stored,device,manufacturer1,device_type1',
-            'csv3,stored,device,manufacturer_csv,device_type_csv',
-        )
-        cls.csv_update_data = (
-            'id,serial,status',
-            f'{asset1.pk},133,stored',
-            f'{asset2.pk},233,stored',
-            f'{asset3.pk},333,stored',
-        )
-        cls.bulk_edit_data = {
-            'status': 'retired',
-        }
-
-    @override_settings(EXEMPT_VIEW_PERMISSIONS=['*'])
-    def test_assign_device_from_asset(self):
-
-        # Assign unconstrained permission
-        obj_perm = ObjectPermission(
-            name='test-device-assign permission',
-            actions=['add', 'change']
-        )
-        obj_perm.save()
-        obj_perm.users.add(self.user)
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
-        obj_perm.object_types.add(ContentType.objects.get_for_model(Device))
-
-        asset = Asset.objects.create(
-            status='stored',
-            serial='123assign',
-            device_type=DeviceType.objects.first(),
-        )
-        device = Device.objects.create(
-            name='test-device-assign',
-            device_role = DeviceRole.objects.first(),
-            device_type=asset.device_type,
-            site = Site.objects.first(),
-            status = 'active',
-        )
-
-        form_data = {
-            'name': 'test-device-assign',
-            'device_type': asset.device_type.pk,
-            'device': device.pk,
-        }
-
-        request = {
-            'path': self._get_url('assign', asset),
-            'data': post_data(form_data),
-        }
-        self.assertHttpStatus(self.client.post(**request), 302)
-
-        devices = Device.objects.filter(name=device.name)
-        self.assertEqual(len(devices), 1)
-        self.assertEqual(devices.first().assigned_asset, asset)
-
-    @override_settings(PLUGINS_CONFIG=CONFIG_ALLOW_CREATE_DEVICE_TYPE)
-    def test_bulk_import_objects_with_permission(self):
-        return super().test_bulk_import_objects_with_permission()
-
-    @override_settings(PLUGINS_CONFIG=CONFIG_ALLOW_CREATE_DEVICE_TYPE)
-    def test_bulk_import_objects_with_constrained_permission(self):
-        return super().test_bulk_import_objects_with_constrained_permission()
-
-
-class AssetBulkAddTestCase(
-    ModelViewTestCase,
-    ViewTestCases.CreateMultipleObjectsViewTestCase,
-):
+class AssetReassignBase():
     """
-    test for /plugins/inventory/assets/bulk-add/
-    """
-    model = Asset
-
-    @classmethod
-    def setUpTestData(cls):
-        manufacturer1 = Manufacturer.objects.create(
-            name='manufacturer1',
-            slug='manufacturer1',
-        )
-        device_type1 = DeviceType.objects.create(
-            model='device_type1',
-            slug='device_type1',
-            manufacturer=manufacturer1,
-            u_height=1,
-        )
-
-        cls.bulk_create_data = {
-            'count': 3,
-            'status': 'stored',
-            'device_type': device_type1.pk,
-        }
-
-    def _get_url(self, action, instance=None):
-        # fix - CreateMultipleObjectsViewTestCase assumes view names contains only 'add' but we need 'bulk_add'
-        if action == 'add':
-            action = 'bulk_add'
-        return super()._get_url(action, instance)
-
-class AssetCreateHwBase():
-    """
-    Base class for tests that create hardware and assign Asset to it
+    Base class for tests that reassign another asset to hardware
     """
 
+    @override_settings(PLUGINS_CONFIG=CONFIG_SYNC_ON)
     def setUp(self):
         super().setUp()
 
         self.site1 = Site.objects.create(
             name='site1',
             slug='site1',
             status='active',
         )
         self.manufacturer1 = Manufacturer.objects.create(
             name='manufacturer1',
             slug='manufacturer1',
         )
+        self.manufacturer2 = Manufacturer.objects.create(
+            name='manufacturer2',
+            slug='manufacturer2',
+        )
         self.device_type1 = DeviceType.objects.create(
             manufacturer=self.manufacturer1,
             model='device_type1',
             slug='device_type1'
         )
         self.module_type1 = ModuleType.objects.create(
             manufacturer=self.manufacturer1,
@@ -192,182 +49,260 @@
             slug='device_role1'
         )
         self.inventoryitem_type1 = InventoryItemType.objects.create(
             manufacturer=self.manufacturer1,
             model='inventoryitem_type1',
             slug='inventoryitem_type1'
         )
+        self.inventoryitem_type2 = InventoryItemType.objects.create(
+            manufacturer=self.manufacturer1,
+            model='inventoryitem_type2',
+            slug='inventoryitem_type2'
+        )
         self.device1 = Device.objects.create(
             site=self.site1,
             status='active',
             device_type=self.device_type1,
             device_role=self.device_role1,
             name='device1',
         )
         self.module_bay1 = ModuleBay.objects.create(
             device=self.device1,
             name='1',
         )
-        self.asset_device_sn = Asset.objects.create(
+        self.module1 = Module.objects.create(
+            module_bay=self.module_bay1,
+            device=self.device1,
+            module_type=self.module_type1,
+        )
+        self.inventoryitem1 = InventoryItem.objects.create(
+            device=self.device1,
+            name='inventoryitem1',
+        )
+        self.asset_device_old = Asset.objects.create(
             asset_tag='asset_device',
             serial='asset_device',
-            status='stored',
+            status='used',
             device_type=self.device_type1,
+            device=self.device1,
         )
-        self.asset_module_sn = Asset.objects.create(
+        self.asset_module_old = Asset.objects.create(
             asset_tag='asset_module',
             serial='asset_module',
-            status='stored',
+            status='used',
             module_type=self.module_type1,
+            module=self.module1,
         )
-        self.asset_inventoryitem_sn = Asset.objects.create(
+        self.asset_inventoryitem_old = Asset.objects.create(
             asset_tag='asset_inventoryitem',
             serial='asset_inventoryitem',
-            status='stored',
+            status='used',
             inventoryitem_type=self.inventoryitem_type1,
+            inventoryitem=self.inventoryitem1,
         )
-        self.asset_device_no = Asset.objects.create(
+        self.asset_device_new = Asset.objects.create(
+            asset_tag='asset_device2',
+            serial='asset_device2',
             status='stored',
             device_type=self.device_type1,
         )
-        self.asset_module_no = Asset.objects.create(
+        self.asset_module_new = Asset.objects.create(
+            asset_tag='asset_module2',
+            serial='asset_module2',
             status='stored',
             module_type=self.module_type1,
         )
-        self.asset_inventoryitem_no = Asset.objects.create(
+        self.asset_inventoryitem_new = Asset.objects.create(
+            asset_tag='asset_inventoryitem2',
+            serial='asset_inventoryitem2',
             status='stored',
-            inventoryitem_type=self.inventoryitem_type1,
+            inventoryitem_type=self.inventoryitem_type2,
         )
 
-    def _get_url(self, _):
-        hardware_kind = self.tested_asset.kind
-        if hardware_kind == 'inventoryitem':
-            hardware_kind = 'inventory-item'
-        return f'/plugins/inventory/assets/{hardware_kind}/create/?asset_id={self.tested_asset.pk}'
+    def _get_url(self, _, instance):
+        hardware_kind = self.model._meta.model_name
+        return f'/plugins/inventory/assets/{hardware_kind}/{self.tested_hardware.pk}/reassign/'
 
     @override_settings(EXEMPT_VIEW_PERMISSIONS=['*'])
     @override_settings(PLUGINS_CONFIG=CONFIG_SYNC_ON)
-    def test_create_object_with_permission(self):
-        super().test_create_object_with_permission()
-        # in addition to a new inventoryitem instance in db,
-        # it must have matching serial and asset2 must have it assigned
-        # blank value for Asset.serial is None, but for Device/Module/IItem.serial it's ''
-        checked_serial = self.tested_asset.serial or '' 
-        instance = self._get_queryset().order_by('pk').last()
-        self.assertEqual(instance.asset_tag, self.tested_asset.asset_tag)
-        self.assertEqual(instance.serial, checked_serial)
-        self.tested_asset.refresh_from_db()
-        self.assertEqual(instance, self.tested_asset.hardware)
+    def test_edit_object_with_permission(self):
+        # copy & pasted from super() and modified
+        instance = self._get_queryset().first()
 
-    @override_settings(EXEMPT_VIEW_PERMISSIONS=['*'])
-    @override_settings(PLUGINS_CONFIG=CONFIG_SYNC_ON)
-    def test_create_object_with_constrained_permission(self):
-        super().test_create_object_with_constrained_permission()
-        # in addition to a new inventoryitem instance in db,
-        # it must have matching serial and asset2 must have it assigned
-        # blank value for Asset.serial is None, but for Device/Module/IItem.serial it's ''
-        checked_serial = self.tested_asset.serial or '' 
-        instance = self._get_queryset().order_by('pk').last()
-        self.assertEqual(instance.asset_tag, self.tested_asset.asset_tag)
-        self.assertEqual(instance.serial, checked_serial)
-        self.tested_asset.refresh_from_db()
-        self.assertEqual(instance, self.tested_asset.hardware)
+        # Assign model-level permission
+        obj_perm = ObjectPermission(
+            name='Test permission',
+            actions=['change']
+        )
+        obj_perm.save()
+        obj_perm.users.add(self.user)
+        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
 
+        # Try GET with model-level permission
+        self.assertHttpStatus(self.client.get(self._get_url('edit', instance)), 200)
 
-class SerialDeviceAssetCreateHwTestCase(AssetCreateHwBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
+        # Try POST with model-level permission
+        request = {
+            'path': self._get_url('edit', instance),
+            'data': post_data(self.form_data),
+        }
+        self.assertHttpStatus(self.client.post(**request), 302)
+        # cannot use assertInstanceEqual, use custom asserts
+        ##self.assertInstanceEqual(self._get_queryset().get(pk=instance.pk), self.form_data)
+        updated = self._get_queryset().get(pk=instance.pk)
+        if self.asset_new:
+            self.assertEqual(updated.asset_tag, self.asset_new.asset_tag)
+            self.assertEqual(updated.serial, self.asset_new.serial)
+        else:
+            self.assertEqual(updated.asset_tag, None)
+            self.assertEqual(updated.serial, '')
+
+        # Verify ObjectChange creation
+        objectchanges = ObjectChange.objects.filter(
+            changed_object_type=ContentType.objects.get_for_model(instance),
+            changed_object_id=instance.pk
+        )
+        self.assertEqual(len(objectchanges), 1)
+        self.assertEqual(objectchanges[0].action, ObjectChangeActionChoices.ACTION_UPDATE)
+
+        # check for changes on asset instances
+        self.asset_old.refresh_from_db()
+        self.assertEqual(self.asset_old.status, 'stored')
+        self.assertEqual(self.asset_old.hardware, None)
+        objectchanges = ObjectChange.objects.filter(
+            changed_object_type=ContentType.objects.get_for_model(self.asset_old),
+            changed_object_id=self.asset_old.pk
+        )
+        self.assertEqual(len(objectchanges), 1)
+        self.assertEqual(objectchanges[0].action, ObjectChangeActionChoices.ACTION_UPDATE)
+        if self.asset_new:
+            self.asset_new.refresh_from_db()
+            self.assertEqual(self.asset_new.status, 'used')
+            self.assertEqual(self.asset_new.hardware, updated)
+            objectchanges = ObjectChange.objects.filter(
+                changed_object_type=ContentType.objects.get_for_model(self.asset_new),
+                changed_object_id=self.asset_new.pk
+            )
+            self.assertEqual(len(objectchanges), 1)
+            self.assertEqual(objectchanges[0].action, ObjectChangeActionChoices.ACTION_UPDATE)
+
+
+class DeviceReassignAssetTestCase(AssetReassignBase, ModelViewTestCase):
     """
-    Test creating new Device from Asset with serial
+    Test assigning different Asset to Device
     """
     model = Device
 
     def setUp(self):
         super().setUp()
         self.form_data = {
-            'site': self.site1.pk,
-            'device_type': self.device_type1.pk,
-            'device_role': self.device_role1.pk,
-            'status': 'active',
-            'name': 'tested_device',
+            'device_type': self.device1.device_type.pk,
+            'assigned_asset': self.asset_device_new.pk,
+            'asset_status': 'stored',
         }
-        self.tested_asset = self.asset_device_sn
+        self.tested_hardware = self.device1
+        self.asset_new = self.asset_device_new
+        self.asset_old = self.asset_device_old
 
 
-class SerialModuleAssetCreateHwTestCase(AssetCreateHwBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
+class ModuleReassignAssetTestCase(AssetReassignBase, ModelViewTestCase):
     """
-    Test creating new Module from Asset with serial
+    Test assigning different Asset to Module
     """
     model = Module
 
     def setUp(self):
         super().setUp()
         self.form_data = {
-            'device': self.device1.pk,
-            'module_bay': self.module_bay1.pk,
-            'module_type': self.module_type1.pk,
-            'status': 'active',
+            'module_type': self.module1.module_type.pk,
+            'assigned_asset': self.asset_module_new.pk,
+            'asset_status': 'stored',
         }
-        self.tested_asset = self.asset_module_sn
+        self.tested_hardware = self.module1
+        self.asset_new = self.asset_module_new
+        self.asset_old = self.asset_module_old
 
 
-class SerialInventoryItemAssetCreateHwTestCase(AssetCreateHwBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
+class InventoryItemReassignAssetTestCase(AssetReassignBase, ModelViewTestCase):
     """
-    Test creating new InventoryItem from Asset with serial
+    Test assigning different Asset to InventoryItem
     """
     model = InventoryItem
 
     def setUp(self):
         super().setUp()
         self.form_data = {
-            'device': self.device1.pk,
-            'name': 'inventoryitem1',
+            'assigned_asset': self.asset_inventoryitem_new.pk,
+            'asset_status': 'stored',
         }
-        self.tested_asset = self.asset_inventoryitem_sn
+        self.tested_hardware = self.inventoryitem1
+        self.asset_new = self.asset_inventoryitem_new
+        self.asset_old = self.asset_inventoryitem_old
+
+    @override_settings(EXEMPT_VIEW_PERMISSIONS=['*'])
+    @override_settings(PLUGINS_CONFIG=CONFIG_SYNC_ON)
+    def test_edit_object_with_permission(self):
+        super().test_edit_object_with_permission()
+        # also check if inventory item manufacturer and part_id was set
+        self.tested_hardware.refresh_from_db()
+        self.asset_new.refresh_from_db()
+        self.assertEqual(self.tested_hardware.manufacturer, self.asset_new.inventoryitem_type.manufacturer)
+        self.assertEqual(self.tested_hardware.part_id, self.asset_new.inventoryitem_type.model)
 
 
-class NoSerialDeviceAssetCreateHwTestCase(AssetCreateHwBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
+class DeviceUnassignAssetTestCase(AssetReassignBase, ModelViewTestCase):
     """
-    Test creating new Device from Asset with blank serial
+    Test assigning no Asset to Device
     """
     model = Device
 
     def setUp(self):
         super().setUp()
         self.form_data = {
-            'site': self.site1.pk,
-            'device_type': self.device_type1.pk,
-            'device_role': self.device_role1.pk,
-            'status': 'active',
-            'name': 'tested_device',
+            'device_type': self.device1.device_type.pk,
+            'asset_status': 'stored',
         }
-        self.tested_asset = self.asset_device_no
+        self.tested_hardware = self.device1
+        self.asset_new = None
+        self.asset_old = self.asset_device_old
 
 
-class NoSerialModuleAssetCreateHwTestCase(AssetCreateHwBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
+class ModuleUnassignAssetTestCase(AssetReassignBase, ModelViewTestCase):
     """
-    Test creating new Module from Asset with blank serial
+    Test assigning no Asset to Module
     """
     model = Module
 
     def setUp(self):
         super().setUp()
         self.form_data = {
-            'device': self.device1.pk,
-            'module_bay': self.module_bay1.pk,
-            'module_type': self.module_type1.pk,
-            'status': 'active',
+            'module_type': self.module1.module_type.pk,
+            'asset_status': 'stored',
         }
-        self.tested_asset = self.asset_module_no
+        self.tested_hardware = self.module1
+        self.asset_new = None
+        self.asset_old = self.asset_module_old
 
 
-class NoSerialInventoryItemAssetCreateHwTestCase(AssetCreateHwBase, ModelViewTestCase, ViewTestCases.CreateObjectViewTestCase):
+class InventoryItemUnassignAssetTestCase(AssetReassignBase, ModelViewTestCase):
     """
-    Test creating new InventoryItem from Asset with blank serial
+    Test assigning no Asset to InventoryItem
     """
     model = InventoryItem
 
     def setUp(self):
         super().setUp()
         self.form_data = {
-            'device': self.device1.pk,
-            'name': 'inventoryitem1',
+            'asset_status': 'stored',
         }
-        self.tested_asset = self.asset_inventoryitem_no
+        self.tested_hardware = self.inventoryitem1
+        self.asset_new = None
+        self.asset_old = self.asset_inventoryitem_old
+
+    @override_settings(EXEMPT_VIEW_PERMISSIONS=['*'])
+    @override_settings(PLUGINS_CONFIG=CONFIG_SYNC_ON)
+    def test_edit_object_with_permission(self):
+        super().test_edit_object_with_permission()
+        # also check if inventory item manufacturer and part_id was kept
+        self.tested_hardware.refresh_from_db()
+        self.assertEqual(self.tested_hardware.manufacturer, self.asset_old.inventoryitem_type.manufacturer)
+        self.assertEqual(self.tested_hardware.part_id, self.asset_old.inventoryitem_type.model)
```

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tests/custom.py` & `netbox-inventory-1.2.3/netbox_inventory/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_group/test_api.py` & `netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_group/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_group/test_views.py` & `netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_group/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_type/test_api.py` & `netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_type/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tests/inventoryitem_type/test_views.py` & `netbox-inventory-1.2.3/netbox_inventory/tests/inventoryitem_type/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tests/purchase/test_api.py` & `netbox-inventory-1.2.3/netbox_inventory/tests/purchase/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tests/purchase/test_views.py` & `netbox-inventory-1.2.3/netbox_inventory/tests/purchase/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tests/settings.py` & `netbox-inventory-1.2.3/netbox_inventory/tests/settings.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tests/supplier/test_api.py` & `netbox-inventory-1.2.3/netbox_inventory/tests/supplier/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tests/supplier/test_views.py` & `netbox-inventory-1.2.3/netbox_inventory/tests/supplier/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/tests/test_load.py` & `netbox-inventory-1.2.3/netbox_inventory/tests/test_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class NetboxDnsVersionTestCase(SimpleTestCase):
     """
     Test for netbox_inventory package
     """
 
     def test_version(self):
-        assert __version__ == "1.2.2"
+        assert __version__ == "1.2.3"
 
 
 class AppTest(APITestCase):
     """
     Test the availability of the plugin API root
     """
```

### Comparing `netbox-inventory-1.2.2/netbox_inventory/urls.py` & `netbox-inventory-1.2.3/netbox_inventory/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     path('assets/<int:pk>/delete/', views.AssetDeleteView.as_view(), name='asset_delete'),
     path('assets/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='asset_changelog', kwargs={'model': models.Asset}),
     path('assets/<int:pk>/journal/', ObjectJournalView.as_view(), name='asset_journal', kwargs={'model': models.Asset}),
     path('assets/<int:pk>/assign/', views.AssetAssignView.as_view(), name='asset_assign'),
     path('assets/device/create/', views.AssetDeviceCreateView.as_view(), name='asset_device_create'),
     path('assets/module/create/', views.AssetModuleCreateView.as_view(), name='asset_module_create'),
     path('assets/inventory-item/create/', views.AssetInventoryItemCreateView.as_view(), name='asset_inventoryitem_create'),
+    path('assets/device/<int:pk>/reassign/', views.AssetDeviceReassignView.as_view(), name='asset_device_reassign'),
+    path('assets/module/<int:pk>/reassign/', views.AssetModuleReassignView.as_view(), name='asset_module_reassign'),
+    path('assets/inventoryitem/<int:pk>/reassign/', views.AssetInventoryItemReassignView.as_view(), name='asset_inventoryitem_reassign'),
 
     # Suppliers
     path('suppliers/', views.SupplierListView.as_view(), name='supplier_list'),
     path('suppliers/add/', views.SupplierEditView.as_view(), name='supplier_add'),
     path('suppliers/import/', views.SupplierBulkImportView.as_view(), name='supplier_import'),
     path('suppliers/edit/', views.SupplierBulkEditView.as_view(), name='supplier_bulk_edit'),
     path('suppliers/delete/', views.SupplierBulkDeleteView.as_view(), name='supplier_bulk_delete'),
```

### Comparing `netbox-inventory-1.2.2/netbox_inventory/utils.py` & `netbox-inventory-1.2.3/netbox_inventory/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -99,14 +99,44 @@
     old_hw.asset_tag = None
     old_hw.save()
     pre_save.connect(prevent_update_serial_asset_tag, sender=Device)
     pre_save.connect(prevent_update_serial_asset_tag, sender=Module)
     pre_save.connect(prevent_update_serial_asset_tag, sender=InventoryItem)
 
 
+def asset_set_new_hw(asset, hw):
+    """
+    Asset was assigned to hardware (device/module/inventory item) and we want to
+    sync some field values from asset to hardware
+    Validation if asset can be assigned to hw should be done before calling this function.
+    """
+    # device, module... needs None for blank asset_tag to enforce uniqness at DB level
+    new_asset_tag = asset.asset_tag or None
+    # device, module... does not allow serial to be null
+    new_serial = asset.serial or ''
+    hw_save = False
+    if hw.serial != new_serial:
+        hw.serial = new_serial
+        hw_save = True
+    if hw.asset_tag != new_asset_tag:
+        hw.asset_tag = new_asset_tag
+        hw_save = True
+    # for inventory items also set manufacturer and part_number
+    if asset.inventoryitem_type:
+        if hw.manufacturer != asset.inventoryitem_type.manufacturer:
+            hw.manufacturer = asset.inventoryitem_type.manufacturer
+            hw_save = True
+        part_id = asset.inventoryitem_type.part_number or asset.inventoryitem_type.model
+        if hw.part_id != part_id:
+            hw.part_id = part_id
+            hw_save = True
+    if hw_save:
+        hw.save()
+
+
 def is_equal_none(a, b):
     """ Compare a and b as string. None is considered the same as empty string. """
     if a is None or b is None:
         return a == b or a == '' or b == ''
     return a == b
```

### Comparing `netbox-inventory-1.2.2/netbox_inventory/views/asset.py` & `netbox-inventory-1.2.3/netbox_inventory/views/asset.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/views/asset_assign.py` & `netbox-inventory-1.2.3/netbox_inventory/views/asset_assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/views/asset_create.py` & `netbox-inventory-1.2.3/netbox_inventory/views/asset_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/views/inventoryitem_group.py` & `netbox-inventory-1.2.3/netbox_inventory/views/inventoryitem_group.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/views/inventoryitem_type.py` & `netbox-inventory-1.2.3/netbox_inventory/views/inventoryitem_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,19 @@
     'InventoryItemTypeBulkEditView',
     'InventoryItemTypeBulkDeleteView',
 )
 
 class InventoryItemTypeView(generic.ObjectView):
     queryset = models.InventoryItemType.objects.all()
 
+    def get_extra_context(self, request, instance):
+        context = super().get_extra_context(request, instance)
+        context['asset_count'] = models.Asset.objects.restrict(request.user, 'view').filter(inventoryitem_type=instance).count()
+        return context
+
 
 class InventoryItemTypeListView(generic.ObjectListView):
     queryset = models.InventoryItemType.objects.annotate(
         asset_count=count_related(models.Asset, 'inventoryitem_type'),
     )
     table = tables.InventoryItemTypeTable
     filterset = filtersets.InventoryItemTypeFilterSet
```

### Comparing `netbox-inventory-1.2.2/netbox_inventory/views/purchase.py` & `netbox-inventory-1.2.3/netbox_inventory/views/purchase.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/views/supplier.py` & `netbox-inventory-1.2.3/netbox_inventory/views/supplier.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory/views/tabs.py` & `netbox-inventory-1.2.3/netbox_inventory/views/tabs.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.2/netbox_inventory.egg-info/PKG-INFO` & `netbox-inventory-1.2.3/netbox_inventory.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.2.2
+Version: 1.2.3
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,26 +20,36 @@
 ## Features
 
 Keep track of your hardware, whether it is installed or in storage. You can
 define assets that represent hardware that can be used as a device, module or
 inventory item in NetBox.
 
 Each asset can have a storage location defined, when not in use. You can assign
-an asset to a device or module. The plugin can keep serial number and asset tag
-between asset and device or module in sync if enabled in settings.
+an asset to a device, module or inventory item. The plugin can keep serial number
+and asset tag between asset and device, module or inventory item in sync if
+enabled in settings.
+
+On Site and Location detail views there is a new tab Assets that can show assets
+that are stored or installed at that location or both. Rack details view also has
+a tab for installed Assets. This provides a unified view of all assets at a given
+location.
 
 To properly support inventory items (that are used in NetBox to model SFP and
 similar modules) the plugin defines inventory item types that are equivalent to
 device types and module types. 
 
 Inventory item types can be assigned into inventory item groups. On a group detail
 view you have an overview of the number of contained assets broken down by asset
 status or inventory item type and status. This way you can quickly see how many
 of a certain type of hardware you still have spare.
 
+Inventory item groups can be nested, so you can for example model all pluggables
+as one top-level group with child groups for SFP+ modules, SFP28 modules and so
+on.
+
 ### Automatic management of asset status
 
 Each asset has a status attribute that can indicate use of the asset. These
 statuses can be set as needed by each NetBox installation.
 
 Two statuses can have a special meaning. One to indicate asset is in storage and one
 to indicate asset is in use.
@@ -151,14 +161,15 @@
 | `used_status_name` | `'used'`| Status that indicates asset is in use. See "Automatic management of asset status" below for more info on this setting.
 | `stored_status_name` | `'stored'`| Status that indicates asset is in storage. See "Automatic management of asset status" below for more info on this setting.
 | `sync_hardware_serial_asset_tag` | `False` | When an asset is assigned or unassigned to a device, module or inventory item, update its serial number and asset tag to be in sync with the asset? |
 | `asset_import_create_purchase` | `False` | When importing assets, automatically create purchase (and supplier) if it doesn't exist |
 | `asset_import_create_device_type` | `False` | When importing a device type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_module_type` | `False` | When importing a module type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_inventoryitem_type` | `False` | When importing an inventory type asset, automatically create manufacturer and/or device type if it doesn't exist |
+| `asset_import_create_tenant` | `False` | When importing an asset, with owner or tenant, automatically create tenant if it doesn't exist |
 | `asset_disable_editing_fields_for_tags` | `{}` | A dictionary of tags and fields that should be disabled for editing. This is useful if you want to prevent editing of certain fields for certain assets. The dictionary is in the form of `{tag: [field1, field2]}`. Example: `{'no-edit': ['serial_number', 'asset_tag']}`. This only affects the UI, the API can still be used to edit the fields. |
 | `asset_disable_deletion_for_tags` | `[]` | List of tags that will disable deletion of assets. This only affects the UI, not the API. |
 
 You can extend or define your own status choices for Asset, via [`FIELD_CHOICES`](https://docs.netbox.dev/en/stable/configuration/data-validation/#field_choices) setting in Netbox:
 
 ```
 FIELD_CHOICES = {
```

### Comparing `netbox-inventory-1.2.2/netbox_inventory.egg-info/SOURCES.txt` & `netbox-inventory-1.2.3/netbox_inventory.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,44 +27,50 @@
 netbox_inventory/forms/__init__.py
 netbox_inventory/forms/assign.py
 netbox_inventory/forms/bulk.py
 netbox_inventory/forms/bulk_add.py
 netbox_inventory/forms/create.py
 netbox_inventory/forms/filters.py
 netbox_inventory/forms/models.py
+netbox_inventory/forms/reassign.py
 netbox_inventory/migrations/0001_initial_prod.py
 netbox_inventory/migrations/0002_alter_asset_serial.py
 netbox_inventory/migrations/0003_add_inventoryitemgroup.py
 netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
 netbox_inventory/migrations/__init__.py
 netbox_inventory/templates/netbox_inventory/asset.html
 netbox_inventory/templates/netbox_inventory/asset_assign.html
 netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
 netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
 netbox_inventory/templates/netbox_inventory/asset_create.html
 netbox_inventory/templates/netbox_inventory/asset_edit.html
+netbox_inventory/templates/netbox_inventory/asset_reassign.html
 netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
 netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
 netbox_inventory/templates/netbox_inventory/purchase.html
 netbox_inventory/templates/netbox_inventory/supplier.html
 netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
 netbox_inventory/templates/netbox_inventory/inc/asset_info.html
+netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
+netbox_inventory/templates/netbox_inventory/inc/asset_tenant.html
 netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
 netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
 netbox_inventory/tests/__init__.py
 netbox_inventory/tests/custom.py
 netbox_inventory/tests/settings.py
 netbox_inventory/tests/test_load.py
 netbox_inventory/tests/asset/__init__.py
 netbox_inventory/tests/asset/test_api.py
 netbox_inventory/tests/asset/test_models.py
 netbox_inventory/tests/asset/test_views.py
+netbox_inventory/tests/asset/test_views_create.py
+netbox_inventory/tests/asset/test_views_reassign.py
 netbox_inventory/tests/inventoryitem_group/__init__.py
 netbox_inventory/tests/inventoryitem_group/test_api.py
 netbox_inventory/tests/inventoryitem_group/test_views.py
 netbox_inventory/tests/inventoryitem_type/__init__.py
 netbox_inventory/tests/inventoryitem_type/test_api.py
 netbox_inventory/tests/inventoryitem_type/test_views.py
 netbox_inventory/tests/purchase/__init__.py
@@ -73,12 +79,13 @@
 netbox_inventory/tests/supplier/__init__.py
 netbox_inventory/tests/supplier/test_api.py
 netbox_inventory/tests/supplier/test_views.py
 netbox_inventory/views/__init__.py
 netbox_inventory/views/asset.py
 netbox_inventory/views/asset_assign.py
 netbox_inventory/views/asset_create.py
+netbox_inventory/views/asset_reassign.py
 netbox_inventory/views/inventoryitem_group.py
 netbox_inventory/views/inventoryitem_type.py
 netbox_inventory/views/purchase.py
 netbox_inventory/views/supplier.py
 netbox_inventory/views/tabs.py
```

### Comparing `netbox-inventory-1.2.2/pyproject.toml` & `netbox-inventory-1.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-inventory"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="Matej Vadnjal", email="matej.vadnjal@arnes.si" },
 ]
 description = "Inventory asset management in NetBox"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

