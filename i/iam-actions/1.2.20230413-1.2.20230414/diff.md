# Comparing `tmp/iam_actions-1.2.20230413.tar.gz` & `tmp/iam_actions-1.2.20230414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230413.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230414.tar", max compression
```

## Comparing `iam_actions-1.2.20230413.tar` & `iam_actions-1.2.20230414.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-13 02:24:37.848636 iam_actions-1.2.20230413/LICENSE
--rw-r--r--   0        0        0     2302 2023-04-13 02:24:37.848636 iam_actions-1.2.20230413/README.md
--rw-r--r--   0        0        0      228 2023-04-13 02:24:37.848636 iam_actions-1.2.20230413/iam_actions/__init__.py
--rw-r--r--   0        0        0  4204979 2023-04-13 02:26:01.851926 iam_actions-1.2.20230413/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-04-13 02:24:37.848636 iam_actions-1.2.20230413/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-04-13 02:24:37.852637 iam_actions-1.2.20230413/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-13 02:24:37.852637 iam_actions-1.2.20230413/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-04-13 02:24:37.852637 iam_actions-1.2.20230413/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-04-13 02:24:37.852637 iam_actions-1.2.20230413/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-04-13 02:24:37.852637 iam_actions-1.2.20230413/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-04-13 02:24:37.852637 iam_actions-1.2.20230413/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-04-13 02:24:37.852637 iam_actions-1.2.20230413/iam_actions/generate/services.py
--rw-r--r--   0        0        0   539604 2023-04-13 02:26:01.851926 iam_actions-1.2.20230413/iam_actions/policies.json
--rw-r--r--   0        0        0   190147 2023-04-13 02:26:01.851926 iam_actions-1.2.20230413/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   523256 2023-04-13 02:26:01.851926 iam_actions-1.2.20230413/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-04-13 02:26:02.903967 iam_actions-1.2.20230413/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230413/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230413/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/LICENSE
+-rw-r--r--   0        0        0     2302 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/README.md
+-rw-r--r--   0        0        0      228 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4208597 2023-04-14 02:25:53.397005 iam_actions-1.2.20230414/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   540398 2023-04-14 02:25:53.397005 iam_actions-1.2.20230414/iam_actions/policies.json
+-rw-r--r--   0        0        0   189864 2023-04-14 02:25:53.397005 iam_actions-1.2.20230414/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   524022 2023-04-14 02:25:53.397005 iam_actions-1.2.20230414/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-04-14 02:25:54.452994 iam_actions-1.2.20230414/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230414/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230414/PKG-INFO
```

### Comparing `iam_actions-1.2.20230413/LICENSE` & `iam_actions-1.2.20230414/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230413/README.md` & `iam_actions-1.2.20230414/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230413/iam_actions/actions.json` & `iam_actions-1.2.20230414/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990136457847754%*

 * *Differences: {"'groundstation'": "{'TagResource': {'resources': {insert: [(3, 'EphemerisItem')]}}, "*

 * *                    "'UntagResource': {'description': 'Grants permission to unassign a resource "*

 * *                    "tag', 'resources': {insert: [(3, 'EphemerisItem')]}}}",*

 * * "'inspector2'": "{'UpdateOrgEc2DeepInspectionConfiguration': OrderedDict([('access_level', "*

 * *                 "'Undocumented'), ('action', 'UpdateOrgEc2DeepInspectionConfiguration'), "*

 * *                 "('condition_keys', []), ('description', 'Not  […]*

```diff
@@ -68596,29 +68596,31 @@
             ],
             "description": "Grants permission to assign a resource tag",
             "orphan": false,
             "resources": [
                 "Config",
                 "Contact",
                 "DataflowEndpointGroup",
+                "EphemerisItem",
                 "MissionProfile"
             ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [
                 "aws:TagKeys"
             ],
-            "description": "Grants permission to deassign a resource tag",
+            "description": "Grants permission to unassign a resource tag",
             "orphan": false,
             "resources": [
                 "Config",
                 "Contact",
                 "DataflowEndpointGroup",
+                "EphemerisItem",
                 "MissionProfile"
             ]
         },
         "UpdateAgentStatus": {
             "access_level": "Write",
             "action": "UpdateAgentStatus",
             "condition_keys": [],
@@ -72631,14 +72633,30 @@
             "access_level": "Read",
             "action": "BatchGetFreeTrialInfo",
             "condition_keys": [],
             "description": "Grants permission to retrieve free trial period eligibility about Amazon Inspector accounts for an account",
             "orphan": false,
             "resources": []
         },
+        "BatchGetMemberEc2DeepInspectionStatus": {
+            "access_level": "Undocumented",
+            "action": "BatchGetMemberEc2DeepInspectionStatus",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "BatchUpdateMemberEc2DeepInspectionStatus": {
+            "access_level": "Undocumented",
+            "action": "BatchUpdateMemberEc2DeepInspectionStatus",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CancelFindingsReport": {
             "access_level": "Write",
             "action": "CancelFindingsReport",
             "condition_keys": [],
             "description": "Grants permission to cancel the generation of a findings report",
             "orphan": false,
             "resources": []
@@ -72734,14 +72752,22 @@
             "access_level": "Read",
             "action": "GetDelegatedAdminAccount",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the Amazon Inspector administrator account for an account",
             "orphan": false,
             "resources": []
         },
+        "GetEc2DeepInspectionConfiguration": {
+            "access_level": "Undocumented",
+            "action": "GetEc2DeepInspectionConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetFindingsReportStatus": {
             "access_level": "Read",
             "action": "GetFindingsReportStatus",
             "condition_keys": [],
             "description": "Grants permission to retrieve status for a requested findings report",
             "orphan": false,
             "resources": []
@@ -72860,27 +72886,43 @@
             "access_level": "Write",
             "action": "UpdateConfiguration",
             "condition_keys": [],
             "description": "Grants permission to update information about the Amazon Inspector configuration settings for an AWS account",
             "orphan": false,
             "resources": []
         },
+        "UpdateEc2DeepInspectionConfiguration": {
+            "access_level": "Undocumented",
+            "action": "UpdateEc2DeepInspectionConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateFilter": {
             "access_level": "Write",
             "action": "UpdateFilter",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to update the settings for a findings filter",
             "orphan": false,
             "resources": [
                 "Filter"
             ]
         },
+        "UpdateOrgEc2DeepInspectionConfiguration": {
+            "access_level": "Undocumented",
+            "action": "UpdateOrgEc2DeepInspectionConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateOrganizationConfiguration": {
             "access_level": "Write",
             "action": "UpdateOrganizationConfiguration",
             "condition_keys": [],
             "description": "Grants permission to update Amazon Inspector configuration settings for an AWS organization",
             "orphan": false,
             "resources": []
@@ -82270,288 +82312,242 @@
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesis": {
         "AddTagsToStream": {
-            "access_level": "Tagging",
+            "access_level": "Undocumented",
             "action": "AddTagsToStream",
             "condition_keys": [],
-            "description": "Grants permission to add or update tags for the specified Amazon Kinesis stream. Each stream can have up to 10 tags",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "CreateStream": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateStream",
             "condition_keys": [],
-            "description": "Grants permission to create a Amazon Kinesis stream",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "DecreaseStreamRetentionPeriod": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DecreaseStreamRetentionPeriod",
             "condition_keys": [],
-            "description": "Grants permission to decrease the stream's retention period, which is the length of time data records are accessible after they are added to the stream",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "DeleteStream": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteStream",
             "condition_keys": [],
-            "description": "Grants permission to delete a stream and all its shards and data",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "DeregisterStreamConsumer": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeregisterStreamConsumer",
             "condition_keys": [],
-            "description": "Grants permission to deregister a stream consumer with a Kinesis data stream",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "consumer"
-            ]
+            "resources": []
         },
         "DescribeLimits": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeLimits",
             "condition_keys": [],
-            "description": "Grants permission to describe the shard limits and usage for the account",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeStream": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeStream",
             "condition_keys": [],
-            "description": "Grants permission to describe the specified stream",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "DescribeStreamConsumer": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeStreamConsumer",
             "condition_keys": [],
-            "description": "Grants permission to get the description of a registered stream consumer",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "consumer"
-            ]
+            "resources": []
         },
         "DescribeStreamSummary": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeStreamSummary",
             "condition_keys": [],
-            "description": "Grants permission to provide a summarized description of the specified Kinesis data stream without the shard list",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "DisableEnhancedMonitoring": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisableEnhancedMonitoring",
             "condition_keys": [],
-            "description": "Grants permission to disables enhanced monitoring",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "EnableEnhancedMonitoring": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "EnableEnhancedMonitoring",
             "condition_keys": [],
-            "description": "Grants permission to enable enhanced Kinesis data stream monitoring for shard-level metrics",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetRecords": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetRecords",
             "condition_keys": [],
-            "description": "Grants permission to get data records from a shard",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "GetShardIterator": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetShardIterator",
             "condition_keys": [],
-            "description": "Grants permission to get a shard iterator. A shard iterator expires five minutes after it is returned to the requester",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "IncreaseStreamRetentionPeriod": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "IncreaseStreamRetentionPeriod",
             "condition_keys": [],
-            "description": "Grants permission to increase the stream's retention period, which is the length of time data records are accessible after they are added to the stream",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "ListShards": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListShards",
             "condition_keys": [],
-            "description": "Grants permission to list the shards in a stream and provides information about each shard",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListStreamConsumers": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListStreamConsumers",
             "condition_keys": [],
-            "description": "Grants permission to list the stream consumers registered to receive data from a Kinesis stream using enhanced fan-out, and provides information about each consumer",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "ListStreams": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListStreams",
             "condition_keys": [],
-            "description": "Grants permission to list your streams",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForStream": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ListTagsForStream",
             "condition_keys": [],
-            "description": "Grants permission to list the tags for the specified Amazon Kinesis stream",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "MergeShards": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "MergeShards",
             "condition_keys": [],
-            "description": "Grants permission to merge two adjacent shards in a stream and combines them into a single shard to reduce the stream's capacity to ingest and transport data",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "PutRecord": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "PutRecord",
             "condition_keys": [],
-            "description": "Grants permission to write a single data record from a producer into an Amazon Kinesis stream",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "PutRecords": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "PutRecords",
             "condition_keys": [],
-            "description": "Grants permission to write multiple data records from a producer into an Amazon Kinesis stream in a single call (also referred to as a PutRecords request)",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "RegisterStreamConsumer": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RegisterStreamConsumer",
             "condition_keys": [],
-            "description": "Grants permission to register a stream consumer with a Kinesis data stream",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "RemoveTagsFromStream": {
-            "access_level": "Tagging",
+            "access_level": "Undocumented",
             "action": "RemoveTagsFromStream",
             "condition_keys": [],
-            "description": "Grants permission to remove tags from the specified Kinesis data stream. Removed tags are deleted and cannot be recovered after this operation successfully completes",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "SplitShard": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "SplitShard",
             "condition_keys": [],
-            "description": "Grants permission to split a shard into two new shards in the Kinesis data stream, to increase the stream's capacity to ingest and transport data",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "stream"
-            ]
+            "resources": []
         },
         "StartStreamEncryption": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StartStreamEncryption",
             "condition_keys": [],
-            "description": "Grants permission to enable or update server-side encryption using an AWS KMS key for a specified stream",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "kmsKey",
-                "stream"
-            ]
+            "resources": []
         },
         "StopStreamEncryption": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "StopStreamEncryption",
             "condition_keys": [],
-            "description": "Grants permission to disable server-side encryption for a specified stream",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "kmsKey",
-                "stream"
-            ]
+            "resources": []
         },
         "SubscribeToShard": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "SubscribeToShard",
             "condition_keys": [],
-            "description": "Grants permission to listen to a specific shard with enhanced fan-out",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "consumer"
-            ]
+            "resources": []
         },
         "UpdateShardCount": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateShardCount",
             "condition_keys": [],
-            "description": "Grants permission to update the shard count of the specified stream to the specified number of shards",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateStreamMode": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateStreamMode",
             "condition_keys": [],
-            "description": "Grants permission to update the capacity mode of the data stream",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesisanalytics": {
         "AddApplicationCloudWatchLoggingOption": {
             "access_level": "Write",
@@ -91883,14 +91879,30 @@
             "condition_keys": [],
             "description": "The UpdateQualificationType operation modifies the attributes of an existing Qualification type, which is represented by a QualificationType data structure",
             "orphan": false,
             "resources": []
         }
     },
     "mediaconnect": {
+        "AddBridgeOutputs": {
+            "access_level": "Undocumented",
+            "action": "AddBridgeOutputs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "AddBridgeSources": {
+            "access_level": "Undocumented",
+            "action": "AddBridgeSources",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "AddFlowMediaStreams": {
             "access_level": "Write",
             "action": "AddFlowMediaStreams",
             "condition_keys": [],
             "description": "Grants permission to add media streams to any flow",
             "orphan": false,
             "resources": []
@@ -91915,38 +91927,102 @@
             "access_level": "Write",
             "action": "AddFlowVpcInterfaces",
             "condition_keys": [],
             "description": "Grants permission to add VPC interfaces to any flow",
             "orphan": false,
             "resources": []
         },
+        "CreateBridge": {
+            "access_level": "Undocumented",
+            "action": "CreateBridge",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateFlow": {
             "access_level": "Write",
             "action": "CreateFlow",
             "condition_keys": [],
             "description": "Grants permission to create flows",
             "orphan": false,
             "resources": []
         },
+        "CreateGateway": {
+            "access_level": "Undocumented",
+            "action": "CreateGateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteBridge": {
+            "access_level": "Undocumented",
+            "action": "DeleteBridge",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteFlow": {
             "access_level": "Write",
             "action": "DeleteFlow",
             "condition_keys": [],
             "description": "Grants permission to delete flows",
             "orphan": false,
             "resources": []
         },
+        "DeleteGateway": {
+            "access_level": "Undocumented",
+            "action": "DeleteGateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeregisterGatewayInstance": {
+            "access_level": "Undocumented",
+            "action": "DeregisterGatewayInstance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeBridge": {
+            "access_level": "Undocumented",
+            "action": "DescribeBridge",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeFlow": {
             "access_level": "Read",
             "action": "DescribeFlow",
             "condition_keys": [],
             "description": "Grants permission to display the details of a flow including the flow ARN, name, and Availability Zone, as well as details about the source, outputs, and entitlements",
             "orphan": false,
             "resources": []
         },
+        "DescribeGateway": {
+            "access_level": "Undocumented",
+            "action": "DescribeGateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeGatewayInstance": {
+            "access_level": "Undocumented",
+            "action": "DescribeGatewayInstance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeOffering": {
             "access_level": "Read",
             "action": "DescribeOffering",
             "condition_keys": [],
             "description": "Grants permission to display the details of an offering",
             "orphan": false,
             "resources": []
@@ -91955,22 +92031,38 @@
             "access_level": "Read",
             "action": "DescribeReservation",
             "condition_keys": [],
             "description": "Grants permission to display the details of a reservation",
             "orphan": false,
             "resources": []
         },
+        "DiscoverGatewayPollEndpoint": {
+            "access_level": "Undocumented",
+            "action": "DiscoverGatewayPollEndpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GrantFlowEntitlements": {
             "access_level": "Write",
             "action": "GrantFlowEntitlements",
             "condition_keys": [],
             "description": "Grants permission to grant entitlements on any flow",
             "orphan": false,
             "resources": []
         },
+        "ListBridges": {
+            "access_level": "Undocumented",
+            "action": "ListBridges",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListEntitlements": {
             "access_level": "List",
             "action": "ListEntitlements",
             "condition_keys": [],
             "description": "Grants permission to display a list of all entitlements that have been granted to the account",
             "orphan": false,
             "resources": []
@@ -91979,14 +92071,30 @@
             "access_level": "List",
             "action": "ListFlows",
             "condition_keys": [],
             "description": "Grants permission to display a list of flows that are associated with this account",
             "orphan": false,
             "resources": []
         },
+        "ListGatewayInstances": {
+            "access_level": "Undocumented",
+            "action": "ListGatewayInstances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListGateways": {
+            "access_level": "Undocumented",
+            "action": "ListGateways",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListOfferings": {
             "access_level": "List",
             "action": "ListOfferings",
             "condition_keys": [],
             "description": "Grants permission to display a list of all offerings that are available to the account in the current AWS Region",
             "orphan": false,
             "resources": []
@@ -92003,22 +92111,46 @@
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to display a list of all tags associated with a resource",
             "orphan": false,
             "resources": []
         },
+        "PollGateway": {
+            "access_level": "Undocumented",
+            "action": "PollGateway",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "PurchaseOffering": {
             "access_level": "Write",
             "action": "PurchaseOffering",
             "condition_keys": [],
             "description": "Grants permission to purchase an offering",
             "orphan": false,
             "resources": []
         },
+        "RemoveBridgeOutput": {
+            "access_level": "Undocumented",
+            "action": "RemoveBridgeOutput",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "RemoveBridgeSource": {
+            "access_level": "Undocumented",
+            "action": "RemoveBridgeSource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "RemoveFlowMediaStream": {
             "access_level": "Write",
             "action": "RemoveFlowMediaStream",
             "condition_keys": [],
             "description": "Grants permission to remove media streams from any flow",
             "orphan": false,
             "resources": []
@@ -92067,14 +92199,22 @@
             "access_level": "Write",
             "action": "StopFlow",
             "condition_keys": [],
             "description": "Grants permission to stop flows",
             "orphan": false,
             "resources": []
         },
+        "SubmitGatewayStateChange": {
+            "access_level": "Undocumented",
+            "action": "SubmitGatewayStateChange",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Grants permission to associate tags with resources",
             "orphan": false,
             "resources": []
@@ -92083,14 +92223,46 @@
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [],
             "description": "Grants permission to remove tags from resources",
             "orphan": false,
             "resources": []
         },
+        "UpdateBridge": {
+            "access_level": "Undocumented",
+            "action": "UpdateBridge",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateBridgeOutput": {
+            "access_level": "Undocumented",
+            "action": "UpdateBridgeOutput",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateBridgeSource": {
+            "access_level": "Undocumented",
+            "action": "UpdateBridgeSource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateBridgeState": {
+            "access_level": "Undocumented",
+            "action": "UpdateBridgeState",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateFlow": {
             "access_level": "Write",
             "action": "UpdateFlow",
             "condition_keys": [],
             "description": "Grants permission to update flows",
             "orphan": false,
             "resources": []
@@ -135678,14 +135850,22 @@
             "condition_keys": [],
             "description": "Grants permission to list all receipts of a page",
             "orphan": false,
             "resources": [
                 "page"
             ]
         },
+        "ListPageResolutions": {
+            "access_level": "Undocumented",
+            "action": "ListPageResolutions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListPagesByContact": {
             "access_level": "List",
             "action": "ListPagesByContact",
             "condition_keys": [],
             "description": "Grants permission to list all pages sent to a contact",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20230413/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230414/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230413/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230414/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230413/iam_actions/generate/generate.py` & `iam_actions-1.2.20230414/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230413/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230414/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230413/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230414/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230413/iam_actions/generate/services.py` & `iam_actions-1.2.20230414/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230413/iam_actions/policies.json` & `iam_actions-1.2.20230414/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999790059543349%*

 * *Differences: {"'serviceMap'": "{'AWS Elemental MediaConnect': {'Actions': {insert: [(0, 'AddBridgeOutputs'), "*

 * *                 "(1, 'AddBridgeSources'), (6, 'CreateBridge'), (8, 'CreateGateway'), (9, "*

 * *                 "'DeleteBridge'), (11, 'DeleteGateway'), (12, 'DeregisterGatewayInstance'), (13, "*

 * *                 "'DescribeBridge'), (15, 'DescribeGateway'), (16, 'DescribeGatewayInstance'), "*

 * *                 "(19, 'DiscoverGatewayPollEndpoint'), (21, 'ListBridges'), (24, "*

 * *                 "'ListGatewayInstances'), […]*

```diff
@@ -3337,42 +3337,64 @@
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
         "AWS Elemental MediaConnect": {
-            "ARNFormat": "arn:aws:mediaconnect:${Region}:${Account}:<namespace>:<relative-id>:<relative-name>",
+            "ARNFormat": "arn:aws:mediaconnect:${Region}:${Account}:${Namespace}:${RelativeId}:${RelativeName}",
             "ARNRegex": "^arn:aws:mediaconnect:.+",
             "Actions": [
+                "AddBridgeOutputs",
+                "AddBridgeSources",
                 "AddFlowMediaStreams",
                 "AddFlowOutputs",
                 "AddFlowSources",
                 "AddFlowVpcInterfaces",
+                "CreateBridge",
                 "CreateFlow",
+                "CreateGateway",
+                "DeleteBridge",
                 "DeleteFlow",
+                "DeleteGateway",
+                "DeregisterGatewayInstance",
+                "DescribeBridge",
                 "DescribeFlow",
+                "DescribeGateway",
+                "DescribeGatewayInstance",
                 "DescribeOffering",
                 "DescribeReservation",
+                "DiscoverGatewayPollEndpoint",
                 "GrantFlowEntitlements",
+                "ListBridges",
                 "ListEntitlements",
                 "ListFlows",
+                "ListGatewayInstances",
+                "ListGateways",
                 "ListOfferings",
                 "ListReservations",
                 "ListTagsForResource",
+                "PollGateway",
                 "PurchaseOffering",
+                "RemoveBridgeOutput",
+                "RemoveBridgeSource",
                 "RemoveFlowMediaStream",
                 "RemoveFlowOutput",
                 "RemoveFlowSource",
                 "RemoveFlowVpcInterface",
                 "RevokeFlowEntitlement",
                 "StartFlow",
                 "StopFlow",
+                "SubmitGatewayStateChange",
                 "TagResource",
                 "UntagResource",
+                "UpdateBridge",
+                "UpdateBridgeOutput",
+                "UpdateBridgeSource",
+                "UpdateBridgeState",
                 "UpdateFlow",
                 "UpdateFlowEntitlement",
                 "UpdateFlowMediaStream",
                 "UpdateFlowOutput",
                 "UpdateFlowSource"
             ],
             "HasResource": true,
@@ -8607,14 +8629,15 @@
                 "GetContactPolicy",
                 "GetRotation",
                 "GetRotationOverride",
                 "ListContactChannels",
                 "ListContacts",
                 "ListEngagements",
                 "ListPageReceipts",
+                "ListPageResolutions",
                 "ListPagesByContact",
                 "ListPagesByEngagement",
                 "ListPreviewRotationShifts",
                 "ListRotationOverrides",
                 "ListRotationShifts",
                 "ListRotations",
                 "ListTagsForResource",
@@ -14094,26 +14117,29 @@
             "ARNFormat": "arn:aws:inspector2:${Region}:${Account}:.+",
             "ARNRegex": "^arn:aws:inspector2:.+:.+:.+",
             "Actions": [
                 "AssociateMember",
                 "BatchGetAccountStatus",
                 "BatchGetCodeSnippet",
                 "BatchGetFreeTrialInfo",
+                "BatchGetMemberEc2DeepInspectionStatus",
+                "BatchUpdateMemberEc2DeepInspectionStatus",
                 "CancelFindingsReport",
                 "CreateFilter",
                 "CreateFindingsReport",
                 "DeleteFilter",
                 "DescribeOrganizationConfiguration",
                 "Disable",
                 "DisableDelegatedAdminAccount",
                 "DisassociateMember",
                 "Enable",
                 "EnableDelegatedAdminAccount",
                 "GetConfiguration",
                 "GetDelegatedAdminAccount",
+                "GetEc2DeepInspectionConfiguration",
                 "GetFindingsReportStatus",
                 "GetMember",
                 "ListAccountPermissions",
                 "ListCoverage",
                 "ListCoverageStatistics",
                 "ListDelegatedAdminAccounts",
                 "ListFilters",
@@ -14121,15 +14147,17 @@
                 "ListFindings",
                 "ListMembers",
                 "ListTagsForResource",
                 "ListUsageTotals",
                 "TagResource",
                 "UntagResource",
                 "UpdateConfiguration",
+                "UpdateEc2DeepInspectionConfiguration",
                 "UpdateFilter",
+                "UpdateOrgEc2DeepInspectionConfiguration",
                 "UpdateOrganizationConfiguration"
             ],
             "HasResource": true,
             "StringPrefix": "inspector2",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
```

### Comparing `iam_actions-1.2.20230413/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230414/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985835694050992%*

 * *Differences: {"'kinesis'": '{replace: OrderedDict()}'}*

```diff
@@ -3687,28 +3687,15 @@
         },
         "thesaurus": {
             "arn_pattern": "arn:*:kendra:*:*:index/*/thesaurus/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "kendra-ranking": {},
-    "kinesis": {
-        "consumer": {
-            "arn_pattern": "arn:*:kinesis:*:*:*/*/consumer/*:*",
-            "condition_keys": null
-        },
-        "kmsKey": {
-            "arn_pattern": "arn:*:kms:*:*:key/*",
-            "condition_keys": null
-        },
-        "stream": {
-            "arn_pattern": "arn:*:kinesis:*:*:stream/*",
-            "condition_keys": null
-        }
-    },
+    "kinesis": {},
     "kinesisanalytics": {
         "application": {
             "arn_pattern": "arn:*:kinesisanalytics:*:*:application/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "kinesisvideo": {
```

### Comparing `iam_actions-1.2.20230413/iam_actions/services.json` & `iam_actions-1.2.20230414/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998135439246404%*

 * *Differences: {"'inspector2'": "{'Actions': {insert: [(4, 'BatchGetMemberEc2DeepInspectionStatus'), (5, "*

 * *                 "'BatchUpdateMemberEc2DeepInspectionStatus'), (18, "*

 * *                 "'GetEc2DeepInspectionConfiguration'), (34, "*

 * *                 "'UpdateEc2DeepInspectionConfiguration'), (36, "*

 * *                 "'UpdateOrgEc2DeepInspectionConfiguration')]}}",*

 * * "'mediaconnect'": "{'Actions': {insert: [(0, 'AddBridgeOutputs'), (1, 'AddBridgeSources'), (6, "*

 * *                   "'CreateBridge'), (8, 'CreateGateway') […]*

```diff
@@ -10043,26 +10043,29 @@
             "^arn:aws:inspector2:.+:.+:.+"
         ],
         "Actions": [
             "AssociateMember",
             "BatchGetAccountStatus",
             "BatchGetCodeSnippet",
             "BatchGetFreeTrialInfo",
+            "BatchGetMemberEc2DeepInspectionStatus",
+            "BatchUpdateMemberEc2DeepInspectionStatus",
             "CancelFindingsReport",
             "CreateFilter",
             "CreateFindingsReport",
             "DeleteFilter",
             "DescribeOrganizationConfiguration",
             "Disable",
             "DisableDelegatedAdminAccount",
             "DisassociateMember",
             "Enable",
             "EnableDelegatedAdminAccount",
             "GetConfiguration",
             "GetDelegatedAdminAccount",
+            "GetEc2DeepInspectionConfiguration",
             "GetFindingsReportStatus",
             "GetMember",
             "ListAccountPermissions",
             "ListCoverage",
             "ListCoverageStatistics",
             "ListDelegatedAdminAccounts",
             "ListFilters",
@@ -10070,15 +10073,17 @@
             "ListFindings",
             "ListMembers",
             "ListTagsForResource",
             "ListUsageTotals",
             "TagResource",
             "UntagResource",
             "UpdateConfiguration",
+            "UpdateEc2DeepInspectionConfiguration",
             "UpdateFilter",
+            "UpdateOrgEc2DeepInspectionConfiguration",
             "UpdateOrganizationConfiguration"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
         ],
@@ -12856,45 +12861,67 @@
         "HasResource": false,
         "ServiceNames": [
             "Amazon Mechanical Turk"
         ]
     },
     "mediaconnect": {
         "ARNFormats": [
-            "arn:aws:mediaconnect:${Region}:${Account}:<namespace>:<relative-id>:<relative-name>"
+            "arn:aws:mediaconnect:${Region}:${Account}:${Namespace}:${RelativeId}:${RelativeName}"
         ],
         "ARNRegexes": [
             "^arn:aws:mediaconnect:.+"
         ],
         "Actions": [
+            "AddBridgeOutputs",
+            "AddBridgeSources",
             "AddFlowMediaStreams",
             "AddFlowOutputs",
             "AddFlowSources",
             "AddFlowVpcInterfaces",
+            "CreateBridge",
             "CreateFlow",
+            "CreateGateway",
+            "DeleteBridge",
             "DeleteFlow",
+            "DeleteGateway",
+            "DeregisterGatewayInstance",
+            "DescribeBridge",
             "DescribeFlow",
+            "DescribeGateway",
+            "DescribeGatewayInstance",
             "DescribeOffering",
             "DescribeReservation",
+            "DiscoverGatewayPollEndpoint",
             "GrantFlowEntitlements",
+            "ListBridges",
             "ListEntitlements",
             "ListFlows",
+            "ListGatewayInstances",
+            "ListGateways",
             "ListOfferings",
             "ListReservations",
             "ListTagsForResource",
+            "PollGateway",
             "PurchaseOffering",
+            "RemoveBridgeOutput",
+            "RemoveBridgeSource",
             "RemoveFlowMediaStream",
             "RemoveFlowOutput",
             "RemoveFlowSource",
             "RemoveFlowVpcInterface",
             "RevokeFlowEntitlement",
             "StartFlow",
             "StopFlow",
+            "SubmitGatewayStateChange",
             "TagResource",
             "UntagResource",
+            "UpdateBridge",
+            "UpdateBridgeOutput",
+            "UpdateBridgeSource",
+            "UpdateBridgeState",
             "UpdateFlow",
             "UpdateFlowEntitlement",
             "UpdateFlowMediaStream",
             "UpdateFlowOutput",
             "UpdateFlowSource"
         ],
         "ConditionKeys": [],
@@ -18832,14 +18859,15 @@
             "GetContactPolicy",
             "GetRotation",
             "GetRotationOverride",
             "ListContactChannels",
             "ListContacts",
             "ListEngagements",
             "ListPageReceipts",
+            "ListPageResolutions",
             "ListPagesByContact",
             "ListPagesByEngagement",
             "ListPreviewRotationShifts",
             "ListRotationOverrides",
             "ListRotationShifts",
             "ListRotations",
             "ListTagsForResource",
```

### Comparing `iam_actions-1.2.20230413/pyproject.toml` & `iam_actions-1.2.20230414/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230413"
+version = "1.2.20230414"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230413/setup.py` & `iam_actions-1.2.20230414/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230413',
+    'version': '1.2.20230414',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230413/PKG-INFO` & `iam_actions-1.2.20230414/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230413
+Version: 1.2.20230414
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

