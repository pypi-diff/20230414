# Comparing `tmp/cdktf-cdktf-provider-azuread-5.0.5.tar.gz` & `tmp/cdktf-cdktf-provider-azuread-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-azuread-5.0.5.tar", last modified: Sat Mar  4 03:19:34 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-azuread-6.0.0.tar", last modified: Fri Apr 14 03:15:55 2023, max compression
```

## Comparing `cdktf-cdktf-provider-azuread-5.0.5.tar` & `cdktf-cdktf-provider-azuread-6.0.0.tar`

### file list

```diff
@@ -1,105 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.731480 cdktf-cdktf-provider-azuread-5.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-03-04 03:19:34.731480 cdktf-cdktf-provider-azuread-5.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 03:19:34.731480 cdktf-cdktf-provider-azuread-5.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.711479 cdktf-cdktf-provider-azuread-5.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.719480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.719480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2050569 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/_jsii/provider-azuread@5.0.5.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.719480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/administrative_unit/
--rw-r--r--   0 runner    (1001) docker     (123)    44934 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.719480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/administrative_unit_member/
--rw-r--r--   0 runner    (1001) docker     (123)    36110 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/administrative_unit_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.719480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/app_role_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    35528 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/app_role_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application/
--rw-r--r--   0 runner    (1001) docker     (123)   336786 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    51104 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/
--rw-r--r--   0 runner    (1001) docker     (123)    47523 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application_password/
--rw-r--r--   0 runner    (1001) docker     (123)    47170 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application_password/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application_pre_authorized/
--rw-r--r--   0 runner    (1001) docker     (123)    38158 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application_pre_authorized/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/conditional_access_policy/
--rw-r--r--   0 runner    (1001) docker     (123)   159595 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/conditional_access_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/custom_directory_role/
--rw-r--r--   0 runner    (1001) docker     (123)    58656 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/custom_directory_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/
--rw-r--r--   0 runner    (1001) docker     (123)    35968 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_application/
--rw-r--r--   0 runner    (1001) docker     (123)   171186 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/
--rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/
--rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/
--rw-r--r--   0 runner    (1001) docker     (123)    24063 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/
--rw-r--r--   0 runner    (1001) docker     (123)    26028 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/
--rw-r--r--   0 runner    (1001) docker     (123)    33738 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_domains/
--rw-r--r--   0 runner    (1001) docker     (123)    52583 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_domains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_group/
--rw-r--r--   0 runner    (1001) docker     (123)    48087 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.723480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_groups/
--rw-r--r--   0 runner    (1001) docker     (123)    43649 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/
--rw-r--r--   0 runner    (1001) docker     (123)    85954 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/
--rw-r--r--   0 runner    (1001) docker     (123)    50940 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_user/
--rw-r--r--   0 runner    (1001) docker     (123)    38267 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_users/
--rw-r--r--   0 runner    (1001) docker     (123)    48498 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/directory_role/
--rw-r--r--   0 runner    (1001) docker     (123)    34780 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/directory_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/directory_role_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    46418 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/directory_role_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/directory_role_member/
--rw-r--r--   0 runner    (1001) docker     (123)    35113 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/directory_role_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/group/
--rw-r--r--   0 runner    (1001) docker     (123)    98454 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/group_member/
--rw-r--r--   0 runner    (1001) docker     (123)    34251 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/group_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/invitation/
--rw-r--r--   0 runner    (1001) docker     (123)    52285 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/invitation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/named_location/
--rw-r--r--   0 runner    (1001) docker     (123)    53279 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/named_location/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    57813 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal/
--rw-r--r--   0 runner    (1001) docker     (123)   148246 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    51492 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    21574 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    43680 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_password/
--rw-r--r--   0 runner    (1001) docker     (123)    47768 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_password/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    40516 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/synchronization_job/
--rw-r--r--   0 runner    (1001) docker     (123)    47076 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/synchronization_job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.727480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/synchronization_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    50249 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/synchronization_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.731480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/user/
--rw-r--r--   0 runner    (1001) docker     (123)   124438 2023-03-04 03:19:20.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 03:19:34.719480 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-03-04 03:19:34.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-03-04 03:19:34.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 03:19:34.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-04 03:19:34.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-04 03:19:34.000000 cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.963014 cdktf-cdktf-provider-azuread-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-14 03:15:55.963014 cdktf-cdktf-provider-azuread-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 03:15:55.963014 cdktf-cdktf-provider-azuread-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.947014 cdktf-cdktf-provider-azuread-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.951014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.951014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2454082 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/_jsii/provider-azuread@6.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.951014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package/
+-rw-r--r--   0 runner    (1001) docker     (123)    38947 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.951014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)   312905 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    41133 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/
+-rw-r--r--   0 runner    (1001) docker     (123)    37366 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/
+-rw-r--r--   0 runner    (1001) docker     (123)    37722 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)    44934 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    36110 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    38281 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/app_role_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    35528 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/app_role_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application/
+-rw-r--r--   0 runner    (1001) docker     (123)   339995 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    51104 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/
+-rw-r--r--   0 runner    (1001) docker     (123)    47523 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_password/
+-rw-r--r--   0 runner    (1001) docker     (123)    47170 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_password/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_pre_authorized/
+-rw-r--r--   0 runner    (1001) docker     (123)    38158 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_pre_authorized/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/conditional_access_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)   159595 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/conditional_access_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/custom_directory_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    58656 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/custom_directory_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package/
+-rw-r--r--   0 runner    (1001) docker     (123)    31337 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    29683 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)    35968 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application/
+-rw-r--r--   0 runner    (1001) docker     (123)   171414 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    24063 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.955014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/
+-rw-r--r--   0 runner    (1001) docker     (123)    26028 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)    33738 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_domains/
+-rw-r--r--   0 runner    (1001) docker     (123)    52583 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_domains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    48521 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)    43649 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/
+-rw-r--r--   0 runner    (1001) docker     (123)    85954 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/
+-rw-r--r--   0 runner    (1001) docker     (123)    50940 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_user/
+-rw-r--r--   0 runner    (1001) docker     (123)    40255 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_users/
+-rw-r--r--   0 runner    (1001) docker     (123)    48498 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    34780 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    46418 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    35113 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/group/
+-rw-r--r--   0 runner    (1001) docker     (123)   104726 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/group_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    34251 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/group_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/invitation/
+-rw-r--r--   0 runner    (1001) docker     (123)    52285 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/invitation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/named_location/
+-rw-r--r--   0 runner    (1001) docker     (123)    53279 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/named_location/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    57813 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal/
+-rw-r--r--   0 runner    (1001) docker     (123)   148246 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    51492 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    21574 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    43680 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_password/
+-rw-r--r--   0 runner    (1001) docker     (123)    47768 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_password/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    40516 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/synchronization_job/
+-rw-r--r--   0 runner    (1001) docker     (123)    47076 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/synchronization_job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/synchronization_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    50249 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/synchronization_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.959014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/user/
+-rw-r--r--   0 runner    (1001) docker     (123)   124438 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.963014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/user_flow_attribute/
+-rw-r--r--   0 runner    (1001) docker     (123)    36734 2023-04-14 03:15:41.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/user_flow_attribute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:15:55.951014 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-14 03:15:55.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-14 03:15:55.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:15:55.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 03:15:55.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 03:15:55.000000 cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/LICENSE` & `cdktf-cdktf-provider-azuread-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/PKG-INFO` & `cdktf-cdktf-provider-azuread-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-azuread
-Version: 5.0.5
+Version: 6.0.0
 Summary: Prebuilt azuread Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-azuread.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-azuread.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/README.md` & `cdktf-cdktf-provider-azuread-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/setup.py` & `cdktf-cdktf-provider-azuread-6.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-azuread",
