# Comparing `tmp/cis_checks_2023-2.0.8.tar.gz` & `tmp/cis_checks_2023-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cis_checks_2023-2.0.8.tar", last modified: Fri Apr 14 06:07:13 2023, max compression
+gzip compressed data, was "cis_checks_2023-2.0.9.tar", last modified: Fri Apr 14 10:50:28 2023, max compression
```

## Comparing `cis_checks_2023-2.0.8.tar` & `cis_checks_2023-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 06:07:13.225733 cis_checks_2023-2.0.8/
--rw-rw-rw-   0        0        0      836 2023-04-14 06:07:13.224739 cis_checks_2023-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 cis_checks_2023-2.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 06:07:13.208806 cis_checks_2023-2.0.8/cis_checks_2023/
--rw-rw-rw-   0        0        0     7025 2023-04-14 06:00:10.000000 cis_checks_2023-2.0.8/cis_checks_2023/__init__.py
--rw-rw-rw-   0        0        0    35333 2023-04-07 14:21:10.000000 cis_checks_2023-2.0.8/cis_checks_2023/_security_control_5.py
--rw-rw-rw-   0        0        0    55484 2023-04-14 06:00:10.000000 cis_checks_2023-2.0.8/cis_checks_2023/iam_control_1.py
--rw-rw-rw-   0        0        0    25256 2023-04-13 06:34:22.000000 cis_checks_2023-2.0.8/cis_checks_2023/logging_control_3.py
--rw-rw-rw-   0        0        0    79813 2023-04-11 05:42:02.000000 cis_checks_2023-2.0.8/cis_checks_2023/monitoring_control_4.py
--rw-rw-rw-   0        0        0    25055 2023-04-11 07:00:11.000000 cis_checks_2023-2.0.8/cis_checks_2023/networking_control_5.py
--rw-rw-rw-   0        0        0    16019 2023-04-13 09:03:31.000000 cis_checks_2023-2.0.8/cis_checks_2023/storage_control_2.py
--rw-rw-rw-   0        0        0    21541 2023-04-13 07:03:52.000000 cis_checks_2023-2.0.8/cis_checks_2023/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 06:07:13.221752 cis_checks_2023-2.0.8/cis_checks_2023.egg-info/
--rw-rw-rw-   0        0        0      836 2023-04-14 06:07:13.000000 cis_checks_2023-2.0.8/cis_checks_2023.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-04-14 06:07:13.000000 cis_checks_2023-2.0.8/cis_checks_2023.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 06:07:13.000000 cis_checks_2023-2.0.8/cis_checks_2023.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-14 06:07:13.000000 cis_checks_2023-2.0.8/cis_checks_2023.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      557 2023-04-14 06:00:10.000000 cis_checks_2023-2.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 06:07:13.226730 cis_checks_2023-2.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 10:50:28.737119 cis_checks_2023-2.0.9/
+-rw-rw-rw-   0        0        0      836 2023-04-14 10:50:28.736120 cis_checks_2023-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 cis_checks_2023-2.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 10:50:28.712140 cis_checks_2023-2.0.9/cis_checks_2023/
+-rw-rw-rw-   0        0        0     6880 2023-04-14 10:49:28.000000 cis_checks_2023-2.0.9/cis_checks_2023/__init__.py
+-rw-rw-rw-   0        0        0    35333 2023-04-07 14:21:10.000000 cis_checks_2023-2.0.9/cis_checks_2023/_security_control_5.py
+-rw-rw-rw-   0        0        0    55484 2023-04-14 06:00:10.000000 cis_checks_2023-2.0.9/cis_checks_2023/iam_control_1.py
+-rw-rw-rw-   0        0        0    25256 2023-04-13 06:34:22.000000 cis_checks_2023-2.0.9/cis_checks_2023/logging_control_3.py
+-rw-rw-rw-   0        0        0    79813 2023-04-11 05:42:02.000000 cis_checks_2023-2.0.9/cis_checks_2023/monitoring_control_4.py
+-rw-rw-rw-   0        0        0    25055 2023-04-11 07:00:11.000000 cis_checks_2023-2.0.9/cis_checks_2023/networking_control_5.py
+-rw-rw-rw-   0        0        0    16019 2023-04-13 09:03:31.000000 cis_checks_2023-2.0.9/cis_checks_2023/storage_control_2.py
+-rw-rw-rw-   0        0        0    22117 2023-04-14 10:49:45.000000 cis_checks_2023-2.0.9/cis_checks_2023/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:50:28.732120 cis_checks_2023-2.0.9/cis_checks_2023.egg-info/
+-rw-rw-rw-   0        0        0      836 2023-04-14 10:50:28.000000 cis_checks_2023-2.0.9/cis_checks_2023.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-04-14 10:50:28.000000 cis_checks_2023-2.0.9/cis_checks_2023.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 10:50:28.000000 cis_checks_2023-2.0.9/cis_checks_2023.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-14 10:50:28.000000 cis_checks_2023-2.0.9/cis_checks_2023.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      557 2023-04-14 10:49:28.000000 cis_checks_2023-2.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 10:50:28.738119 cis_checks_2023-2.0.9/setup.cfg
```

### Comparing `cis_checks_2023-2.0.8/PKG-INFO` & `cis_checks_2023-2.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cis_checks_2023
-Version: 2.0.8
+Version: 2.0.9
 Summary: Provides AWS compliance details
 Author-email: Dheeraj Banodha <dheeraj.banodha@impetus.com>, Ravish Sharma <ravish.sharma@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cis_checks_2023-2.0.8/cis_checks_2023/__init__.py` & `cis_checks_2023-2.0.9/cis_checks_2023/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from cis_checks_2023.iam_control_1 import iam_control
 
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Dheeraj Banodha'
-__version__ = '2.0.8'
+__version__ = '2.0.9'
 
 
 class aws_client(iam_control, utils, storage_control, logging_control, monitoring_control, networking_control):
     def __init__(self, **kwargs):
         """
         @param str aws_access_key_id: AWS Access Key ID
         @param str aws_secret_access_key: AWS Secret Access Key
@@ -37,92 +37,94 @@
     def get_compliance(self) -> list:
         """
         :return list: consolidated list  of compliance.py checks
         """
         logger.info(" ---Inside get_compliance()")
 
         regions = self.get_regions()
+        if type(regions) is dict:
+            return [regions]
         CloudTrail = self.get_cloudtrails(regions)
         creds_report = self.get_cred_report()
         password_policy = self.get_account_password_policy()
         s3_buckets = self.list_s3_buckets()
         rds_instances = self.list_rds_instances(regions)
 
         compliance = [
             # iam_control_1
 
-            # self.control_1_01_maintain_contact_details(),
-            # self.control_1_02_security_contact_information_registered(),
-            # self.control_1_03_security_questions_registered(),
-            # self.control_1_04_root_key_exists(creds_report),
-            # self.control_1_05_root_mfa_enabled(),
-            # self.control_1_06_root_hardware_mfa_enabled(),
-            # self.control_1_07_root_use(creds_report),
-            # self.control_1_08_password_policy_length(password_policy),
-            # self.control_1_09_password_policy_reuse(password_policy),
-            # self.control_1_10_mfa_on_password_enabled_iam(creds_report),
-            # self.control_1_11_no_accesskey_on_initial_setup(creds_report),
-            # self.control_1_12_unused_credentials(creds_report),
-            # self.control_1_13_one_active_key(creds_report),
-            # self.control_1_14_ensure_access_keys_are_rotated_90_days(),
-            # self.control_1_15_no_policies_on_iam_users(),
+            self.control_1_01_maintain_contact_details(),
+            self.control_1_02_security_contact_information_registered(),
+            self.control_1_03_security_questions_registered(),
+            self.control_1_04_root_key_exists(creds_report),
+            self.control_1_05_root_mfa_enabled(),
+            self.control_1_06_root_hardware_mfa_enabled(),
+            self.control_1_07_root_use(creds_report),
+            self.control_1_08_password_policy_length(password_policy),
+            self.control_1_09_password_policy_reuse(password_policy),
+            self.control_1_10_mfa_on_password_enabled_iam(creds_report),
+            self.control_1_11_no_accesskey_on_initial_setup(creds_report),
+            self.control_1_12_unused_credentials(creds_report),
+            self.control_1_13_one_active_key(creds_report),
+            self.control_1_14_ensure_access_keys_are_rotated_90_days(),
+            self.control_1_15_no_policies_on_iam_users(),
             self.control_1_16_no_policies_with_full_administrative_privileges(),
-            # self.control_1_17_AWS_support_role_created(),
-            # self.control_1_18_iam_instance_role_for_access_from_instances(),
-            # self.control_1_19_expired_ssl_tls_certificates_removed(regions),
-            # self.control_1_2_iam_access_analyzer_enabled(regions),
-            # self.control_1_21_iam_user_managed_centrally(),
-            #
-            # # storage_control_2
-            #
-            # self.control_2_1_1_s3_default_encryption_at_rest(s3_buckets),
-            # self.control_2_1_2_s3_deny_http_requests(s3_buckets),
-            # self.control_2_1_3_s3_mfa_delete_enabled(s3_buckets),
-            # self.control_2_1_4_ensure_all_data_discovered_classified_secured(),
-            # self.control_2_1_5_s3_blocks_public_access(s3_buckets),
-            # self.control_2_2_1_ebs_volumes_encrypted(regions),
-            # self.control_2_3_1_rds_encryption_enabled(rds_instances),
-            # self.control_2_3_2_rds_auto_minor_version_upgrade_enabled(rds_instances),
-            # self.control_2_3_3_rds_publicly_accessible(rds_instances),
-            # self.control_2_4_1_encryption_enabled_for_efs(),
-            #
-            # # logging control 3
-            # self.control_3_01_ensure_cloud_trail_all_regions(CloudTrail),
-            # self.control_3_02_ensure_cloudtrail_validation(CloudTrail),
-            # self.control_3_03_ensure_cloudtrail_bucket_not_public(CloudTrail),
-            # self.control_3_04_ensure_cloudtrail_cloudwatch_logs_integration(CloudTrail),
-            # self.control_3_05_ensure_config_all_regions(regions),
-            # self.control_3_06_ensure_cloudtrail_bucket_logging(CloudTrail),
-            # self.control_3_07_ensure_cloudtrail_encryption_kms(CloudTrail),
-            # self.control_3_08_ensure_kms_cmk_rotation(regions),
-            # self.control_3_09_ensure_flow_logs_enabled_on_all_vpc(regions),
-            # self.control_3_1_ensure_logging_enabled_for_s3_write(regions),
-            # self.control_3_1_1_ensure_logging_enabled_for_s3_read(regions),
-            #
-            # # Monitoring_control_4
-            #
-            # self.control_4_0_1_ensure_log_metric_filter_unauthorized_api_calls(CloudTrail),
-            # self.control_4_0_2_ensure_log_metric_filter_console_signin_no_mfa(CloudTrail),
-            # self.control_4_0_3_ensure_log_metric_filter_root_usage(CloudTrail),
-            # self.control_4_0_4_ensure_log_metric_iam_policy_change(CloudTrail),
-            # self.control_4_0_5_ensure_log_metric_cloudtrail_configuration_changes(CloudTrail),
-            # self.control_4_0_6_ensure_log_metric_console_auth_failures(CloudTrail),
-            # self.control_4_0_7_ensure_log_metric_disabling_scheduled_delete_of_kms_cmk(CloudTrail),
-            # self.control_4_0_8_ensure_log_metric_s3_bucket_policy_changes(CloudTrail),
-            # self.control_4_0_9_ensure_log_metric_config_configuration_changes(CloudTrail),
-            # self.control_4_1_ensure_log_metric_security_group_changes(CloudTrail),
-            # self.control_4_11_ensure_log_metric_nacl(CloudTrail),
-            # self.control_4_12_ensure_log_metric_changes_to_network_gateways(CloudTrail),
-            # self.control_4_13_ensure_log_metric_changes_to_route_tables(CloudTrail),
-            # self.control_4_14_ensure_log_metric_changes_to_vpc(CloudTrail),
-            # self.control_4_15_ensure_log_metric_changes_to_org(CloudTrail),
-            # self.control_4_16_ensure_security_hub_is_enabled(regions),
-            #
-            # # networking control
-            # self.control_5_01_no_nacl_allow_ingress(regions),
-            # self.control_5_02_ensure_admin_ports_open_to_world_over_ipv4(regions),
-            # self.control_5_03_ensure_ports_open_to_world_over_ipv6(regions),
-            # self.control_5_04_ensure_default_security_groups_restricts_traffic(regions),
-            # self.control_5_05_ensure_route_tables_are_least_access(regions)
+            self.control_1_17_AWS_support_role_created(),
+            self.control_1_18_iam_instance_role_for_access_from_instances(),
+            self.control_1_19_expired_ssl_tls_certificates_removed(regions),
+            self.control_1_2_iam_access_analyzer_enabled(regions),
+            self.control_1_21_iam_user_managed_centrally(),
+
+            # storage_control_2
+
+            self.control_2_1_1_s3_default_encryption_at_rest(s3_buckets),
+            self.control_2_1_2_s3_deny_http_requests(s3_buckets),
+            self.control_2_1_3_s3_mfa_delete_enabled(s3_buckets),
+            self.control_2_1_4_ensure_all_data_discovered_classified_secured(),
+            self.control_2_1_5_s3_blocks_public_access(s3_buckets),
+            self.control_2_2_1_ebs_volumes_encrypted(regions),
+            self.control_2_3_1_rds_encryption_enabled(rds_instances),
+            self.control_2_3_2_rds_auto_minor_version_upgrade_enabled(rds_instances),
+            self.control_2_3_3_rds_publicly_accessible(rds_instances),
+            self.control_2_4_1_encryption_enabled_for_efs(),
+
+            # logging control 3
+            self.control_3_01_ensure_cloud_trail_all_regions(CloudTrail),
+            self.control_3_02_ensure_cloudtrail_validation(CloudTrail),
+            self.control_3_03_ensure_cloudtrail_bucket_not_public(CloudTrail),
+            self.control_3_04_ensure_cloudtrail_cloudwatch_logs_integration(CloudTrail),
+            self.control_3_05_ensure_config_all_regions(regions),
+            self.control_3_06_ensure_cloudtrail_bucket_logging(CloudTrail),
+            self.control_3_07_ensure_cloudtrail_encryption_kms(CloudTrail),
+            self.control_3_08_ensure_kms_cmk_rotation(regions),
+            self.control_3_09_ensure_flow_logs_enabled_on_all_vpc(regions),
+            self.control_3_1_ensure_logging_enabled_for_s3_write(regions),
+            self.control_3_1_1_ensure_logging_enabled_for_s3_read(regions),
+
+            # Monitoring_control_4
+
+            self.control_4_0_1_ensure_log_metric_filter_unauthorized_api_calls(CloudTrail),
+            self.control_4_0_2_ensure_log_metric_filter_console_signin_no_mfa(CloudTrail),
+            self.control_4_0_3_ensure_log_metric_filter_root_usage(CloudTrail),
+            self.control_4_0_4_ensure_log_metric_iam_policy_change(CloudTrail),
+            self.control_4_0_5_ensure_log_metric_cloudtrail_configuration_changes(CloudTrail),
+            self.control_4_0_6_ensure_log_metric_console_auth_failures(CloudTrail),
+            self.control_4_0_7_ensure_log_metric_disabling_scheduled_delete_of_kms_cmk(CloudTrail),
+            self.control_4_0_8_ensure_log_metric_s3_bucket_policy_changes(CloudTrail),
+            self.control_4_0_9_ensure_log_metric_config_configuration_changes(CloudTrail),
+            self.control_4_1_ensure_log_metric_security_group_changes(CloudTrail),
+            self.control_4_11_ensure_log_metric_nacl(CloudTrail),
+            self.control_4_12_ensure_log_metric_changes_to_network_gateways(CloudTrail),
+            self.control_4_13_ensure_log_metric_changes_to_route_tables(CloudTrail),
+            self.control_4_14_ensure_log_metric_changes_to_vpc(CloudTrail),
+            self.control_4_15_ensure_log_metric_changes_to_org(CloudTrail),
+            self.control_4_16_ensure_security_hub_is_enabled(regions),
+
+            # networking control
+            self.control_5_01_no_nacl_allow_ingress(regions),
+            self.control_5_02_ensure_admin_ports_open_to_world_over_ipv4(regions),
+            self.control_5_03_ensure_ports_open_to_world_over_ipv6(regions),
+            self.control_5_04_ensure_default_security_groups_restricts_traffic(regions),
+            self.control_5_05_ensure_route_tables_are_least_access(regions)
         ]
 
         return compliance
```

### Comparing `cis_checks_2023-2.0.8/cis_checks_2023/_security_control_5.py` & `cis_checks_2023-2.0.9/cis_checks_2023/_security_control_5.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.8/cis_checks_2023/iam_control_1.py` & `cis_checks_2023-2.0.9/cis_checks_2023/iam_control_1.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.8/cis_checks_2023/logging_control_3.py` & `cis_checks_2023-2.0.9/cis_checks_2023/logging_control_3.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.8/cis_checks_2023/monitoring_control_4.py` & `cis_checks_2023-2.0.9/cis_checks_2023/monitoring_control_4.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.8/cis_checks_2023/networking_control_5.py` & `cis_checks_2023-2.0.9/cis_checks_2023/networking_control_5.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.8/cis_checks_2023/storage_control_2.py` & `cis_checks_2023-2.0.9/cis_checks_2023/storage_control_2.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.8/cis_checks_2023/utils.py` & `cis_checks_2023-2.0.9/cis_checks_2023/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,18 +143,32 @@
         client = self.session.client('ec2', region_name='us-east-1')
         region_response = {}
         try:
             region_response = client.describe_regions()
         except botocore.exceptions.ClientError as error:
             if error.response['Error']['Code'] == 'AuthFailure':
                 logger.error(f" AccessKey credentails not found here: {error}")
-                exit(1)
+                return {
+                    'Result': 'Auth Failure',
+                    'failReason': 'Auth Failure',
+                    'Offenders': [],
+                    'ScoredControl': False,
+                    'Description': 'Auth Failure',
+                    'ControlId': 'Auth Failure'
+                }
         except botocore.exceptions.NoCredentialsError as e:
             logger.error(f" Unable to locate credentials: {e} ")
-            exit(1)
+            return {
+                'Result': 'Auth Failure',
+                'failReason': 'Auth Failure',
+                'Offenders': [],
+                'ScoredControl': False,
+                'Description': 'Auth Failure',
+                'ControlId': 'Auth Failure'
+            }
 
         logger.debug(region_response)
         regions = [region['RegionName'] for region in region_response['Regions']]
         return regions
 
     def get_cloudtrails(self, regions):
         logger.info(" ---Inside utils :: get_cloudtrails()--- ")
```

### Comparing `cis_checks_2023-2.0.8/cis_checks_2023.egg-info/PKG-INFO` & `cis_checks_2023-2.0.9/cis_checks_2023.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cis-checks-2023
-Version: 2.0.8
+Version: 2.0.9
 Summary: Provides AWS compliance details
 Author-email: Dheeraj Banodha <dheeraj.banodha@impetus.com>, Ravish Sharma <ravish.sharma@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cis_checks_2023-2.0.8/pyproject.toml` & `cis_checks_2023-2.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "cis_checks_2023"
-version = "2.0.8"
+version = "2.0.9"
 authors = [
   { name="Dheeraj Banodha", email="dheeraj.banodha@impetus.com" },
   { name="Ravish Sharma", email="ravish.sharma@impetus.com"}
 ]
 description = "Provides AWS compliance details"
 readme = "README.md"
 requires-python = ">=3.7"
```

