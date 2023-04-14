# Comparing `tmp/alibabacloud_dingtalk-1.5.63.tar.gz` & `tmp/alibabacloud_dingtalk-1.5.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-1.5.63.tar", last modified: Tue Apr 11 09:50:13 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-1.5.64.tar", last modified: Fri Apr 14 01:59:04 2023, max compression
```

## Comparing `alibabacloud_dingtalk-1.5.63.tar` & `alibabacloud_dingtalk-1.5.64.tar`

### file list

```diff
@@ -1,345 +1,345 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/
--rw-r--r--   0 root         (0) root         (0)    18974 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8708 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22962 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51882 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   179168 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21344 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44730 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18586 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22436 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81490 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   140148 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   134106 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   288074 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40908 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    63666 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   177626 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   583083 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4180 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3576 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   130914 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   326360 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24154 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41993 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31362 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   106693 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    61834 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   121561 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56162 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    82298 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51372 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   127231 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260294 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   382552 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18716 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44885 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5814 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10402 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15642 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32114 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   194896 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   555654 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4048 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7207 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29122 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    47050 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   340246 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503096 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    99276 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   149418 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50064 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    53792 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40488 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    66172 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   196916 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   261579 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   134506 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   276268 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   127432 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   192831 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   401586 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   699718 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62504 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110186 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75706 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   118345 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4334 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6225 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   273442 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   424209 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140236 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   310177 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4520 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5052 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9290 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9446 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69681 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   140857 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14767 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18751 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4620 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4336 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79106 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   133812 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   268744 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   381405 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12612 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    19194 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76078 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83510 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   454060 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   731352 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54446 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   160887 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54782 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   111368 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77806 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   129784 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14978 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    24607 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   117228 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   154147 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45940 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    51039 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26123 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    39828 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7690 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6891 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67864 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137575 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68812 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   125156 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48952 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    57536 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   233262 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   399779 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16002 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9973 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4606 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4435 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   118728 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   171405 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71838 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    91606 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50744 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    82767 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35104 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    47649 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   322628 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   499096 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28634 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25101 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40406 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105120 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   173162 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   389740 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9158 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31448 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12420 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30097 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60784 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   156671 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12502 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16057 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12410 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21548 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12290 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17800 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16936 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33576 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68340 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110827 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3452 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3124 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7006 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20769 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4608 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8329 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24540 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28057 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   154430 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   385214 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4012 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3485 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   416280 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   690137 2023-04-11 09:50:12.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11356 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2585 2023-04-11 09:50:13.000000 alibabacloud_dingtalk-1.5.63/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/
+-rw-r--r--   0 root         (0) root         (0)    19039 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8708 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22962 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51882 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   179168 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21344 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44730 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18586 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22436 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81490 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   140148 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   134106 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   288074 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40908 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    63666 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   177626 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   583083 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3576 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   131164 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   326662 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24154 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41993 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31362 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   106693 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    61834 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   121561 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56162 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    82298 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51372 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   127231 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260294 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   382552 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18716 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44885 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5814 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10402 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15642 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32114 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   194896 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   555654 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4048 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7207 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29122 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    47050 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   340246 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503096 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99276 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   149418 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50064 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    53792 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40488 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    66172 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   196916 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   261579 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   134506 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   276268 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   127432 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   192831 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   401586 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   699718 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62504 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110186 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75706 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   118345 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4334 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6225 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   273442 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   424209 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140236 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   310177 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4520 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5052 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9290 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9446 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69681 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   140857 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14767 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18751 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4336 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79392 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   134254 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   268744 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   381405 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12612 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    19194 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76078 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83510 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   454060 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   731352 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54446 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   160887 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54782 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   111368 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77806 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   129784 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14978 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    24607 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   117228 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   154147 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45940 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    51039 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26123 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    39828 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7690 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6891 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    67864 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137575 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68812 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   125156 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48952 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    57536 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   233262 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   399779 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16002 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9973 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4606 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   118728 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   171405 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71838 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    91606 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50744 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    82767 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35104 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    47649 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   322628 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   499096 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28634 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25101 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40406 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105120 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   173162 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   389740 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9158 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31448 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12420 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30097 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60784 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   156671 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12502 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16057 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12410 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21548 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12290 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17800 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16936 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33576 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68340 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110827 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3124 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7006 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20769 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4608 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8329 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24540 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28057 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   154430 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   385214 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4012 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3485 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   416280 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   688786 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11356 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/setup.py
```

### Comparing `alibabacloud_dingtalk-1.5.63/ChangeLog.md` & `alibabacloud_dingtalk-1.5.64/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-04-11 Version: 1.5.63
+- Update AddOfficialAccountFollower.
+
 2023-04-07 Version: 1.5.62
 - Update AddOfficialAccountFollower.
 
 2023-04-04 Version: 1.5.61
 - Update AddOfficialAccountFollower.
 
 2023-03-27 Version: 1.5.59