-    "version": "5.0.5",
+    "version": "6.0.0",
     "description": "Prebuilt azuread Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-azuread.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -19,25 +19,33 @@
     },
     "package_dir": {
         "": "src"
     },
     "packages": [
         "cdktf_cdktf_provider_azuread",
         "cdktf_cdktf_provider_azuread._jsii",
+        "cdktf_cdktf_provider_azuread.access_package",
+        "cdktf_cdktf_provider_azuread.access_package_assignment_policy",
+        "cdktf_cdktf_provider_azuread.access_package_catalog",
+        "cdktf_cdktf_provider_azuread.access_package_resource_catalog_association",
+        "cdktf_cdktf_provider_azuread.access_package_resource_package_association",
         "cdktf_cdktf_provider_azuread.administrative_unit",
         "cdktf_cdktf_provider_azuread.administrative_unit_member",
+        "cdktf_cdktf_provider_azuread.administrative_unit_role_member",
         "cdktf_cdktf_provider_azuread.app_role_assignment",
         "cdktf_cdktf_provider_azuread.application",
         "cdktf_cdktf_provider_azuread.application_certificate",
         "cdktf_cdktf_provider_azuread.application_federated_identity_credential",
         "cdktf_cdktf_provider_azuread.application_password",
         "cdktf_cdktf_provider_azuread.application_pre_authorized",
         "cdktf_cdktf_provider_azuread.claims_mapping_policy",
         "cdktf_cdktf_provider_azuread.conditional_access_policy",
         "cdktf_cdktf_provider_azuread.custom_directory_role",
+        "cdktf_cdktf_provider_azuread.data_azuread_access_package",
+        "cdktf_cdktf_provider_azuread.data_azuread_access_package_catalog",
         "cdktf_cdktf_provider_azuread.data_azuread_administrative_unit",
         "cdktf_cdktf_provider_azuread.data_azuread_application",
         "cdktf_cdktf_provider_azuread.data_azuread_application_published_app_ids",
         "cdktf_cdktf_provider_azuread.data_azuread_application_template",
         "cdktf_cdktf_provider_azuread.data_azuread_client_config",
         "cdktf_cdktf_provider_azuread.data_azuread_directory_object",
         "cdktf_cdktf_provider_azuread.data_azuread_directory_roles",
@@ -60,41 +68,43 @@
         "cdktf_cdktf_provider_azuread.service_principal_certificate",
         "cdktf_cdktf_provider_azuread.service_principal_claims_mapping_policy_assignment",
         "cdktf_cdktf_provider_azuread.service_principal_delegated_permission_grant",
         "cdktf_cdktf_provider_azuread.service_principal_password",
         "cdktf_cdktf_provider_azuread.service_principal_token_signing_certificate",
         "cdktf_cdktf_provider_azuread.synchronization_job",
         "cdktf_cdktf_provider_azuread.synchronization_secret",
-        "cdktf_cdktf_provider_azuread.user"
+        "cdktf_cdktf_provider_azuread.user",
+        "cdktf_cdktf_provider_azuread.user_flow_attribute"
     ],
     "package_data": {
         "cdktf_cdktf_provider_azuread._jsii": [
-            "provider-azuread@5.0.5.jsii.tgz"
+            "provider-azuread@6.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_azuread": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdktf>=0.15.0, <0.16.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.76.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -101,25 +101,33 @@
 import typing_extensions
 
 from typeguard import check_type
 
 from ._jsii import *
 
 __all__ = [
+    "access_package",
+    "access_package_assignment_policy",
+    "access_package_catalog",
+    "access_package_resource_catalog_association",
+    "access_package_resource_package_association",
     "administrative_unit",
     "administrative_unit_member",
+    "administrative_unit_role_member",
     "app_role_assignment",
     "application",
     "application_certificate",
     "application_federated_identity_credential",
     "application_password",
     "application_pre_authorized",
     "claims_mapping_policy",
     "conditional_access_policy",
     "custom_directory_role",
+    "data_azuread_access_package",
+    "data_azuread_access_package_catalog",
     "data_azuread_administrative_unit",
     "data_azuread_application",
     "data_azuread_application_published_app_ids",
     "data_azuread_application_template",
     "data_azuread_client_config",
     "data_azuread_directory_object",
     "data_azuread_directory_roles",
@@ -143,30 +151,39 @@
     "service_principal_claims_mapping_policy_assignment",
     "service_principal_delegated_permission_grant",
     "service_principal_password",
     "service_principal_token_signing_certificate",
     "synchronization_job",
     "synchronization_secret",
     "user",
+    "user_flow_attribute",
 ]
 
 publication.publish()
 
 # Loading modules to ensure their types are registered with the jsii runtime library
+from . import access_package
+from . import access_package_assignment_policy
+from . import access_package_catalog
+from . import access_package_resource_catalog_association
+from . import access_package_resource_package_association
 from . import administrative_unit
 from . import administrative_unit_member
+from . import administrative_unit_role_member
 from . import app_role_assignment
 from . import application
 from . import application_certificate
 from . import application_federated_identity_credential
 from . import application_password
 from . import application_pre_authorized
 from . import claims_mapping_policy
 from . import conditional_access_policy
 from . import custom_directory_role
+from . import data_azuread_access_package
+from . import data_azuread_access_package_catalog
 from . import data_azuread_administrative_unit
 from . import data_azuread_application
 from . import data_azuread_application_published_app_ids
 from . import data_azuread_application_template
 from . import data_azuread_client_config
 from . import data_azuread_directory_object
 from . import data_azuread_directory_roles
@@ -190,7 +207,8 @@
 from . import service_principal_claims_mapping_policy_assignment
 from . import service_principal_delegated_permission_grant
 from . import service_principal_password
 from . import service_principal_token_signing_certificate
 from . import synchronization_job
 from . import synchronization_secret
 from . import user
+from . import user_flow_attribute
```

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/administrative_unit_member/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/app_role_assignment/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/app_role_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         oauth2_post_response_required: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         optional_claims: typing.Optional[typing.Union["ApplicationOptionalClaims", typing.Dict[builtins.str, typing.Any]]] = None,
         owners: typing.Optional[typing.Sequence[builtins.str]] = None,
         prevent_duplicate_names: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         privacy_statement_url: typing.Optional[builtins.str] = None,
         public_client: typing.Optional[typing.Union["ApplicationPublicClient", typing.Dict[builtins.str, typing.Any]]] = None,
         required_resource_access: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ApplicationRequiredResourceAccess", typing.Dict[builtins.str, typing.Any]]]]] = None,
+        service_management_reference: typing.Optional[builtins.str] = None,
         sign_in_audience: typing.Optional[builtins.str] = None,
         single_page_application: typing.Optional[typing.Union["ApplicationSinglePageApplication", typing.Dict[builtins.str, typing.Any]]] = None,
         support_url: typing.Optional[builtins.str] = None,
         tags: typing.Optional[typing.Sequence[builtins.str]] = None,
         template_id: typing.Optional[builtins.str] = None,
         terms_of_service_url: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["ApplicationTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
@@ -89,14 +90,15 @@
         :param oauth2_post_response_required: Specifies whether, as part of OAuth 2.0 token requests, Azure AD allows POST requests, as opposed to GET requests. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#oauth2_post_response_required Application#oauth2_post_response_required}
         :param optional_claims: optional_claims block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#optional_claims Application#optional_claims}
         :param owners: A list of object IDs of principals that will be granted ownership of the application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#owners Application#owners}
         :param prevent_duplicate_names: If ``true``, will return an error if an existing application is found with the same name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#prevent_duplicate_names Application#prevent_duplicate_names}
         :param privacy_statement_url: URL of the application's privacy statement. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#privacy_statement_url Application#privacy_statement_url}
         :param public_client: public_client block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#public_client Application#public_client}
         :param required_resource_access: required_resource_access block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#required_resource_access Application#required_resource_access}
+        :param service_management_reference: References application or service contact information from a Service or Asset Management database. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#service_management_reference Application#service_management_reference}
         :param sign_in_audience: The Microsoft account types that are supported for the current application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#sign_in_audience Application#sign_in_audience}
         :param single_page_application: single_page_application block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#single_page_application Application#single_page_application}
         :param support_url: URL of the application's support page. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#support_url Application#support_url}
         :param tags: A set of tags to apply to the application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#tags Application#tags}
         :param template_id: Unique ID of the application template from which this application is created. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#template_id Application#template_id}
         :param terms_of_service_url: URL of the application's terms of service statement. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#terms_of_service_url Application#terms_of_service_url}
         :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#timeouts Application#timeouts}
@@ -130,14 +132,15 @@
             oauth2_post_response_required=oauth2_post_response_required,
             optional_claims=optional_claims,
             owners=owners,
             prevent_duplicate_names=prevent_duplicate_names,
             privacy_statement_url=privacy_statement_url,
             public_client=public_client,
             required_resource_access=required_resource_access,
+            service_management_reference=service_management_reference,
             sign_in_audience=sign_in_audience,
             single_page_application=single_page_application,
             support_url=support_url,
             tags=tags,
             template_id=template_id,
             terms_of_service_url=terms_of_service_url,
             timeouts=timeouts,
@@ -378,14 +381,18 @@
     def reset_public_client(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetPublicClient", []))
 
     @jsii.member(jsii_name="resetRequiredResourceAccess")
     def reset_required_resource_access(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetRequiredResourceAccess", []))
 
+    @jsii.member(jsii_name="resetServiceManagementReference")
+    def reset_service_management_reference(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetServiceManagementReference", []))
+
     @jsii.member(jsii_name="resetSignInAudience")
     def reset_sign_in_audience(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetSignInAudience", []))
 
     @jsii.member(jsii_name="resetSinglePageApplication")
     def reset_single_page_application(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetSinglePageApplication", []))
@@ -618,14 +625,19 @@
     @jsii.member(jsii_name="requiredResourceAccessInput")
     def required_resource_access_input(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ApplicationRequiredResourceAccess"]]]:
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ApplicationRequiredResourceAccess"]]], jsii.get(self, "requiredResourceAccessInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="serviceManagementReferenceInput")
+    def service_management_reference_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "serviceManagementReferenceInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="signInAudienceInput")
     def sign_in_audience_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "signInAudienceInput"))
 
     @builtins.property
     @jsii.member(jsii_name="singlePageApplicationInput")
     def single_page_application_input(
@@ -850,14 +862,26 @@
     def privacy_statement_url(self, value: builtins.str) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2abe2527a40053f36c39edc05474ae1ecd773193611946ac0e2567b524be8def)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "privacyStatementUrl", value)
 
     @builtins.property
+    @jsii.member(jsii_name="serviceManagementReference")
+    def service_management_reference(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "serviceManagementReference"))
+
+    @service_management_reference.setter
+    def service_management_reference(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__4d3379a935de6279c322ac6bad07850eb5afa2c82d99a279ad07a616dc069a84)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "serviceManagementReference", value)
+
+    @builtins.property
     @jsii.member(jsii_name="signInAudience")
     def sign_in_audience(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "signInAudience"))
 
     @sign_in_audience.setter
     def sign_in_audience(self, value: builtins.str) -> None:
         if __debug__:
@@ -2003,14 +2027,15 @@
         "oauth2_post_response_required": "oauth2PostResponseRequired",
         "optional_claims": "optionalClaims",
         "owners": "owners",
         "prevent_duplicate_names": "preventDuplicateNames",
         "privacy_statement_url": "privacyStatementUrl",
         "public_client": "publicClient",
         "required_resource_access": "requiredResourceAccess",
+        "service_management_reference": "serviceManagementReference",
         "sign_in_audience": "signInAudience",
         "single_page_application": "singlePageApplication",
         "support_url": "supportUrl",
         "tags": "tags",
         "template_id": "templateId",
         "terms_of_service_url": "termsOfServiceUrl",
         "timeouts": "timeouts",
@@ -2044,14 +2069,15 @@
         oauth2_post_response_required: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         optional_claims: typing.Optional[typing.Union["ApplicationOptionalClaims", typing.Dict[builtins.str, typing.Any]]] = None,
         owners: typing.Optional[typing.Sequence[builtins.str]] = None,
         prevent_duplicate_names: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         privacy_statement_url: typing.Optional[builtins.str] = None,
         public_client: typing.Optional[typing.Union["ApplicationPublicClient", typing.Dict[builtins.str, typing.Any]]] = None,
         required_resource_access: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ApplicationRequiredResourceAccess", typing.Dict[builtins.str, typing.Any]]]]] = None,
+        service_management_reference: typing.Optional[builtins.str] = None,
         sign_in_audience: typing.Optional[builtins.str] = None,
         single_page_application: typing.Optional[typing.Union["ApplicationSinglePageApplication", typing.Dict[builtins.str, typing.Any]]] = None,
         support_url: typing.Optional[builtins.str] = None,
         tags: typing.Optional[typing.Sequence[builtins.str]] = None,
         template_id: typing.Optional[builtins.str] = None,
         terms_of_service_url: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["ApplicationTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
@@ -2081,14 +2107,15 @@
         :param oauth2_post_response_required: Specifies whether, as part of OAuth 2.0 token requests, Azure AD allows POST requests, as opposed to GET requests. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#oauth2_post_response_required Application#oauth2_post_response_required}
         :param optional_claims: optional_claims block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#optional_claims Application#optional_claims}
         :param owners: A list of object IDs of principals that will be granted ownership of the application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#owners Application#owners}
         :param prevent_duplicate_names: If ``true``, will return an error if an existing application is found with the same name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#prevent_duplicate_names Application#prevent_duplicate_names}
         :param privacy_statement_url: URL of the application's privacy statement. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#privacy_statement_url Application#privacy_statement_url}
         :param public_client: public_client block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#public_client Application#public_client}
         :param required_resource_access: required_resource_access block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#required_resource_access Application#required_resource_access}
+        :param service_management_reference: References application or service contact information from a Service or Asset Management database. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#service_management_reference Application#service_management_reference}
         :param sign_in_audience: The Microsoft account types that are supported for the current application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#sign_in_audience Application#sign_in_audience}
         :param single_page_application: single_page_application block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#single_page_application Application#single_page_application}
         :param support_url: URL of the application's support page. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#support_url Application#support_url}
         :param tags: A set of tags to apply to the application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#tags Application#tags}
         :param template_id: Unique ID of the application template from which this application is created. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#template_id Application#template_id}
         :param terms_of_service_url: URL of the application's terms of service statement. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#terms_of_service_url Application#terms_of_service_url}
         :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#timeouts Application#timeouts}
@@ -2133,14 +2160,15 @@
             check_type(argname="argument oauth2_post_response_required", value=oauth2_post_response_required, expected_type=type_hints["oauth2_post_response_required"])
             check_type(argname="argument optional_claims", value=optional_claims, expected_type=type_hints["optional_claims"])
             check_type(argname="argument owners", value=owners, expected_type=type_hints["owners"])
             check_type(argname="argument prevent_duplicate_names", value=prevent_duplicate_names, expected_type=type_hints["prevent_duplicate_names"])
             check_type(argname="argument privacy_statement_url", value=privacy_statement_url, expected_type=type_hints["privacy_statement_url"])
             check_type(argname="argument public_client", value=public_client, expected_type=type_hints["public_client"])
             check_type(argname="argument required_resource_access", value=required_resource_access, expected_type=type_hints["required_resource_access"])
+            check_type(argname="argument service_management_reference", value=service_management_reference, expected_type=type_hints["service_management_reference"])
             check_type(argname="argument sign_in_audience", value=sign_in_audience, expected_type=type_hints["sign_in_audience"])
             check_type(argname="argument single_page_application", value=single_page_application, expected_type=type_hints["single_page_application"])
             check_type(argname="argument support_url", value=support_url, expected_type=type_hints["support_url"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument template_id", value=template_id, expected_type=type_hints["template_id"])
             check_type(argname="argument terms_of_service_url", value=terms_of_service_url, expected_type=type_hints["terms_of_service_url"])
             check_type(argname="argument timeouts", value=timeouts, expected_type=type_hints["timeouts"])
@@ -2196,14 +2224,16 @@
             self._values["prevent_duplicate_names"] = prevent_duplicate_names
         if privacy_statement_url is not None:
             self._values["privacy_statement_url"] = privacy_statement_url
         if public_client is not None:
             self._values["public_client"] = public_client
         if required_resource_access is not None:
             self._values["required_resource_access"] = required_resource_access
+        if service_management_reference is not None:
+            self._values["service_management_reference"] = service_management_reference
         if sign_in_audience is not None:
             self._values["sign_in_audience"] = sign_in_audience
         if single_page_application is not None:
             self._values["single_page_application"] = single_page_application
         if support_url is not None:
             self._values["support_url"] = support_url
         if tags is not None:
@@ -2474,14 +2504,23 @@
 
         Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#required_resource_access Application#required_resource_access}
         '''
         result = self._values.get("required_resource_access")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ApplicationRequiredResourceAccess"]]], result)
 
     @builtins.property
+    def service_management_reference(self) -> typing.Optional[builtins.str]:
+        '''References application or service contact information from a Service or Asset Management database.
+
+        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#service_management_reference Application#service_management_reference}
+        '''
+        result = self._values.get("service_management_reference")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def sign_in_audience(self) -> typing.Optional[builtins.str]:
         '''The Microsoft account types that are supported for the current application.
 
         Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/application#sign_in_audience Application#sign_in_audience}
         '''
         result = self._values.get("sign_in_audience")
         return typing.cast(typing.Optional[builtins.str], result)
@@ -5346,14 +5385,15 @@
     oauth2_post_response_required: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     optional_claims: typing.Optional[typing.Union[ApplicationOptionalClaims, typing.Dict[builtins.str, typing.Any]]] = None,
     owners: typing.Optional[typing.Sequence[builtins.str]] = None,
     prevent_duplicate_names: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     privacy_statement_url: typing.Optional[builtins.str] = None,
     public_client: typing.Optional[typing.Union[ApplicationPublicClient, typing.Dict[builtins.str, typing.Any]]] = None,
     required_resource_access: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ApplicationRequiredResourceAccess, typing.Dict[builtins.str, typing.Any]]]]] = None,
+    service_management_reference: typing.Optional[builtins.str] = None,
     sign_in_audience: typing.Optional[builtins.str] = None,
     single_page_application: typing.Optional[typing.Union[ApplicationSinglePageApplication, typing.Dict[builtins.str, typing.Any]]] = None,
     support_url: typing.Optional[builtins.str] = None,
     tags: typing.Optional[typing.Sequence[builtins.str]] = None,
     template_id: typing.Optional[builtins.str] = None,
     terms_of_service_url: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[ApplicationTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -5467,14 +5507,20 @@
 
 def _typecheckingstub__2abe2527a40053f36c39edc05474ae1ecd773193611946ac0e2567b524be8def(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__4d3379a935de6279c322ac6bad07850eb5afa2c82d99a279ad07a616dc069a84(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__e9aa5403d0d67c71116c7dda47a66970883add862c75c0e4179b4df2d3d42d0b(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__a88c7e24fa536fe013f7a05ae1a9a969a285cf3629f02713c1de7c0a7303caf3(
@@ -5789,14 +5835,15 @@
     oauth2_post_response_required: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     optional_claims: typing.Optional[typing.Union[ApplicationOptionalClaims, typing.Dict[builtins.str, typing.Any]]] = None,
     owners: typing.Optional[typing.Sequence[builtins.str]] = None,
     prevent_duplicate_names: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     privacy_statement_url: typing.Optional[builtins.str] = None,
     public_client: typing.Optional[typing.Union[ApplicationPublicClient, typing.Dict[builtins.str, typing.Any]]] = None,
     required_resource_access: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ApplicationRequiredResourceAccess, typing.Dict[builtins.str, typing.Any]]]]] = None,
+    service_management_reference: typing.Optional[builtins.str] = None,
     sign_in_audience: typing.Optional[builtins.str] = None,
     single_page_application: typing.Optional[typing.Union[ApplicationSinglePageApplication, typing.Dict[builtins.str, typing.Any]]] = None,
     support_url: typing.Optional[builtins.str] = None,
     tags: typing.Optional[typing.Sequence[builtins.str]] = None,
     template_id: typing.Optional[builtins.str] = None,
     terms_of_service_url: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[ApplicationTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
```

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application_certificate/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application_password/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_password/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/application_pre_authorized/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/application_pre_authorized/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/conditional_access_policy/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/conditional_access_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/custom_directory_role/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/custom_directory_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_application/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,14 +226,19 @@
     @jsii.member(jsii_name="requiredResourceAccess")
     def required_resource_access(
         self,
     ) -> "DataAzureadApplicationRequiredResourceAccessList":
         return typing.cast("DataAzureadApplicationRequiredResourceAccessList", jsii.get(self, "requiredResourceAccess"))
 
     @builtins.property
+    @jsii.member(jsii_name="serviceManagementReference")
+    def service_management_reference(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "serviceManagementReference"))
+
+    @builtins.property
     @jsii.member(jsii_name="signInAudience")
     def sign_in_audience(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "signInAudience"))
 
     @builtins.property
     @jsii.member(jsii_name="singlePageApplication")
     def single_page_application(
```

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_domains/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_domains/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_group/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_group/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,19 @@
 
     @builtins.property
     @jsii.member(jsii_name="onpremisesDomainName")
     def onpremises_domain_name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "onpremisesDomainName"))
 
     @builtins.property
+    @jsii.member(jsii_name="onpremisesGroupType")
+    def onpremises_group_type(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "onpremisesGroupType"))
+
+    @builtins.property
     @jsii.member(jsii_name="onpremisesNetbiosName")
     def onpremises_netbios_name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "onpremisesNetbiosName"))
 
     @builtins.property
     @jsii.member(jsii_name="onpremisesSamAccountName")
     def onpremises_sam_account_name(self) -> builtins.str:
@@ -246,14 +251,19 @@
 
     @builtins.property
     @jsii.member(jsii_name="visibility")
     def visibility(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "visibility"))
 
     @builtins.property
+    @jsii.member(jsii_name="writebackEnabled")
+    def writeback_enabled(self) -> _cdktf_9a9027ec.IResolvable:
+        return typing.cast(_cdktf_9a9027ec.IResolvable, jsii.get(self, "writebackEnabled"))
+
+    @builtins.property
     @jsii.member(jsii_name="displayNameInput")
     def display_name_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "displayNameInput"))
 
     @builtins.property
     @jsii.member(jsii_name="idInput")
     def id_input(self) -> typing.Optional[builtins.str]:
```

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_groups/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_user/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_user/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
+        mail: typing.Optional[builtins.str] = None,
         mail_nickname: typing.Optional[builtins.str] = None,
         object_id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataAzureadUserTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         user_principal_name: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[jsii.Number] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
@@ -47,14 +48,15 @@
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
         '''Create a new {@link https://www.terraform.io/docs/providers/azuread/d/user azuread_user} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
         :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/d/user#id DataAzureadUser#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param mail: The SMTP address for the user. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/d/user#mail DataAzureadUser#mail}
         :param mail_nickname: The email alias of the user. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/d/user#mail_nickname DataAzureadUser#mail_nickname}
         :param object_id: The object ID of the user. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/d/user#object_id DataAzureadUser#object_id}
         :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/d/user#timeouts DataAzureadUser#timeouts}
         :param user_principal_name: The user principal name (UPN) of the user. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/d/user#user_principal_name DataAzureadUser#user_principal_name}
         :param connection: 
         :param count: 
         :param depends_on: 
@@ -65,14 +67,15 @@
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0f2eb5c3b56abd12687b991210cbfcf7505584474a3051b3cb7d27514fbb092d)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
         config = DataAzureadUserConfig(
             id=id,
+            mail=mail,
             mail_nickname=mail_nickname,
             object_id=object_id,
             timeouts=timeouts,
             user_principal_name=user_principal_name,
             connection=connection,
             count=count,
             depends_on=depends_on,
@@ -93,14 +96,18 @@
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetId", []))
 
+    @jsii.member(jsii_name="resetMail")
+    def reset_mail(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetMail", []))
+
     @jsii.member(jsii_name="resetMailNickname")
     def reset_mail_nickname(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetMailNickname", []))
 
     @jsii.member(jsii_name="resetObjectId")
     def reset_object_id(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetObjectId", []))
@@ -214,19 +221,14 @@
 
     @builtins.property
     @jsii.member(jsii_name="jobTitle")
     def job_title(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "jobTitle"))
 
     @builtins.property
-    @jsii.member(jsii_name="mail")
-    def mail(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "mail"))
-
-    @builtins.property
     @jsii.member(jsii_name="managerId")
     def manager_id(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "managerId"))
 
     @builtins.property
     @jsii.member(jsii_name="mobilePhone")
     def mobile_phone(self) -> builtins.str:
@@ -329,14 +331,19 @@
 
     @builtins.property
     @jsii.member(jsii_name="idInput")
     def id_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "idInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="mailInput")
+    def mail_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "mailInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="mailNicknameInput")
     def mail_nickname_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "mailNicknameInput"))
 
     @builtins.property
     @jsii.member(jsii_name="objectIdInput")
     def object_id_input(self) -> typing.Optional[builtins.str]:
@@ -363,14 +370,26 @@
     def id(self, value: builtins.str) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5aaef3b37e4f31ffdfbc9484b64c4668ecbe029a742e64cd7a7bbc272c7abe69)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "id", value)
 
     @builtins.property
+    @jsii.member(jsii_name="mail")
+    def mail(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "mail"))
+
+    @mail.setter
+    def mail(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9fcd40ea8b7605446b4fdb3d5f7c2a2bfc98b70c1eb43295dd2ae1e06d9422b8)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "mail", value)
+
+    @builtins.property
     @jsii.member(jsii_name="mailNickname")
     def mail_nickname(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "mailNickname"))
 
     @mail_nickname.setter
     def mail_nickname(self, value: builtins.str) -> None:
         if __debug__:
@@ -411,14 +430,15 @@
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "id": "id",
+        "mail": "mail",
         "mail_nickname": "mailNickname",
         "object_id": "objectId",
         "timeouts": "timeouts",
         "user_principal_name": "userPrincipalName",
     },
 )
 class DataAzureadUserConfig(_cdktf_9a9027ec.TerraformMetaArguments):
@@ -429,28 +449,30 @@
         count: typing.Optional[jsii.Number] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         id: typing.Optional[builtins.str] = None,
+        mail: typing.Optional[builtins.str] = None,
         mail_nickname: typing.Optional[builtins.str] = None,
         object_id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataAzureadUserTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         user_principal_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/d/user#id DataAzureadUser#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param mail: The SMTP address for the user. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/d/user#mail DataAzureadUser#mail}
         :param mail_nickname: The email alias of the user. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/d/user#mail_nickname DataAzureadUser#mail_nickname}
         :param object_id: The object ID of the user. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/d/user#object_id DataAzureadUser#object_id}
         :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/d/user#timeouts DataAzureadUser#timeouts}
         :param user_principal_name: The user principal name (UPN) of the user. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/d/user#user_principal_name DataAzureadUser#user_principal_name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
@@ -462,14 +484,15 @@
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument mail", value=mail, expected_type=type_hints["mail"])
             check_type(argname="argument mail_nickname", value=mail_nickname, expected_type=type_hints["mail_nickname"])
             check_type(argname="argument object_id", value=object_id, expected_type=type_hints["object_id"])
             check_type(argname="argument timeouts", value=timeouts, expected_type=type_hints["timeouts"])
             check_type(argname="argument user_principal_name", value=user_principal_name, expected_type=type_hints["user_principal_name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if connection is not None:
             self._values["connection"] = connection
@@ -483,14 +506,16 @@
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
         if id is not None:
             self._values["id"] = id
+        if mail is not None:
+            self._values["mail"] = mail
         if mail_nickname is not None:
             self._values["mail_nickname"] = mail_nickname
         if object_id is not None:
             self._values["object_id"] = object_id
         if timeouts is not None:
             self._values["timeouts"] = timeouts
         if user_principal_name is not None:
@@ -565,14 +590,23 @@
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def mail(self) -> typing.Optional[builtins.str]:
+        '''The SMTP address for the user.
+
+        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/d/user#mail DataAzureadUser#mail}
+        '''
+        result = self._values.get("mail")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def mail_nickname(self) -> typing.Optional[builtins.str]:
         '''The email alias of the user.
 
         Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/d/user#mail_nickname DataAzureadUser#mail_nickname}
         '''
         result = self._values.get("mail_nickname")
         return typing.cast(typing.Optional[builtins.str], result)
@@ -720,14 +754,15 @@
 publication.publish()
 
 def _typecheckingstub__0f2eb5c3b56abd12687b991210cbfcf7505584474a3051b3cb7d27514fbb092d(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     id: typing.Optional[builtins.str] = None,
+    mail: typing.Optional[builtins.str] = None,
     mail_nickname: typing.Optional[builtins.str] = None,
     object_id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataAzureadUserTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
     user_principal_name: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[jsii.Number] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
@@ -741,14 +776,20 @@
 
 def _typecheckingstub__5aaef3b37e4f31ffdfbc9484b64c4668ecbe029a742e64cd7a7bbc272c7abe69(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__9fcd40ea8b7605446b4fdb3d5f7c2a2bfc98b70c1eb43295dd2ae1e06d9422b8(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__374d1d710cc3ecb4ac7b58de7a56693b01a4b022c4b442333d1f5d402588368d(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__020468c8e6d4f7ccc94fa115bdf52ee6a4c0308ec14e26fb5c1d778cc3c5197e(
@@ -769,14 +810,15 @@
     count: typing.Optional[jsii.Number] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
+    mail: typing.Optional[builtins.str] = None,
     mail_nickname: typing.Optional[builtins.str] = None,
     object_id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataAzureadUserTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
     user_principal_name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/data_azuread_users/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_users/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/directory_role/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/directory_role_assignment/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/directory_role_member/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/directory_role_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/group/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/group/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,22 +43,24 @@
         external_senders_allowed: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         hide_from_address_lists: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         hide_from_outlook_clients: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         id: typing.Optional[builtins.str] = None,
         mail_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         mail_nickname: typing.Optional[builtins.str] = None,
         members: typing.Optional[typing.Sequence[builtins.str]] = None,
+        onpremises_group_type: typing.Optional[builtins.str] = None,
         owners: typing.Optional[typing.Sequence[builtins.str]] = None,
         prevent_duplicate_names: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         provisioning_options: typing.Optional[typing.Sequence[builtins.str]] = None,
         security_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         theme: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["GroupTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         types: typing.Optional[typing.Sequence[builtins.str]] = None,
         visibility: typing.Optional[builtins.str] = None,
+        writeback_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[jsii.Number] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
@@ -77,22 +79,24 @@
         :param external_senders_allowed: Indicates whether people external to the organization can send messages to the group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#external_senders_allowed Group#external_senders_allowed}
         :param hide_from_address_lists: Indicates whether the group is displayed in certain parts of the Outlook user interface: in the Address Book, in address lists for selecting message recipients, and in the Browse Groups dialog for searching groups. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#hide_from_address_lists Group#hide_from_address_lists}
         :param hide_from_outlook_clients: Indicates whether the group is displayed in Outlook clients, such as Outlook for Windows and Outlook on the web. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#hide_from_outlook_clients Group#hide_from_outlook_clients}
         :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#id Group#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param mail_enabled: Whether the group is a mail enabled, with a shared group mailbox. At least one of ``mail_enabled`` or ``security_enabled`` must be specified. A group can be mail enabled *and* security enabled Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#mail_enabled Group#mail_enabled}
         :param mail_nickname: The mail alias for the group, unique in the organisation. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#mail_nickname Group#mail_nickname}
         :param members: A set of members who should be present in this group. Supported object types are Users, Groups or Service Principals Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#members Group#members}
+        :param onpremises_group_type: Indicates the target on-premise group type the group will be written back as. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#onpremises_group_type Group#onpremises_group_type}
         :param owners: A set of owners who own this group. Supported object types are Users or Service Principals. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#owners Group#owners}
         :param prevent_duplicate_names: If ``true``, will return an error if an existing group is found with the same name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#prevent_duplicate_names Group#prevent_duplicate_names}
         :param provisioning_options: The group provisioning options for a Microsoft 365 group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#provisioning_options Group#provisioning_options}
         :param security_enabled: Whether the group is a security group for controlling access to in-app resources. At least one of ``security_enabled`` or ``mail_enabled`` must be specified. A group can be security enabled *and* mail enabled Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#security_enabled Group#security_enabled}
         :param theme: The colour theme for a Microsoft 365 group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#theme Group#theme}
         :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#timeouts Group#timeouts}
         :param types: A set of group types to configure for the group. ``Unified`` specifies a Microsoft 365 group. Required when ``mail_enabled`` is true Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#types Group#types}
         :param visibility: Specifies the group join policy and group content visibility. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#visibility Group#visibility}
+        :param writeback_enabled: Whether this group should be synced from Azure AD to the on-premises directory when Azure AD Connect is used. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#writeback_enabled Group#writeback_enabled}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -112,22 +116,24 @@
             external_senders_allowed=external_senders_allowed,
             hide_from_address_lists=hide_from_address_lists,
             hide_from_outlook_clients=hide_from_outlook_clients,
             id=id,
             mail_enabled=mail_enabled,
             mail_nickname=mail_nickname,
             members=members,
+            onpremises_group_type=onpremises_group_type,
             owners=owners,
             prevent_duplicate_names=prevent_duplicate_names,
             provisioning_options=provisioning_options,
             security_enabled=security_enabled,
             theme=theme,
             timeouts=timeouts,
             types=types,
             visibility=visibility,
+            writeback_enabled=writeback_enabled,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
@@ -217,14 +223,18 @@
     def reset_mail_nickname(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetMailNickname", []))
 
     @jsii.member(jsii_name="resetMembers")
     def reset_members(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetMembers", []))
 
+    @jsii.member(jsii_name="resetOnpremisesGroupType")
+    def reset_onpremises_group_type(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetOnpremisesGroupType", []))
+
     @jsii.member(jsii_name="resetOwners")
     def reset_owners(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetOwners", []))
 
     @jsii.member(jsii_name="resetPreventDuplicateNames")
     def reset_prevent_duplicate_names(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetPreventDuplicateNames", []))
@@ -249,14 +259,18 @@
     def reset_types(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetTypes", []))
 
     @jsii.member(jsii_name="resetVisibility")
     def reset_visibility(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetVisibility", []))
 
+    @jsii.member(jsii_name="resetWritebackEnabled")
+    def reset_writeback_enabled(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetWritebackEnabled", []))
+
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
@@ -398,14 +412,19 @@
 
     @builtins.property
     @jsii.member(jsii_name="membersInput")
     def members_input(self) -> typing.Optional[typing.List[builtins.str]]:
         return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "membersInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="onpremisesGroupTypeInput")
+    def onpremises_group_type_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "onpremisesGroupTypeInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="ownersInput")
     def owners_input(self) -> typing.Optional[typing.List[builtins.str]]:
         return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "ownersInput"))
 
     @builtins.property
     @jsii.member(jsii_name="preventDuplicateNamesInput")
     def prevent_duplicate_names_input(
@@ -444,14 +463,21 @@
 
     @builtins.property
     @jsii.member(jsii_name="visibilityInput")
     def visibility_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "visibilityInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="writebackEnabledInput")
+    def writeback_enabled_input(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "writebackEnabledInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="administrativeUnitIds")
     def administrative_unit_ids(self) -> typing.List[builtins.str]:
         return typing.cast(typing.List[builtins.str], jsii.get(self, "administrativeUnitIds"))
 
     @administrative_unit_ids.setter
     def administrative_unit_ids(self, value: typing.List[builtins.str]) -> None:
         if __debug__:
@@ -628,14 +654,26 @@
     def members(self, value: typing.List[builtins.str]) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__08b262a67fbb284a8d5b748d0d6b57e4862e547efaa86bbd5823d43a4e5a44d2)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "members", value)
 
     @builtins.property
+    @jsii.member(jsii_name="onpremisesGroupType")
+    def onpremises_group_type(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "onpremisesGroupType"))
+
+    @onpremises_group_type.setter
+    def onpremises_group_type(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__3784016360ceb15900b6f36bfc18d6bcf06c7629d554adf72514b0df0d5f2e42)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "onpremisesGroupType", value)
+
+    @builtins.property
     @jsii.member(jsii_name="owners")
     def owners(self) -> typing.List[builtins.str]:
         return typing.cast(typing.List[builtins.str], jsii.get(self, "owners"))
 
     @owners.setter
     def owners(self, value: typing.List[builtins.str]) -> None:
         if __debug__:
@@ -721,14 +759,31 @@
     @visibility.setter
     def visibility(self, value: builtins.str) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a6eee3d246ce0c9fadbcd29f564ef0f2d3667a88c0ea3fad2b9329729c71f344)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "visibility", value)
 
+    @builtins.property
+    @jsii.member(jsii_name="writebackEnabled")
+    def writeback_enabled(
+        self,
+    ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
+        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "writebackEnabled"))
+
+    @writeback_enabled.setter
+    def writeback_enabled(
+        self,
+        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__c3b37268e93f02d1bf64bc382309efb235f636ad3bf36e49197cd3c9550f0957)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "writebackEnabled", value)
+
 
 @jsii.data_type(
     jsii_type="@cdktf/provider-azuread.group.GroupConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
@@ -747,22 +802,24 @@
         "external_senders_allowed": "externalSendersAllowed",
         "hide_from_address_lists": "hideFromAddressLists",
         "hide_from_outlook_clients": "hideFromOutlookClients",
         "id": "id",
         "mail_enabled": "mailEnabled",
         "mail_nickname": "mailNickname",
         "members": "members",
+        "onpremises_group_type": "onpremisesGroupType",
         "owners": "owners",
         "prevent_duplicate_names": "preventDuplicateNames",
         "provisioning_options": "provisioningOptions",
         "security_enabled": "securityEnabled",
         "theme": "theme",
         "timeouts": "timeouts",
         "types": "types",
         "visibility": "visibility",
+        "writeback_enabled": "writebackEnabled",
     },
 )
 class GroupConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
@@ -782,22 +839,24 @@
         external_senders_allowed: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         hide_from_address_lists: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         hide_from_outlook_clients: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         id: typing.Optional[builtins.str] = None,
         mail_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         mail_nickname: typing.Optional[builtins.str] = None,
         members: typing.Optional[typing.Sequence[builtins.str]] = None,
+        onpremises_group_type: typing.Optional[builtins.str] = None,
         owners: typing.Optional[typing.Sequence[builtins.str]] = None,
         prevent_duplicate_names: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         provisioning_options: typing.Optional[typing.Sequence[builtins.str]] = None,
         security_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         theme: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["GroupTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         types: typing.Optional[typing.Sequence[builtins.str]] = None,
         visibility: typing.Optional[builtins.str] = None,
+        writeback_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
@@ -813,22 +872,24 @@
         :param external_senders_allowed: Indicates whether people external to the organization can send messages to the group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#external_senders_allowed Group#external_senders_allowed}
         :param hide_from_address_lists: Indicates whether the group is displayed in certain parts of the Outlook user interface: in the Address Book, in address lists for selecting message recipients, and in the Browse Groups dialog for searching groups. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#hide_from_address_lists Group#hide_from_address_lists}
         :param hide_from_outlook_clients: Indicates whether the group is displayed in Outlook clients, such as Outlook for Windows and Outlook on the web. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#hide_from_outlook_clients Group#hide_from_outlook_clients}
         :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#id Group#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param mail_enabled: Whether the group is a mail enabled, with a shared group mailbox. At least one of ``mail_enabled`` or ``security_enabled`` must be specified. A group can be mail enabled *and* security enabled Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#mail_enabled Group#mail_enabled}
         :param mail_nickname: The mail alias for the group, unique in the organisation. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#mail_nickname Group#mail_nickname}
         :param members: A set of members who should be present in this group. Supported object types are Users, Groups or Service Principals Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#members Group#members}
+        :param onpremises_group_type: Indicates the target on-premise group type the group will be written back as. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#onpremises_group_type Group#onpremises_group_type}
         :param owners: A set of owners who own this group. Supported object types are Users or Service Principals. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#owners Group#owners}
         :param prevent_duplicate_names: If ``true``, will return an error if an existing group is found with the same name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#prevent_duplicate_names Group#prevent_duplicate_names}
         :param provisioning_options: The group provisioning options for a Microsoft 365 group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#provisioning_options Group#provisioning_options}
         :param security_enabled: Whether the group is a security group for controlling access to in-app resources. At least one of ``security_enabled`` or ``mail_enabled`` must be specified. A group can be security enabled *and* mail enabled Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#security_enabled Group#security_enabled}
         :param theme: The colour theme for a Microsoft 365 group. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#theme Group#theme}
         :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#timeouts Group#timeouts}
         :param types: A set of group types to configure for the group. ``Unified`` specifies a Microsoft 365 group. Required when ``mail_enabled`` is true Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#types Group#types}
         :param visibility: Specifies the group join policy and group content visibility. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#visibility Group#visibility}
+        :param writeback_enabled: Whether this group should be synced from Azure AD to the on-premises directory when Azure AD Connect is used. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#writeback_enabled Group#writeback_enabled}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(dynamic_membership, dict):
             dynamic_membership = GroupDynamicMembership(**dynamic_membership)
         if isinstance(timeouts, dict):
             timeouts = GroupTimeouts(**timeouts)
@@ -851,22 +912,24 @@
             check_type(argname="argument external_senders_allowed", value=external_senders_allowed, expected_type=type_hints["external_senders_allowed"])
             check_type(argname="argument hide_from_address_lists", value=hide_from_address_lists, expected_type=type_hints["hide_from_address_lists"])
             check_type(argname="argument hide_from_outlook_clients", value=hide_from_outlook_clients, expected_type=type_hints["hide_from_outlook_clients"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument mail_enabled", value=mail_enabled, expected_type=type_hints["mail_enabled"])
             check_type(argname="argument mail_nickname", value=mail_nickname, expected_type=type_hints["mail_nickname"])
             check_type(argname="argument members", value=members, expected_type=type_hints["members"])
+            check_type(argname="argument onpremises_group_type", value=onpremises_group_type, expected_type=type_hints["onpremises_group_type"])
             check_type(argname="argument owners", value=owners, expected_type=type_hints["owners"])
             check_type(argname="argument prevent_duplicate_names", value=prevent_duplicate_names, expected_type=type_hints["prevent_duplicate_names"])
             check_type(argname="argument provisioning_options", value=provisioning_options, expected_type=type_hints["provisioning_options"])
             check_type(argname="argument security_enabled", value=security_enabled, expected_type=type_hints["security_enabled"])
             check_type(argname="argument theme", value=theme, expected_type=type_hints["theme"])
             check_type(argname="argument timeouts", value=timeouts, expected_type=type_hints["timeouts"])
             check_type(argname="argument types", value=types, expected_type=type_hints["types"])
             check_type(argname="argument visibility", value=visibility, expected_type=type_hints["visibility"])
+            check_type(argname="argument writeback_enabled", value=writeback_enabled, expected_type=type_hints["writeback_enabled"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "display_name": display_name,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
@@ -902,14 +965,16 @@
             self._values["id"] = id
         if mail_enabled is not None:
             self._values["mail_enabled"] = mail_enabled
         if mail_nickname is not None:
             self._values["mail_nickname"] = mail_nickname
         if members is not None:
             self._values["members"] = members
+        if onpremises_group_type is not None:
+            self._values["onpremises_group_type"] = onpremises_group_type
         if owners is not None:
             self._values["owners"] = owners
         if prevent_duplicate_names is not None:
             self._values["prevent_duplicate_names"] = prevent_duplicate_names
         if provisioning_options is not None:
             self._values["provisioning_options"] = provisioning_options
         if security_enabled is not None:
@@ -918,14 +983,16 @@
             self._values["theme"] = theme
         if timeouts is not None:
             self._values["timeouts"] = timeouts
         if types is not None:
             self._values["types"] = types
         if visibility is not None:
             self._values["visibility"] = visibility
+        if writeback_enabled is not None:
+            self._values["writeback_enabled"] = writeback_enabled
 
     @builtins.property
     def connection(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]]:
         '''
         :stability: experimental
@@ -1130,14 +1197,23 @@
 
         Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#members Group#members}
         '''
         result = self._values.get("members")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
+    def onpremises_group_type(self) -> typing.Optional[builtins.str]:
+        '''Indicates the target on-premise group type the group will be written back as.
+
+        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#onpremises_group_type Group#onpremises_group_type}
+        '''
+        result = self._values.get("onpremises_group_type")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def owners(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A set of owners who own this group. Supported object types are Users or Service Principals.
 
         Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#owners Group#owners}
         '''
         result = self._values.get("owners")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
@@ -1209,14 +1285,25 @@
         '''Specifies the group join policy and group content visibility.
 
         Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#visibility Group#visibility}
         '''
         result = self._values.get("visibility")
         return typing.cast(typing.Optional[builtins.str], result)
 
+    @builtins.property
+    def writeback_enabled(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        '''Whether this group should be synced from Azure AD to the on-premises directory when Azure AD Connect is used.
+
+        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/azuread/r/group#writeback_enabled Group#writeback_enabled}
+        '''
+        result = self._values.get("writeback_enabled")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -1575,22 +1662,24 @@
     external_senders_allowed: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     hide_from_address_lists: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     hide_from_outlook_clients: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     id: typing.Optional[builtins.str] = None,
     mail_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     mail_nickname: typing.Optional[builtins.str] = None,
     members: typing.Optional[typing.Sequence[builtins.str]] = None,
+    onpremises_group_type: typing.Optional[builtins.str] = None,
     owners: typing.Optional[typing.Sequence[builtins.str]] = None,
     prevent_duplicate_names: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     provisioning_options: typing.Optional[typing.Sequence[builtins.str]] = None,
     security_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     theme: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[GroupTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
     types: typing.Optional[typing.Sequence[builtins.str]] = None,
     visibility: typing.Optional[builtins.str] = None,
+    writeback_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[jsii.Number] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
@@ -1672,14 +1761,20 @@
 
 def _typecheckingstub__08b262a67fbb284a8d5b748d0d6b57e4862e547efaa86bbd5823d43a4e5a44d2(
     value: typing.List[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__3784016360ceb15900b6f36bfc18d6bcf06c7629d554adf72514b0df0d5f2e42(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__63991d9fcd1a9966b00b5ca504e2271c355d87bff16871c81cd20dba7a7f0e3c(
     value: typing.List[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__143e4ebfa2770d3cc5dc1556a57d6f7138760293b2f02985b42b946b7d09a8c7(
@@ -1714,14 +1809,20 @@
 
 def _typecheckingstub__a6eee3d246ce0c9fadbcd29f564ef0f2d3667a88c0ea3fad2b9329729c71f344(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__c3b37268e93f02d1bf64bc382309efb235f636ad3bf36e49197cd3c9550f0957(
+    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__47b7233356d26eaf49aa543fb81be0a3612fed53e3db84c23edb8b4664cf46e9(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[jsii.Number] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -1737,22 +1838,24 @@
     external_senders_allowed: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     hide_from_address_lists: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     hide_from_outlook_clients: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     id: typing.Optional[builtins.str] = None,
     mail_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     mail_nickname: typing.Optional[builtins.str] = None,
     members: typing.Optional[typing.Sequence[builtins.str]] = None,
+    onpremises_group_type: typing.Optional[builtins.str] = None,
     owners: typing.Optional[typing.Sequence[builtins.str]] = None,
     prevent_duplicate_names: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     provisioning_options: typing.Optional[typing.Sequence[builtins.str]] = None,
     security_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     theme: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[GroupTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
     types: typing.Optional[typing.Sequence[builtins.str]] = None,
     visibility: typing.Optional[builtins.str] = None,
+    writeback_enabled: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__5baeb9ccec25f32937fbf82a07c8ca7906b4e85dda0c59207893b6b6df2efc30(
     *,
     enabled: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
```

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/group_member/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/group_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/invitation/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/invitation/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/named_location/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/named_location/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/provider/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_certificate/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_password/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_password/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/synchronization_job/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/synchronization_job/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/synchronization_secret/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/synchronization_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread/user/__init__.py` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread/user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-azuread
-Version: 5.0.5
+Version: 6.0.0
 Summary: Prebuilt azuread Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-azuread.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-azuread.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cdktf-cdktf-provider-azuread-5.0.5/src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-azuread-6.0.0/src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,34 @@
 src/cdktf_cdktf_provider_azuread/py.typed
 src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_azuread.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_azuread.egg-info/requires.txt
 src/cdktf_cdktf_provider_azuread.egg-info/top_level.txt
 src/cdktf_cdktf_provider_azuread/_jsii/__init__.py
-src/cdktf_cdktf_provider_azuread/_jsii/provider-azuread@5.0.5.jsii.tgz
+src/cdktf_cdktf_provider_azuread/_jsii/provider-azuread@6.0.0.jsii.tgz
+src/cdktf_cdktf_provider_azuread/access_package/__init__.py
+src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/__init__.py
+src/cdktf_cdktf_provider_azuread/access_package_catalog/__init__.py
+src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/__init__.py
+src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/__init__.py
 src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py
 src/cdktf_cdktf_provider_azuread/administrative_unit_member/__init__.py
+src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/__init__.py
 src/cdktf_cdktf_provider_azuread/app_role_assignment/__init__.py
 src/cdktf_cdktf_provider_azuread/application/__init__.py
 src/cdktf_cdktf_provider_azuread/application_certificate/__init__.py
 src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/__init__.py
 src/cdktf_cdktf_provider_azuread/application_password/__init__.py
 src/cdktf_cdktf_provider_azuread/application_pre_authorized/__init__.py
 src/cdktf_cdktf_provider_azuread/claims_mapping_policy/__init__.py
 src/cdktf_cdktf_provider_azuread/conditional_access_policy/__init__.py
 src/cdktf_cdktf_provider_azuread/custom_directory_role/__init__.py
+src/cdktf_cdktf_provider_azuread/data_azuread_access_package/__init__.py
+src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/__init__.py
 src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/__init__.py
 src/cdktf_cdktf_provider_azuread/data_azuread_application/__init__.py
 src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/__init__.py
 src/cdktf_cdktf_provider_azuread/data_azuread_application_template/__init__.py
 src/cdktf_cdktf_provider_azuread/data_azuread_client_config/__init__.py
 src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/__init__.py
 src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/__init__.py
@@ -49,8 +57,9 @@
 src/cdktf_cdktf_provider_azuread/service_principal_certificate/__init__.py
 src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/__init__.py
 src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/__init__.py
 src/cdktf_cdktf_provider_azuread/service_principal_password/__init__.py
 src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/__init__.py
 src/cdktf_cdktf_provider_azuread/synchronization_job/__init__.py
 src/cdktf_cdktf_provider_azuread/synchronization_secret/__init__.py
-src/cdktf_cdktf_provider_azuread/user/__init__.py
+src/cdktf_cdktf_provider_azuread/user/__init__.py
+src/cdktf_cdktf_provider_azuread/user_flow_attribute/__init__.py
```