```

### Comparing `alibabacloud_dingtalk-1.5.63/LICENSE` & `alibabacloud_dingtalk-1.5.64/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/PKG-INFO` & `alibabacloud_dingtalk-1.5.64/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 1.5.63
+Version: 1.5.64
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-1.5.63/README-CN.md` & `alibabacloud_dingtalk-1.5.64/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/README.md` & `alibabacloud_dingtalk-1.5.64/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1597,14 +1597,16 @@
         query = {}
         if not UtilClient.is_unset(request.max_attendees):
             query['maxAttendees'] = request.max_attendees
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.series_master_id):
+            query['seriesMasterId'] = request.series_master_id
         if not UtilClient.is_unset(request.show_deleted):
             query['showDeleted'] = request.show_deleted
         if not UtilClient.is_unset(request.sync_token):
             query['syncToken'] = request.sync_token
         if not UtilClient.is_unset(request.time_max):
             query['timeMax'] = request.time_max
         if not UtilClient.is_unset(request.time_min):
@@ -1637,14 +1639,16 @@
         query = {}
         if not UtilClient.is_unset(request.max_attendees):
             query['maxAttendees'] = request.max_attendees
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.series_master_id):
+            query['seriesMasterId'] = request.series_master_id
         if not UtilClient.is_unset(request.show_deleted):
             query['showDeleted'] = request.show_deleted
         if not UtilClient.is_unset(request.sync_token):
             query['syncToken'] = request.sync_token
         if not UtilClient.is_unset(request.time_max):
             query['timeMax'] = request.time_max
         if not UtilClient.is_unset(request.time_min):
```

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5146,25 +5146,27 @@
 
 class ListEventsRequest(TeaModel):
     def __init__(
         self,
         max_attendees: int = None,
         max_results: int = None,
         next_token: str = None,
+        series_master_id: str = None,
         show_deleted: bool = None,
         sync_token: str = None,
         time_max: str = None,
         time_min: str = None,
     ):
         # 每个日程的参与者查询个数，默认100，最大100
         self.max_attendees = max_attendees
         # 返回的最大日程数，最大100个，默认100个
         self.max_results = max_results
         # 查询翻页token
         self.next_token = next_token
+        self.series_master_id = series_master_id
         # 是否返回删除事件
         self.show_deleted = show_deleted
         # 增量查询token
         self.sync_token = sync_token
         # 查询截止时间
         self.time_max = time_max
         # 查询开始时间
@@ -5181,14 +5183,16 @@
         result = dict()
         if self.max_attendees is not None:
             result['maxAttendees'] = self.max_attendees
         if self.max_results is not None:
             result['maxResults'] = self.max_results
         if self.next_token is not None:
             result['nextToken'] = self.next_token
+        if self.series_master_id is not None:
+            result['seriesMasterId'] = self.series_master_id
         if self.show_deleted is not None:
             result['showDeleted'] = self.show_deleted
         if self.sync_token is not None:
             result['syncToken'] = self.sync_token
         if self.time_max is not None:
             result['timeMax'] = self.time_max
         if self.time_min is not None:
@@ -5199,14 +5203,16 @@
         m = m or dict()
         if m.get('maxAttendees') is not None:
             self.max_attendees = m.get('maxAttendees')
         if m.get('maxResults') is not None:
             self.max_results = m.get('maxResults')
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
+        if m.get('seriesMasterId') is not None:
+            self.series_master_id = m.get('seriesMasterId')
         if m.get('showDeleted') is not None:
             self.show_deleted = m.get('showDeleted')
         if m.get('syncToken') is not None:
             self.sync_token = m.get('syncToken')
         if m.get('timeMax') is not None:
             self.time_max = m.get('timeMax')
         if m.get('timeMin') is not None:
```

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,16 @@
             body['agentId'] = request.agent_id
         if not UtilClient.is_unset(request.groups):
             body['groups'] = request.groups
         if not UtilClient.is_unset(request.mobile):
             body['mobile'] = request.mobile
         if not UtilClient.is_unset(request.name):
             body['name'] = request.name
+        if not UtilClient.is_unset(request.need_send_pre_entry_msg):
+            body['needSendPreEntryMsg'] = request.need_send_pre_entry_msg
         if not UtilClient.is_unset(request.pre_entry_time):
             body['preEntryTime'] = request.pre_entry_time
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
@@ -83,14 +85,16 @@
             body['agentId'] = request.agent_id
         if not UtilClient.is_unset(request.groups):
             body['groups'] = request.groups
         if not UtilClient.is_unset(request.mobile):
             body['mobile'] = request.mobile
         if not UtilClient.is_unset(request.name):
             body['name'] = request.name
+        if not UtilClient.is_unset(request.need_send_pre_entry_msg):
+            body['needSendPreEntryMsg'] = request.need_send_pre_entry_msg
         if not UtilClient.is_unset(request.pre_entry_time):
             body['preEntryTime'] = request.pre_entry_time
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
```

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,20 +155,23 @@
 class AddHrmPreentryRequest(TeaModel):
     def __init__(
         self,
         agent_id: int = None,
         groups: List[AddHrmPreentryRequestGroups] = None,
         mobile: str = None,
         name: str = None,
+        need_send_pre_entry_msg: bool = None,
         pre_entry_time: int = None,
     ):
         self.agent_id = agent_id
         self.groups = groups
         self.mobile = mobile
         self.name = name
+        # 是否需要发送完善入职登记表的入职IM消息给员工本人
+        self.need_send_pre_entry_msg = need_send_pre_entry_msg
         self.pre_entry_time = pre_entry_time
 
     def validate(self):
         if self.groups:
             for k in self.groups:
                 if k:
                     k.validate()
@@ -185,14 +188,16 @@
         if self.groups is not None:
             for k in self.groups:
                 result['groups'].append(k.to_map() if k else None)
         if self.mobile is not None:
             result['mobile'] = self.mobile
         if self.name is not None:
             result['name'] = self.name
+        if self.need_send_pre_entry_msg is not None:
+            result['needSendPreEntryMsg'] = self.need_send_pre_entry_msg
         if self.pre_entry_time is not None:
             result['preEntryTime'] = self.pre_entry_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('agentId') is not None:
@@ -202,14 +207,16 @@
             for k in m.get('groups'):
                 temp_model = AddHrmPreentryRequestGroups()
                 self.groups.append(temp_model.from_map(k))
         if m.get('mobile') is not None:
             self.mobile = m.get('mobile')
         if m.get('name') is not None:
             self.name = m.get('name')
+        if m.get('needSendPreEntryMsg') is not None:
+            self.need_send_pre_entry_msg = m.get('needSendPreEntryMsg')
         if m.get('preEntryTime') is not None:
             self.pre_entry_time = m.get('preEntryTime')
         return self
 
 
 class AddHrmPreentryResponseBody(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5255,24 +5255,21 @@
 
 
 class GetFormDataByIDResponseBody(TeaModel):
     def __init__(
         self,
         form_data: Dict[str, Any] = None,
         form_inst_id: str = None,
-        form_uuid: str = None,
         modified_time_gmt: str = None,
         originator: GetFormDataByIDResponseBodyOriginator = None,
     ):
         # 表单数据详情
         self.form_data = form_data
         # 表单实例ID
         self.form_inst_id = form_inst_id
-        # 表单ID
-        self.form_uuid = form_uuid
         # 最后修改时间
         self.modified_time_gmt = modified_time_gmt
         # 发起人详情
         self.originator = originator
 
     def validate(self):
         if self.originator:
@@ -5284,30 +5281,26 @@
             return _map
 
         result = dict()
         if self.form_data is not None:
             result['formData'] = self.form_data
         if self.form_inst_id is not None:
             result['formInstId'] = self.form_inst_id
-        if self.form_uuid is not None:
-            result['formUuid'] = self.form_uuid
         if self.modified_time_gmt is not None:
             result['modifiedTimeGMT'] = self.modified_time_gmt
         if self.originator is not None:
             result['originator'] = self.originator.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('formData') is not None:
             self.form_data = m.get('formData')
         if m.get('formInstId') is not None:
             self.form_inst_id = m.get('formInstId')
-        if m.get('formUuid') is not None:
-            self.form_uuid = m.get('formUuid')
         if m.get('modifiedTimeGMT') is not None:
             self.modified_time_gmt = m.get('modifiedTimeGMT')
         if m.get('originator') is not None:
             temp_model = GetFormDataByIDResponseBodyOriginator()
             self.originator = temp_model.from_map(m['originator'])
         return self
 
@@ -18705,23 +18698,17 @@
             self.type = m.get('type')
         return self
 
 
 class SearchFormDatasResponseBodyDataModifyUser(TeaModel):
     def __init__(
         self,
-        department_name: str = None,
-        email: str = None,
         user_id: str = None,
         user_name: SearchFormDatasResponseBodyDataModifyUserUserName = None,
     ):
-        # 部门名称
-        self.department_name = department_name
-        # 邮箱
-        self.email = email
         # 用户工号
         self.user_id = user_id
         # 用户名
         self.user_name = user_name
 
     def validate(self):
         if self.user_name:
@@ -18729,30 +18716,22 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.department_name is not None:
-            result['departmentName'] = self.department_name
-        if self.email is not None:
-            result['email'] = self.email
         if self.user_id is not None:
             result['userId'] = self.user_id
         if self.user_name is not None:
             result['userName'] = self.user_name.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('departmentName') is not None:
-            self.department_name = m.get('departmentName')
-        if m.get('email') is not None:
-            self.email = m.get('email')
         if m.get('userId') is not None:
             self.user_id = m.get('userId')
         if m.get('userName') is not None:
             temp_model = SearchFormDatasResponseBodyDataModifyUserUserName()
             self.user_name = temp_model.from_map(m['userName'])
         return self
 
@@ -18798,23 +18777,17 @@
             self.type = m.get('type')
         return self
 
 
 class SearchFormDatasResponseBodyDataOriginator(TeaModel):
     def __init__(
         self,
-        department_name: str = None,
-        email: str = None,
         user_id: str = None,
         user_name: SearchFormDatasResponseBodyDataOriginatorUserName = None,
     ):
-        # 部门名称
-        self.department_name = department_name
-        # 邮箱
-        self.email = email
         # 用户工号
         self.user_id = user_id
         # 用户名
         self.user_name = user_name
 
     def validate(self):
         if self.user_name:
@@ -18822,30 +18795,22 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.department_name is not None:
-            result['departmentName'] = self.department_name
-        if self.email is not None:
-            result['email'] = self.email
         if self.user_id is not None:
             result['userId'] = self.user_id
         if self.user_name is not None:
             result['userName'] = self.user_name.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('departmentName') is not None:
-            self.department_name = m.get('departmentName')
-        if m.get('email') is not None:
-            self.email = m.get('email')
         if m.get('userId') is not None:
             self.user_id = m.get('userId')
         if m.get('userName') is not None:
             temp_model = SearchFormDatasResponseBodyDataOriginatorUserName()
             self.user_name = temp_model.from_map(m['userName'])
         return self
```

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 1.5.63
+Version: 1.5.64
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-1.5.63/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.63/setup.py` & `alibabacloud_dingtalk-1.5.64/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 11/04/2023
+Created on 14/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

