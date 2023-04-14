# Comparing `tmp/aliyun-python-sdk-airec-2.0.1.tar.gz` & `tmp/aliyun-python-sdk-airec-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-airec-2.0.1.tar", last modified: Tue Mar 30 10:23:30 2021, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-airec-2.1.0.tar", last modified: Fri Apr 14 08:44:16 2023, max compression
```

## Comparing `aliyun-python-sdk-airec-2.0.1.tar` & `aliyun-python-sdk-airec-2.1.0.tar`

### file list

```diff
@@ -1,106 +1,166 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 10:23:30.000000 aliyun-python-sdk-airec-2.0.1/
--rw-r--r--   0 root         (0) root         (0)      575 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1547 2021-03-30 10:23:30.000000 aliyun-python-sdk-airec-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      531 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyun_python_sdk_airec.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1547 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyun_python_sdk_airec.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5688 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyun_python_sdk_airec.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyun_python_sdk_airec.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyun_python_sdk_airec.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyun_python_sdk_airec.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/
--rw-r--r--   0 root         (0) root         (0)       21 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/
--rw-r--r--   0 root         (0) root         (0)        0 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-30 10:23:30.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/
--rw-r--r--   0 root         (0) root         (0)     1703 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/AttachDatasetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1929 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/AttachIndexVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1780 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/CheckRankingModelReachableRequest.py
--rw-r--r--   0 root         (0) root         (0)     2046 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/CloneExperimentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1693 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/CreateFilteringAlgorithmRequest.py
--rw-r--r--   0 root         (0) root         (0)     1321 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/CreateInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1675 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/CreateRankingModelRequest.py
--rw-r--r--   0 root         (0) root         (0)     1502 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/CreateRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1653 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/CreateSceneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1739 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DecribeRankingModelRequest.py
--rw-r--r--   0 root         (0) root         (0)     1689 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DeleteDataSetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1888 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DeleteExperimentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1737 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DeleteFilteringAlgorithmRequest.py
--rw-r--r--   0 root         (0) root         (0)     1740 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DeleteRankingModelRequest.py
--rw-r--r--   0 root         (0) root         (0)     1669 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DeleteSceneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1704 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeBaseExperimentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1713 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeDataSetMessageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1713 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeDefaultAlgorithmsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1722 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeExperimentEnvProgressRequest.py
--rw-r--r--   0 root         (0) root         (0)     1701 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeExperimentEnvRequest.py
--rw-r--r--   0 root         (0) root         (0)     1889 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeExperimentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1738 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeFilteringAlgorithmRequest.py
--rw-r--r--   0 root         (0) root         (0)     1507 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1735 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeLatestTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1507 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeQuotaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1531 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1974 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1700 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeSceneBucketRequest.py
--rw-r--r--   0 root         (0) root         (0)     1670 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeSceneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1701 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeSceneThroughputRequest.py
--rw-r--r--   0 root         (0) root         (0)     2165 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeSyncReportDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2301 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeSyncReportOutliersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2013 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeUserMetricsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1528 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DowngradeInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1703 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/EnableExperimentRequest.py
--rw-r--r--   0 root         (0) root         (0)     2551 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListDashboardDetailsFlowsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2535 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListDashboardDetailsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2041 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListDashboardMetricsFlowsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2025 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListDashboardMetricsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1506 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListDataSetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1515 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListDataSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1686 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListExperimentsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2140 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListFilteringAlgorithmsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1735 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListIndexVersionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2222 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1513 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListInstanceTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1785 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListItemsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2266 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1345 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListMixCategoriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1992 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListRankingModelsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1527 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListRuleConditionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListRuleTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2553 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2704 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListSceneItemsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1540 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListSceneParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2076 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListScenesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1328 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListUmengAppkeysRequest.py
--rw-r--r--   0 root         (0) root         (0)     1521 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListUserClustersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1695 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ModifyDataSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1747 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ModifyFilteringAlgorithmMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1503 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ModifyInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1504 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ModifyItemsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1737 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ModifyRankingModelRequest.py
--rw-r--r--   0 root         (0) root         (0)     1656 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ModifyRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ModifySceneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1753 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/OfflineFilteringAlgorithmRequest.py
--rw-r--r--   0 root         (0) root         (0)     1988 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/PublishRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1696 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/PushDocumentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1526 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/PushInterventionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3689 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/QueryDataMessageRequest.py
--rw-r--r--   0 root         (0) root         (0)     3448 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/QueryDataMessageStatisticsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2004 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/QueryExceptionHistoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2279 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/QueryRawDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1570 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/QuerySingleAggregationReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1708 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/QuerySingleReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1872 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/QuerySyncReportAggregationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1727 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/RebuildIndexRequest.py
--rw-r--r--   0 root         (0) root         (0)     2731 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/RecommendRequest.py
--rw-r--r--   0 root         (0) root         (0)     1513 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/RunInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1696 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/StopDataSetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1738 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/UnLockIndexVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1909 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/UpdateExperimentBasicInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1904 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/UpdateExperimentConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1904 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/UpdateExperimentStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1522 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/UpgradeInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1525 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ValidateInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-03-30 10:23:30.000000 aliyun-python-sdk-airec-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2462 2021-03-30 10:23:29.000000 aliyun-python-sdk-airec-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      531 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyun_python_sdk_airec.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyun_python_sdk_airec.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9582 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyun_python_sdk_airec.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyun_python_sdk_airec.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyun_python_sdk_airec.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyun_python_sdk_airec.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/AttachDatasetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1990 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/AttachIndexVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CheckRankingModelReachableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CloneExperimentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CloneSampleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ColdStartRankRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateCustomAnalysisTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateCustomSampleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateDataDiagnoseTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateExtraDataSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateFilteringAlgorithmRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateFlowControlTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateRankingModelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateRankingModelTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateRankingSystemRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateSampleFormatConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateSceneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateUmengTokenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DecribeRankingModelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteDataSetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteExperimentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteExtraDataSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteFilteringAlgorithmRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteFlowControlTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteRankingModelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteRankingModelTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteRankingModelVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteRankingSystemRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteSampleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteSceneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeployRankingSystemRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeBaseExperimentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeCustomAnalysisTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeDataSetMessageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeDefaultAlgorithmsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeExperimentEnvProgressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeExperimentEnvRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeExperimentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeFilteringAlgorithmRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeLatestTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeQuotaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeSceneBucketRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeSceneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeSceneThroughputRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeSyncReportDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2411 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeSyncReportOutliersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeUserMetricsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DowngradeInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/EnableExperimentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/GenerateSampleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/GetExtraDataSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/GetFlowControlTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/GetLatestDataDiagnoseTaskStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/GetRankingModelTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/GetRankingModelVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/GetRankingSystemHistoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/GetRankingSystemRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/GetSampleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/InitComputingResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListDashboardDetailsFlowsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListDashboardDetailsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListDashboardMetricsFlowsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListDashboardMetricsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListDataDiagnoseReportsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListDataDiagnoseSampleDetailsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListDataSetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListDataSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListExperimentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListExtraDataSourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListFeatureTablesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2243 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListFilteringAlgorithmsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListFlowControlTaskInvalidItemsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListFlowControlTaskItemReportsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListFlowControlTaskItemsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListFlowControlTaskReferenceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListFlowControlTaskReportsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListFlowControlTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListIndexVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListInstanceTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListItemsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2392 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListMixCategoriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListOfflineStoragesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListRankingModelTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListRankingModelVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListRankingModelsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListRankingSystemHistoriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListRankingSystemsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListRuleConditionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListRuleTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListSampleFormatConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListSamplesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListSceneItemsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListSceneParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListScenesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListUmengAppkeysRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListUserClustersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyDataSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyFeatureTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyFilteringAlgorithmMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyFlowControlTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyItemsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyOfflineStoragesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyRankingModelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyRankingModelTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyRankingSystemRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifySampleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifySceneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/OfflineFilteringAlgorithmRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/PublishFlowControlTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/PublishRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/PushColdStartDocumentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1738 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/PushDocumentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/PushInterventionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/QueryDataMessageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3846 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/QueryDataMessageStatisticsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/QueryExceptionHistoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2552 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/QueryRawDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/QuerySingleAggregationReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/QuerySingleReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/QuerySyncReportAggregationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/RebuildIndexRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3608 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/RecommendRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/RefreshFeatureTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/RollbackRankingSystemRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/RunInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/RunRankingModelTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/RunSampleFormatConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1738 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/StopDataSetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/StopFlowControlTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/UnLockIndexVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/UpdateExperimentBasicInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/UpdateExperimentConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/UpdateExperimentStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/UpgradeInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ValidateInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/VerifyRankingSystemRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-04-14 08:44:16.000000 aliyun-python-sdk-airec-2.1.0/setup.py
```

### Comparing `aliyun-python-sdk-airec-2.0.1/LICENSE` & `aliyun-python-sdk-airec-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airec-2.0.1/PKG-INFO` & `aliyun-python-sdk-airec-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-airec
-Version: 2.0.1
+Version: 2.1.0
 Summary: The airec module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-airec
```

### Comparing `aliyun-python-sdk-airec-2.0.1/README.rst` & `aliyun-python-sdk-airec-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyun_python_sdk_airec.egg-info/PKG-INFO` & `aliyun-python-sdk-airec-2.1.0/aliyun_python_sdk_airec.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-airec
-Version: 2.0.1
+Version: 2.1.0
 Summary: The airec module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-airec
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyun_python_sdk_airec.egg-info/SOURCES.txt` & `aliyun-python-sdk-airec-2.1.0/aliyun_python_sdk_airec.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -11,26 +11,45 @@
 aliyunsdkairec/__init__.py
 aliyunsdkairec/endpoint.py
 aliyunsdkairec/request/__init__.py
 aliyunsdkairec/request/v20201126/AttachDatasetRequest.py
 aliyunsdkairec/request/v20201126/AttachIndexVersionRequest.py
 aliyunsdkairec/request/v20201126/CheckRankingModelReachableRequest.py
 aliyunsdkairec/request/v20201126/CloneExperimentRequest.py
+aliyunsdkairec/request/v20201126/CloneSampleRequest.py
+aliyunsdkairec/request/v20201126/ColdStartRankRequest.py
+aliyunsdkairec/request/v20201126/CreateCustomAnalysisTaskRequest.py
+aliyunsdkairec/request/v20201126/CreateCustomSampleRequest.py
+aliyunsdkairec/request/v20201126/CreateDataDiagnoseTaskRequest.py
+aliyunsdkairec/request/v20201126/CreateExtraDataSourceRequest.py
 aliyunsdkairec/request/v20201126/CreateFilteringAlgorithmRequest.py
+aliyunsdkairec/request/v20201126/CreateFlowControlTaskRequest.py
 aliyunsdkairec/request/v20201126/CreateInstanceRequest.py
 aliyunsdkairec/request/v20201126/CreateRankingModelRequest.py
+aliyunsdkairec/request/v20201126/CreateRankingModelTemplateRequest.py
+aliyunsdkairec/request/v20201126/CreateRankingSystemRequest.py
 aliyunsdkairec/request/v20201126/CreateRuleRequest.py
+aliyunsdkairec/request/v20201126/CreateSampleFormatConfigRequest.py
 aliyunsdkairec/request/v20201126/CreateSceneRequest.py
+aliyunsdkairec/request/v20201126/CreateUmengTokenRequest.py
 aliyunsdkairec/request/v20201126/DecribeRankingModelRequest.py
 aliyunsdkairec/request/v20201126/DeleteDataSetRequest.py
 aliyunsdkairec/request/v20201126/DeleteExperimentRequest.py
+aliyunsdkairec/request/v20201126/DeleteExtraDataSourceRequest.py
 aliyunsdkairec/request/v20201126/DeleteFilteringAlgorithmRequest.py
+aliyunsdkairec/request/v20201126/DeleteFlowControlTaskRequest.py
 aliyunsdkairec/request/v20201126/DeleteRankingModelRequest.py
+aliyunsdkairec/request/v20201126/DeleteRankingModelTemplateRequest.py
+aliyunsdkairec/request/v20201126/DeleteRankingModelVersionRequest.py
+aliyunsdkairec/request/v20201126/DeleteRankingSystemRequest.py
+aliyunsdkairec/request/v20201126/DeleteSampleRequest.py
 aliyunsdkairec/request/v20201126/DeleteSceneRequest.py
+aliyunsdkairec/request/v20201126/DeployRankingSystemRequest.py
 aliyunsdkairec/request/v20201126/DescribeBaseExperimentRequest.py
+aliyunsdkairec/request/v20201126/DescribeCustomAnalysisTaskRequest.py
 aliyunsdkairec/request/v20201126/DescribeDataSetMessageRequest.py
 aliyunsdkairec/request/v20201126/DescribeDefaultAlgorithmsRequest.py
 aliyunsdkairec/request/v20201126/DescribeExperimentEnvProgressRequest.py
 aliyunsdkairec/request/v20201126/DescribeExperimentEnvRequest.py
 aliyunsdkairec/request/v20201126/DescribeExperimentRequest.py
 aliyunsdkairec/request/v20201126/DescribeFilteringAlgorithmRequest.py
 aliyunsdkairec/request/v20201126/DescribeInstanceRequest.py
@@ -42,59 +61,100 @@
 aliyunsdkairec/request/v20201126/DescribeSceneRequest.py
 aliyunsdkairec/request/v20201126/DescribeSceneThroughputRequest.py
 aliyunsdkairec/request/v20201126/DescribeSyncReportDetailRequest.py
 aliyunsdkairec/request/v20201126/DescribeSyncReportOutliersRequest.py
 aliyunsdkairec/request/v20201126/DescribeUserMetricsRequest.py
 aliyunsdkairec/request/v20201126/DowngradeInstanceRequest.py
 aliyunsdkairec/request/v20201126/EnableExperimentRequest.py
+aliyunsdkairec/request/v20201126/GenerateSampleRequest.py
+aliyunsdkairec/request/v20201126/GetExtraDataSourceRequest.py
+aliyunsdkairec/request/v20201126/GetFlowControlTaskRequest.py
+aliyunsdkairec/request/v20201126/GetLatestDataDiagnoseTaskStatusRequest.py
+aliyunsdkairec/request/v20201126/GetRankingModelTemplateRequest.py
+aliyunsdkairec/request/v20201126/GetRankingModelVersionRequest.py
+aliyunsdkairec/request/v20201126/GetRankingSystemHistoryRequest.py
+aliyunsdkairec/request/v20201126/GetRankingSystemRequest.py
+aliyunsdkairec/request/v20201126/GetSampleRequest.py
+aliyunsdkairec/request/v20201126/InitComputingResourceRequest.py
 aliyunsdkairec/request/v20201126/ListDashboardDetailsFlowsRequest.py
 aliyunsdkairec/request/v20201126/ListDashboardDetailsRequest.py
 aliyunsdkairec/request/v20201126/ListDashboardMetricsFlowsRequest.py
 aliyunsdkairec/request/v20201126/ListDashboardMetricsRequest.py
+aliyunsdkairec/request/v20201126/ListDataDiagnoseReportsRequest.py
+aliyunsdkairec/request/v20201126/ListDataDiagnoseSampleDetailsRequest.py
 aliyunsdkairec/request/v20201126/ListDataSetRequest.py
 aliyunsdkairec/request/v20201126/ListDataSourceRequest.py
 aliyunsdkairec/request/v20201126/ListExperimentsRequest.py
+aliyunsdkairec/request/v20201126/ListExtraDataSourcesRequest.py
+aliyunsdkairec/request/v20201126/ListFeatureTablesRequest.py
 aliyunsdkairec/request/v20201126/ListFilteringAlgorithmsRequest.py
+aliyunsdkairec/request/v20201126/ListFlowControlTaskInvalidItemsRequest.py
+aliyunsdkairec/request/v20201126/ListFlowControlTaskItemReportsRequest.py
+aliyunsdkairec/request/v20201126/ListFlowControlTaskItemsRequest.py
+aliyunsdkairec/request/v20201126/ListFlowControlTaskReferenceRequest.py
+aliyunsdkairec/request/v20201126/ListFlowControlTaskReportsRequest.py
+aliyunsdkairec/request/v20201126/ListFlowControlTaskRequest.py
 aliyunsdkairec/request/v20201126/ListIndexVersionsRequest.py
 aliyunsdkairec/request/v20201126/ListInstanceRequest.py
 aliyunsdkairec/request/v20201126/ListInstanceTaskRequest.py
 aliyunsdkairec/request/v20201126/ListItemsRequest.py
 aliyunsdkairec/request/v20201126/ListLogsRequest.py
 aliyunsdkairec/request/v20201126/ListMixCategoriesRequest.py
+aliyunsdkairec/request/v20201126/ListOfflineStoragesRequest.py
+aliyunsdkairec/request/v20201126/ListRankingModelTemplatesRequest.py
+aliyunsdkairec/request/v20201126/ListRankingModelVersionsRequest.py
 aliyunsdkairec/request/v20201126/ListRankingModelsRequest.py
+aliyunsdkairec/request/v20201126/ListRankingSystemHistoriesRequest.py
+aliyunsdkairec/request/v20201126/ListRankingSystemsRequest.py
 aliyunsdkairec/request/v20201126/ListRuleConditionsRequest.py
 aliyunsdkairec/request/v20201126/ListRuleTasksRequest.py
 aliyunsdkairec/request/v20201126/ListRulesRequest.py
+aliyunsdkairec/request/v20201126/ListSampleFormatConfigsRequest.py
+aliyunsdkairec/request/v20201126/ListSamplesRequest.py
 aliyunsdkairec/request/v20201126/ListSceneItemsRequest.py
 aliyunsdkairec/request/v20201126/ListSceneParametersRequest.py
 aliyunsdkairec/request/v20201126/ListScenesRequest.py
 aliyunsdkairec/request/v20201126/ListUmengAppkeysRequest.py
 aliyunsdkairec/request/v20201126/ListUserClustersRequest.py
 aliyunsdkairec/request/v20201126/ModifyDataSourceRequest.py
+aliyunsdkairec/request/v20201126/ModifyFeatureTableRequest.py
 aliyunsdkairec/request/v20201126/ModifyFilteringAlgorithmMetaRequest.py
+aliyunsdkairec/request/v20201126/ModifyFlowControlTaskRequest.py
 aliyunsdkairec/request/v20201126/ModifyInstanceRequest.py
 aliyunsdkairec/request/v20201126/ModifyItemsRequest.py
+aliyunsdkairec/request/v20201126/ModifyOfflineStoragesRequest.py
 aliyunsdkairec/request/v20201126/ModifyRankingModelRequest.py
+aliyunsdkairec/request/v20201126/ModifyRankingModelTemplateRequest.py
+aliyunsdkairec/request/v20201126/ModifyRankingSystemRequest.py
 aliyunsdkairec/request/v20201126/ModifyRuleRequest.py
+aliyunsdkairec/request/v20201126/ModifySampleRequest.py
 aliyunsdkairec/request/v20201126/ModifySceneRequest.py
 aliyunsdkairec/request/v20201126/OfflineFilteringAlgorithmRequest.py
+aliyunsdkairec/request/v20201126/PublishFlowControlTaskRequest.py
 aliyunsdkairec/request/v20201126/PublishRuleRequest.py
+aliyunsdkairec/request/v20201126/PushColdStartDocumentRequest.py
 aliyunsdkairec/request/v20201126/PushDocumentRequest.py
 aliyunsdkairec/request/v20201126/PushInterventionRequest.py
 aliyunsdkairec/request/v20201126/QueryDataMessageRequest.py
 aliyunsdkairec/request/v20201126/QueryDataMessageStatisticsRequest.py
 aliyunsdkairec/request/v20201126/QueryExceptionHistoryRequest.py
 aliyunsdkairec/request/v20201126/QueryRawDataRequest.py
 aliyunsdkairec/request/v20201126/QuerySingleAggregationReportRequest.py
 aliyunsdkairec/request/v20201126/QuerySingleReportRequest.py
 aliyunsdkairec/request/v20201126/QuerySyncReportAggregationRequest.py
 aliyunsdkairec/request/v20201126/RebuildIndexRequest.py
 aliyunsdkairec/request/v20201126/RecommendRequest.py
+aliyunsdkairec/request/v20201126/RefreshFeatureTableRequest.py
+aliyunsdkairec/request/v20201126/RollbackRankingSystemRequest.py
 aliyunsdkairec/request/v20201126/RunInstanceRequest.py
+aliyunsdkairec/request/v20201126/RunRankingModelTemplateRequest.py
+aliyunsdkairec/request/v20201126/RunSampleFormatConfigRequest.py
 aliyunsdkairec/request/v20201126/StopDataSetRequest.py
+aliyunsdkairec/request/v20201126/StopFlowControlTaskRequest.py
 aliyunsdkairec/request/v20201126/UnLockIndexVersionRequest.py
 aliyunsdkairec/request/v20201126/UpdateExperimentBasicInfoRequest.py
 aliyunsdkairec/request/v20201126/UpdateExperimentConfigRequest.py
 aliyunsdkairec/request/v20201126/UpdateExperimentStatusRequest.py
 aliyunsdkairec/request/v20201126/UpgradeInstanceRequest.py
 aliyunsdkairec/request/v20201126/ValidateInstanceRequest.py
+aliyunsdkairec/request/v20201126/VerifyRankingSystemRequest.py
 aliyunsdkairec/request/v20201126/__init__.py
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/endpoint.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/AttachDatasetRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/AttachDatasetRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,25 +21,24 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class AttachDatasetRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'AttachDataset','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dataSets/[versionId]/actions/current')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_versionId(self):
+	def get_versionId(self): # String
 		return self.get_path_params().get('versionId')
 
-	def set_versionId(self,versionId):
-		self.add_path_param('versionId',versionId)
-
-	def get_instanceId(self):
+	def set_versionId(self, versionId):  # String
+		self.add_path_param('versionId', versionId)
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/AttachIndexVersionRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/InitComputingResourceRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,36 +16,34 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class AttachIndexVersionRequest(RoaRequest):
+class InitComputingResourceRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'AttachIndexVersion','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms/[algorithmId]/index-versions/[versionId]/actions/attach')
-		self.set_method('POST')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'InitComputingResource','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/computing-resources/actions/init')
+		self.set_method('PUT')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_versionId(self):
-		return self.get_path_params().get('versionId')
-
-	def set_versionId(self,versionId):
-		self.add_path_param('versionId',versionId)
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_algorithmId(self):
-		return self.get_path_params().get('algorithmId')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_type(self): # String
+		return self.get_query_params().get('type')
+
+	def set_type(self, type):  # String
+		self.add_query_param('type', type)
+	def get_key(self): # String
+		return self.get_query_params().get('key')
 
-	def set_algorithmId(self,algorithmId):
-		self.add_path_param('algorithmId',algorithmId)
+	def set_key(self, key):  # String
+		self.add_query_param('key', key)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/CheckRankingModelReachableRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DecribeRankingModelRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class CheckRankingModelReachableRequest(RoaRequest):
+class DecribeRankingModelRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CheckRankingModelReachable','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-models/[rankingModelId]/actions/check-connectivity')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DecribeRankingModel','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-models/[rankingModelId]')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_rankingModelId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_rankingModelId(self): # String
 		return self.get_path_params().get('rankingModelId')
 
-	def set_rankingModelId(self,rankingModelId):
-		self.add_path_param('rankingModelId',rankingModelId)
+	def set_rankingModelId(self, rankingModelId):  # String
+		self.add_path_param('rankingModelId', rankingModelId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/CloneExperimentRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/UpdateExperimentConfigRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,42 +16,34 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class CloneExperimentRequest(RoaRequest):
+class UpdateExperimentConfigRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CloneExperiment','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiments/[experimentId]/actions/clone')
-		self.set_method('POST')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'UpdateExperimentConfig','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiments/[experimentId]/config')
+		self.set_method('PUT')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_dryRun(self):
-		return self.get_query_params().get('dryRun')
-
-	def set_dryRun(self,dryRun):
-		self.add_query_param('dryRun',dryRun)
-
-	def get_sceneId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sceneId(self): # String
 		return self.get_path_params().get('sceneId')
 
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
-
-	def get_experimentId(self):
+	def set_sceneId(self, sceneId):  # String
+		self.add_path_param('sceneId', sceneId)
+	def get_experimentId(self): # String
 		return self.get_path_params().get('experimentId')
 
-	def set_experimentId(self,experimentId):
-		self.add_path_param('experimentId',experimentId)
+	def set_experimentId(self, experimentId):  # String
+		self.add_path_param('experimentId', experimentId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/CreateFilteringAlgorithmRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/QuerySingleAggregationReportRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,30 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class CreateFilteringAlgorithmRequest(RoaRequest):
+class QuerySingleAggregationReportRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateFilteringAlgorithm','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms')
-		self.set_method('POST')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'QuerySingleAggregationReport','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/sync-reports/single-aggregation-report')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_dryRun(self):
-		return self.get_query_params().get('dryRun')
-
-	def set_dryRun(self,dryRun):
-		self.add_query_param('dryRun',dryRun)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/CreateInstanceRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateInstanceRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,12 +21,14 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class CreateInstanceRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateInstance','airec')
 		self.set_uri_pattern('/v2/openapi/instances')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
+
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/CreateRankingModelRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/UpgradeInstanceRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class CreateRankingModelRequest(RoaRequest):
+class UpgradeInstanceRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateRankingModel','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-models')
-		self.set_method('POST')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'UpgradeInstance','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/actions/upgrade')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_dryRun(self):
-		return self.get_query_params().get('dryRun')
-
-	def set_dryRun(self,dryRun):
-		self.add_query_param('dryRun',dryRun)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/CreateRuleRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeQuotaRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class CreateRuleRequest(RoaRequest):
+class DescribeQuotaRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateRule','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/rules')
-		self.set_method('POST')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeQuota','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/quota')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/CreateSceneRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateFilteringAlgorithmRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class CreateSceneRequest(RoaRequest):
+class CreateFilteringAlgorithmRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateScene','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes')
-		self.set_method('POST')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateFilteringAlgorithm','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_dryRun(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_dryRun(self): # String
 		return self.get_query_params().get('dryRun')
 
-	def set_dryRun(self,dryRun):
-		self.add_query_param('dryRun',dryRun)
+	def set_dryRun(self, dryRun):  # String
+		self.add_query_param('dryRun', dryRun)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DecribeRankingModelRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyRankingModelRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DecribeRankingModelRequest(RoaRequest):
+class ModifyRankingModelRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DecribeRankingModel','airec')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ModifyRankingModel','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-models/[rankingModelId]')
-		self.set_method('GET')
+		self.set_method('PUT')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_rankingModelId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_rankingModelId(self): # String
 		return self.get_path_params().get('rankingModelId')
 
-	def set_rankingModelId(self,rankingModelId):
-		self.add_path_param('rankingModelId',rankingModelId)
+	def set_rankingModelId(self, rankingModelId):  # String
+		self.add_path_param('rankingModelId', rankingModelId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DeleteDataSetRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteDataSetRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,25 +21,24 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class DeleteDataSetRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DeleteDataSet','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dataSets/[versionId]')
-		self.set_method('DELETE')
+		self.set_method('DELETE')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_versionId(self):
+	def get_versionId(self): # String
 		return self.get_path_params().get('versionId')
 
-	def set_versionId(self,versionId):
-		self.add_path_param('versionId',versionId)
-
-	def get_instanceId(self):
+	def set_versionId(self, versionId):  # String
+		self.add_path_param('versionId', versionId)
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DeleteExperimentRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeExperimentRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,36 +16,34 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DeleteExperimentRequest(RoaRequest):
+class DescribeExperimentRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DeleteExperiment','airec')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeExperiment','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiments/[experimentId]')
-		self.set_method('DELETE')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sceneId(self): # String
 		return self.get_path_params().get('sceneId')
 
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
-
-	def get_experimentId(self):
+	def set_sceneId(self, sceneId):  # String
+		self.add_path_param('sceneId', sceneId)
+	def get_experimentId(self): # String
 		return self.get_path_params().get('experimentId')
 
-	def set_experimentId(self,experimentId):
-		self.add_path_param('experimentId',experimentId)
+	def set_experimentId(self, experimentId):  # String
+		self.add_path_param('experimentId', experimentId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DeleteFilteringAlgorithmRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteFilteringAlgorithmRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,25 +21,24 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class DeleteFilteringAlgorithmRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DeleteFilteringAlgorithm','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms/[algorithmId]')
-		self.set_method('DELETE')
+		self.set_method('DELETE')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_algorithmId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_algorithmId(self): # String
 		return self.get_path_params().get('algorithmId')
 
-	def set_algorithmId(self,algorithmId):
-		self.add_path_param('algorithmId',algorithmId)
+	def set_algorithmId(self, algorithmId):  # String
+		self.add_path_param('algorithmId', algorithmId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DeleteRankingModelRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListRankingModelsRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,39 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DeleteRankingModelRequest(RoaRequest):
+class ListRankingModelsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DeleteRankingModel','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-models/[rankingModelId]')
-		self.set_method('DELETE')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListRankingModels','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-models')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_size(self): # Integer
+		return self.get_query_params().get('size')
+
+	def set_size(self, size):  # Integer
+		self.add_query_param('size', size)
+	def get_rankingModelId(self): # String
+		return self.get_query_params().get('rankingModelId')
 
-	def get_rankingModelId(self):
-		return self.get_path_params().get('rankingModelId')
+	def set_rankingModelId(self, rankingModelId):  # String
+		self.add_query_param('rankingModelId', rankingModelId)
+	def get_page(self): # Integer
+		return self.get_query_params().get('page')
 
-	def set_rankingModelId(self,rankingModelId):
-		self.add_path_param('rankingModelId',rankingModelId)
+	def set_page(self, page):  # Integer
+		self.add_query_param('page', page)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DeleteSceneRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeInstanceRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,30 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DeleteSceneRequest(RoaRequest):
+class DescribeInstanceRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DeleteScene','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]')
-		self.set_method('DELETE')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeInstance','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
-		return self.get_path_params().get('sceneId')
-
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeBaseExperimentRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DowngradeInstanceRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeBaseExperimentRequest(RoaRequest):
+class DowngradeInstanceRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeBaseExperiment','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/base-experiment')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DowngradeInstance','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/actions/downgrade')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
-		return self.get_path_params().get('sceneId')
-
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeDataSetMessageRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeDataSetMessageRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,25 +21,24 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class DescribeDataSetMessageRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeDataSetMessage','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dataSets/[versionId]/messages')
-		self.set_method('GET')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_versionId(self):
+	def get_versionId(self): # String
 		return self.get_path_params().get('versionId')
 
-	def set_versionId(self,versionId):
-		self.add_path_param('versionId',versionId)
-
-	def get_instanceId(self):
+	def set_versionId(self, versionId):  # String
+		self.add_path_param('versionId', versionId)
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeDefaultAlgorithmsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeSceneBucketRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeDefaultAlgorithmsRequest(RoaRequest):
+class DescribeSceneBucketRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeDefaultAlgorithms','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/default-algorithms')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeSceneBucket','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiment-bucket')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sceneId(self): # String
 		return self.get_path_params().get('sceneId')
 
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
+	def set_sceneId(self, sceneId):  # String
+		self.add_path_param('sceneId', sceneId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeExperimentEnvProgressRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyInstanceRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,30 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeExperimentEnvProgressRequest(RoaRequest):
+class ModifyInstanceRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeExperimentEnvProgress','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiment-progress')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ModifyInstance','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]')
+		self.set_method('PUT')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
-		return self.get_path_params().get('sceneId')
-
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeExperimentEnvRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeSceneRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeExperimentEnvRequest(RoaRequest):
+class DescribeSceneRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeExperimentEnv','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiment-env')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeScene','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sceneId(self): # String
 		return self.get_path_params().get('sceneId')
 
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
+	def set_sceneId(self, sceneId):  # String
+		self.add_path_param('sceneId', sceneId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeExperimentRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CloneExperimentRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,36 +16,39 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeExperimentRequest(RoaRequest):
+class CloneExperimentRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeExperiment','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiments/[experimentId]')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CloneExperiment','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiments/[experimentId]/actions/clone')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_dryRun(self): # Boolean
+		return self.get_query_params().get('dryRun')
+
+	def set_dryRun(self, dryRun):  # Boolean
+		self.add_query_param('dryRun', dryRun)
+	def get_sceneId(self): # String
 		return self.get_path_params().get('sceneId')
 
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
-
-	def get_experimentId(self):
+	def set_sceneId(self, sceneId):  # String
+		self.add_path_param('sceneId', sceneId)
+	def get_experimentId(self): # String
 		return self.get_path_params().get('experimentId')
 
-	def set_experimentId(self,experimentId):
-		self.add_path_param('experimentId',experimentId)
+	def set_experimentId(self, experimentId):  # String
+		self.add_path_param('experimentId', experimentId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeFilteringAlgorithmRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/OfflineFilteringAlgorithmRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeFilteringAlgorithmRequest(RoaRequest):
+class OfflineFilteringAlgorithmRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeFilteringAlgorithm','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms/[algorithmId]')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'OfflineFilteringAlgorithm','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms/[algorithmId]/actions/offline')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_algorithmId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_algorithmId(self): # String
 		return self.get_path_params().get('algorithmId')
 
-	def set_algorithmId(self,algorithmId):
-		self.add_path_param('algorithmId',algorithmId)
+	def set_algorithmId(self, algorithmId):  # String
+		self.add_path_param('algorithmId', algorithmId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeInstanceRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifySceneRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,24 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeInstanceRequest(RoaRequest):
+class ModifySceneRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeInstance','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ModifyScene','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]')
+		self.set_method('PUT')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sceneId(self): # String
+		return self.get_path_params().get('sceneId')
+
+	def set_sceneId(self, sceneId):  # String
+		self.add_path_param('sceneId', sceneId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeLatestTaskRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeFilteringAlgorithmRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeLatestTaskRequest(RoaRequest):
+class DescribeFilteringAlgorithmRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeLatestTask','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms/[algorithmId]/tasks/latest')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeFilteringAlgorithm','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms/[algorithmId]')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_algorithmId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_algorithmId(self): # String
 		return self.get_path_params().get('algorithmId')
 
-	def set_algorithmId(self,algorithmId):
-		self.add_path_param('algorithmId',algorithmId)
+	def set_algorithmId(self, algorithmId):  # String
+		self.add_path_param('algorithmId', algorithmId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeQuotaRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateExtraDataSourceRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeQuotaRequest(RoaRequest):
+class CreateExtraDataSourceRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeQuota','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/quota')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateExtraDataSource','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/extra-data-sources')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeRegionsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeRegionsRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class DescribeRegionsRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeRegions','airec')
 		self.set_uri_pattern('/v2/openapi/configurations/regions')
-		self.set_method('GET')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_acceptLanguage(self):
+	def get_acceptLanguage(self): # String
 		return self.get_query_params().get('acceptLanguage')
 
-	def set_acceptLanguage(self,acceptLanguage):
-		self.add_query_param('acceptLanguage',acceptLanguage)
+	def set_acceptLanguage(self, acceptLanguage):  # String
+		self.add_query_param('acceptLanguage', acceptLanguage)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeRuleRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/PublishRuleRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,42 +16,39 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeRuleRequest(RoaRequest):
+class PublishRuleRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeRule','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/rules/[ruleId]')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'PublishRule','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/rules/[ruleId]/actions/publish')
+		self.set_method('PUT')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_ruleType(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_ruleType(self): # String
 		return self.get_query_params().get('ruleType')
 
-	def set_ruleType(self,ruleType):
-		self.add_query_param('ruleType',ruleType)
-
-	def get_sceneId(self):
+	def set_ruleType(self, ruleType):  # String
+		self.add_query_param('ruleType', ruleType)
+	def get_sceneId(self): # String
 		return self.get_query_params().get('sceneId')
 
-	def set_sceneId(self,sceneId):
-		self.add_query_param('sceneId',sceneId)
-
-	def get_ruleId(self):
+	def set_sceneId(self, sceneId):  # String
+		self.add_query_param('sceneId', sceneId)
+	def get_ruleId(self): # String
 		return self.get_path_params().get('ruleId')
 
-	def set_ruleId(self,ruleId):
-		self.add_path_param('ruleId',ruleId)
+	def set_ruleId(self, ruleId):  # String
+		self.add_path_param('ruleId', ruleId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeSceneBucketRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/EnableExperimentRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeSceneBucketRequest(RoaRequest):
+class EnableExperimentRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeSceneBucket','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiment-bucket')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'EnableExperiment','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/actions/enable-experiment')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sceneId(self): # String
 		return self.get_path_params().get('sceneId')
 
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
+	def set_sceneId(self, sceneId):  # String
+		self.add_path_param('sceneId', sceneId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeSceneRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeBaseExperimentRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeSceneRequest(RoaRequest):
+class DescribeBaseExperimentRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeScene','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeBaseExperiment','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/base-experiment')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sceneId(self): # String
 		return self.get_path_params().get('sceneId')
 
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
+	def set_sceneId(self, sceneId):  # String
+		self.add_path_param('sceneId', sceneId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeSceneThroughputRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListRuleTasksRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeSceneThroughputRequest(RoaRequest):
+class ListRuleTasksRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeSceneThroughput','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/throughput')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListRuleTasks','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/rule-tasks')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
-		return self.get_path_params().get('sceneId')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sceneId(self): # String
+		return self.get_query_params().get('sceneId')
 
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
+	def set_sceneId(self, sceneId):  # String
+		self.add_query_param('sceneId', sceneId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeSyncReportDetailRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListInstanceRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,48 +16,49 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeSyncReportDetailRequest(RoaRequest):
+class ListInstanceRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeSyncReportDetail','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/sync-reports/detail')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListInstance','airec')
+		self.set_uri_pattern('/v2/openapi/instances')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_instanceId(self): # String
+		return self.get_query_params().get('instanceId')
 
-	def get_instanceId(self):
-		return self.get_path_params().get('instanceId')
-
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_levelType(self):
-		return self.get_query_params().get('levelType')
-
-	def set_levelType(self,levelType):
-		self.add_query_param('levelType',levelType)
-
-	def get_endTime(self):
-		return self.get_query_params().get('endTime')
-
-	def set_endTime(self,endTime):
-		self.add_query_param('endTime',endTime)
-
-	def get_startTime(self):
-		return self.get_query_params().get('startTime')
-
-	def set_startTime(self,startTime):
-		self.add_query_param('startTime',startTime)
-
-	def get_type(self):
-		return self.get_query_params().get('type')
+	def set_instanceId(self, instanceId):  # String
+		self.add_query_param('instanceId', instanceId)
+	def get_size(self): # Integer
+		return self.get_query_params().get('size')
+
+	def set_size(self, size):  # Integer
+		self.add_query_param('size', size)
+	def get_name(self): # String
+		return self.get_query_params().get('name')
+
+	def set_name(self, name):  # String
+		self.add_query_param('name', name)
+	def get_expiredTime(self): # String
+		return self.get_query_params().get('expiredTime')
+
+	def set_expiredTime(self, expiredTime):  # String
+		self.add_query_param('expiredTime', expiredTime)
+	def get_page(self): # Integer
+		return self.get_query_params().get('page')
+
+	def set_page(self, page):  # Integer
+		self.add_query_param('page', page)
+	def get_status(self): # String
+		return self.get_query_params().get('status')
 
-	def set_type(self,type):
-		self.add_query_param('type',type)
+	def set_status(self, status):  # String
+		self.add_query_param('status', status)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeSyncReportOutliersRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListSceneItemsRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,54 +16,59 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeSyncReportOutliersRequest(RoaRequest):
+class ListSceneItemsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeSyncReportOutliers','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/sync-reports/outliers')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListSceneItems','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/items')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_selectionRuleId(self): # String
+		return self.get_query_params().get('selectionRuleId')
 
-	def get_instanceId(self):
+	def set_selectionRuleId(self, selectionRuleId):  # String
+		self.add_query_param('selectionRuleId', selectionRuleId)
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_levelType(self):
-		return self.get_query_params().get('levelType')
-
-	def set_levelType(self,levelType):
-		self.add_query_param('levelType',levelType)
-
-	def get_endTime(self):
-		return self.get_query_params().get('endTime')
-
-	def set_endTime(self,endTime):
-		self.add_query_param('endTime',endTime)
-
-	def get_startTime(self):
-		return self.get_query_params().get('startTime')
-
-	def set_startTime(self,startTime):
-		self.add_query_param('startTime',startTime)
-
-	def get_type(self):
-		return self.get_query_params().get('type')
-
-	def set_type(self,type):
-		self.add_query_param('type',type)
-
-	def get_key(self):
-		return self.get_query_params().get('key')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_size(self): # Integer
+		return self.get_query_params().get('size')
+
+	def set_size(self, size):  # Integer
+		self.add_query_param('size', size)
+	def get_queryCount(self): # Integer
+		return self.get_query_params().get('queryCount')
+
+	def set_queryCount(self, queryCount):  # Integer
+		self.add_query_param('queryCount', queryCount)
+	def get_sceneId(self): # String
+		return self.get_path_params().get('sceneId')
+
+	def set_sceneId(self, sceneId):  # String
+		self.add_path_param('sceneId', sceneId)
+	def get_operationRuleId(self): # String
+		return self.get_query_params().get('operationRuleId')
+
+	def set_operationRuleId(self, operationRuleId):  # String
+		self.add_query_param('operationRuleId', operationRuleId)
+	def get_previewType(self): # String
+		return self.get_query_params().get('previewType')
+
+	def set_previewType(self, previewType):  # String
+		self.add_query_param('previewType', previewType)
+	def get_page(self): # Integer
+		return self.get_query_params().get('page')
 
-	def set_key(self,key):
-		self.add_query_param('key',key)
+	def set_page(self, page):  # Integer
+		self.add_query_param('page', page)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DescribeUserMetricsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListDashboardMetricsFlowsRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,42 +16,39 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DescribeUserMetricsRequest(RoaRequest):
+class ListDashboardMetricsFlowsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeUserMetrics','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/metrics')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListDashboardMetricsFlows','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dashboard/metrics/flows')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_metricType(self):
+	def get_metricType(self): # String
 		return self.get_query_params().get('metricType')
 
-	def set_metricType(self,metricType):
-		self.add_query_param('metricType',metricType)
-
-	def get_instanceId(self):
+	def set_metricType(self, metricType):  # String
+		self.add_query_param('metricType', metricType)
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_endTime(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_endTime(self): # Long
 		return self.get_query_params().get('endTime')
 
-	def set_endTime(self,endTime):
-		self.add_query_param('endTime',endTime)
-
-	def get_startTime(self):
+	def set_endTime(self, endTime):  # Long
+		self.add_query_param('endTime', endTime)
+	def get_startTime(self): # Long
 		return self.get_query_params().get('startTime')
 
-	def set_startTime(self,startTime):
-		self.add_query_param('startTime',startTime)
+	def set_startTime(self, startTime):  # Long
+		self.add_query_param('startTime', startTime)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/DowngradeInstanceRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListRuleConditionsRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class DowngradeInstanceRequest(RoaRequest):
+class ListRuleConditionsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DowngradeInstance','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/actions/downgrade')
-		self.set_method('POST')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListRuleConditions','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/rule-conditions')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/EnableExperimentRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateRankingModelTemplateRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,30 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class EnableExperimentRequest(RoaRequest):
+class CreateRankingModelTemplateRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'EnableExperiment','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/actions/enable-experiment')
-		self.set_method('POST')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateRankingModelTemplate','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-model-templates')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
-		return self.get_path_params().get('sceneId')
-
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListDashboardDetailsFlowsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListDashboardDetailsRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,60 +16,59 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListDashboardDetailsFlowsRequest(RoaRequest):
+class ListDashboardDetailsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListDashboardDetailsFlows','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dashboard/details/flows')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListDashboardDetails','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dashboard/details')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_metricType(self):
+	def get_metricType(self): # String
 		return self.get_query_params().get('metricType')
 
-	def set_metricType(self,metricType):
-		self.add_query_param('metricType',metricType)
-
-	def get_instanceId(self):
+	def set_metricType(self, metricType):  # String
+		self.add_query_param('metricType', metricType)
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_experimentIds(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_experimentIds(self): # String
 		return self.get_query_params().get('experimentIds')
 
-	def set_experimentIds(self,experimentIds):
-		self.add_query_param('experimentIds',experimentIds)
-
-	def get_traceIds(self):
+	def set_experimentIds(self, experimentIds):  # String
+		self.add_query_param('experimentIds', experimentIds)
+	def get_matchTypes(self): # String
+		return self.get_query_params().get('matchTypes')
+
+	def set_matchTypes(self, matchTypes):  # String
+		self.add_query_param('matchTypes', matchTypes)
+	def get_traceIds(self): # String
 		return self.get_query_params().get('traceIds')
 
-	def set_traceIds(self,traceIds):
-		self.add_query_param('traceIds',traceIds)
-
-	def get_endTime(self):
+	def set_traceIds(self, traceIds):  # String
+		self.add_query_param('traceIds', traceIds)
+	def get_endTime(self): # Long
 		return self.get_query_params().get('endTime')
 
-	def set_endTime(self,endTime):
-		self.add_query_param('endTime',endTime)
-
-	def get_startTime(self):
+	def set_endTime(self, endTime):  # Long
+		self.add_query_param('endTime', endTime)
+	def get_startTime(self): # Long
 		return self.get_query_params().get('startTime')
 
-	def set_startTime(self,startTime):
-		self.add_query_param('startTime',startTime)
-
-	def get_sceneIds(self):
+	def set_startTime(self, startTime):  # Long
+		self.add_query_param('startTime', startTime)
+	def get_sceneIds(self): # String
 		return self.get_query_params().get('sceneIds')
 
-	def set_sceneIds(self,sceneIds):
-		self.add_query_param('sceneIds',sceneIds)
+	def set_sceneIds(self, sceneIds):  # String
+		self.add_query_param('sceneIds', sceneIds)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListDashboardDetailsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListScenesRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,60 +16,44 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListDashboardDetailsRequest(RoaRequest):
+class ListScenesRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListDashboardDetails','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dashboard/details')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListScenes','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_metricType(self):
-		return self.get_query_params().get('metricType')
-
-	def set_metricType(self,metricType):
-		self.add_query_param('metricType',metricType)
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_experimentIds(self):
-		return self.get_query_params().get('experimentIds')
-
-	def set_experimentIds(self,experimentIds):
-		self.add_query_param('experimentIds',experimentIds)
-
-	def get_traceIds(self):
-		return self.get_query_params().get('traceIds')
-
-	def set_traceIds(self,traceIds):
-		self.add_query_param('traceIds',traceIds)
-
-	def get_endTime(self):
-		return self.get_query_params().get('endTime')
-
-	def set_endTime(self,endTime):
-		self.add_query_param('endTime',endTime)
-
-	def get_startTime(self):
-		return self.get_query_params().get('startTime')
-
-	def set_startTime(self,startTime):
-		self.add_query_param('startTime',startTime)
-
-	def get_sceneIds(self):
-		return self.get_query_params().get('sceneIds')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_size(self): # Integer
+		return self.get_query_params().get('size')
+
+	def set_size(self, size):  # Integer
+		self.add_query_param('size', size)
+	def get_sceneId(self): # String
+		return self.get_query_params().get('sceneId')
+
+	def set_sceneId(self, sceneId):  # String
+		self.add_query_param('sceneId', sceneId)
+	def get_page(self): # Integer
+		return self.get_query_params().get('page')
+
+	def set_page(self, page):  # Integer
+		self.add_query_param('page', page)
+	def get_status(self): # String
+		return self.get_query_params().get('status')
 
-	def set_sceneIds(self,sceneIds):
-		self.add_query_param('sceneIds',sceneIds)
+	def set_status(self, status):  # String
+		self.add_query_param('status', status)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListDashboardMetricsFlowsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/QueryExceptionHistoryRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,42 +16,39 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListDashboardMetricsFlowsRequest(RoaRequest):
+class QueryExceptionHistoryRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListDashboardMetricsFlows','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dashboard/metrics/flows')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'QueryExceptionHistory','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/sync-reports/exception-history')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_metricType(self):
-		return self.get_query_params().get('metricType')
-
-	def set_metricType(self,metricType):
-		self.add_query_param('metricType',metricType)
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_endTime(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_endTime(self): # Long
 		return self.get_query_params().get('endTime')
 
-	def set_endTime(self,endTime):
-		self.add_query_param('endTime',endTime)
-
-	def get_startTime(self):
+	def set_endTime(self, endTime):  # Long
+		self.add_query_param('endTime', endTime)
+	def get_startTime(self): # Long
 		return self.get_query_params().get('startTime')
 
-	def set_startTime(self,startTime):
-		self.add_query_param('startTime',startTime)
+	def set_startTime(self, startTime):  # Long
+		self.add_query_param('startTime', startTime)
+	def get_type(self): # String
+		return self.get_query_params().get('type')
+
+	def set_type(self, type):  # String
+		self.add_query_param('type', type)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListDashboardMetricsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListDataSourceRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,42 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListDashboardMetricsRequest(RoaRequest):
+class ListDataSourceRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListDashboardMetrics','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dashboard/metrics')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListDataSource','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dataSources')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_metricType(self):
-		return self.get_query_params().get('metricType')
-
-	def set_metricType(self,metricType):
-		self.add_query_param('metricType',metricType)
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_endTime(self):
-		return self.get_query_params().get('endTime')
-
-	def set_endTime(self,endTime):
-		self.add_query_param('endTime',endTime)
-
-	def get_startTime(self):
-		return self.get_query_params().get('startTime')
-
-	def set_startTime(self,startTime):
-		self.add_query_param('startTime',startTime)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListDataSetRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListDataSetRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class ListDataSetRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListDataSet','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dataSets')
-		self.set_method('GET')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListDataSourceRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateRuleRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListDataSourceRequest(RoaRequest):
+class CreateRuleRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListDataSource','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dataSources')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateRule','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/rules')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListExperimentsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/GetRankingModelTemplateRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListExperimentsRequest(RoaRequest):
+class GetRankingModelTemplateRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListExperiments','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiments')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'GetRankingModelTemplate','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-model-templates/[templateId]')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
-		return self.get_path_params().get('sceneId')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_templateId(self): # String
+		return self.get_path_params().get('templateId')
 
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
+	def set_templateId(self, templateId):  # String
+		self.add_path_param('templateId', templateId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListFilteringAlgorithmsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ColdStartRankRequest.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,48 +16,49 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListFilteringAlgorithmsRequest(RoaRequest):
+class ColdStartRankRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListFilteringAlgorithms','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ColdStartRank','airec')
+		self.set_uri_pattern('/v2/openapi/instances/cold-start/[instanceId]/actions/rank')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_features(self): # String
+		return self.get_query_params().get('features')
 
-	def get_instanceId(self):
+	def set_features(self, features):  # String
+		self.add_query_param('features', features)
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_size(self):
-		return self.get_query_params().get('size')
-
-	def set_size(self,size):
-		self.add_query_param('size',size)
-
-	def get_page(self):
-		return self.get_query_params().get('page')
-
-	def set_page(self,page):
-		self.add_query_param('page',page)
-
-	def get_status(self):
-		return self.get_query_params().get('status')
-
-	def set_status(self,status):
-		self.add_query_param('status',status)
-
-	def get_algorithmId(self):
-		return self.get_query_params().get('algorithmId')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sceneId(self): # String
+		return self.get_query_params().get('sceneId')
+
+	def set_sceneId(self, sceneId):  # String
+		self.add_query_param('sceneId', sceneId)
+	def get_imei(self): # String
+		return self.get_query_params().get('imei')
+
+	def set_imei(self, imei):  # String
+		self.add_query_param('imei', imei)
+	def get_userId(self): # String
+		return self.get_query_params().get('userId')
+
+	def set_userId(self, userId):  # String
+		self.add_query_param('userId', userId)
+	def get_items(self): # String
+		return self.get_query_params().get('items')
 
-	def set_algorithmId(self,algorithmId):
-		self.add_query_param('algorithmId',algorithmId)
+	def set_items(self, items):  # String
+		self.add_query_param('items', items)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListIndexVersionsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListIndexVersionsRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,25 +21,24 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class ListIndexVersionsRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListIndexVersions','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms/[algorithmId]/index-versions')
-		self.set_method('GET')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_algorithmId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_algorithmId(self): # String
 		return self.get_path_params().get('algorithmId')
 
-	def set_algorithmId(self,algorithmId):
-		self.add_path_param('algorithmId',algorithmId)
+	def set_algorithmId(self, algorithmId):  # String
+		self.add_path_param('algorithmId', algorithmId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListInstanceTaskRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListInstanceTaskRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class ListInstanceTaskRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListInstanceTask','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/tasks')
-		self.set_method('GET')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListItemsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/StopDataSetRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,36 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListItemsRequest(RoaRequest):
+class StopDataSetRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListItems','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/items/actions/list')
-		self.set_method('POST')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'StopDataSet','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dataSets/[versionId]/actions/stop')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_versionId(self): # String
+		return self.get_path_params().get('versionId')
 
-	def get_instanceId(self):
+	def set_versionId(self, versionId):  # String
+		self.add_path_param('versionId', versionId)
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_size(self):
-		return self.get_query_params().get('size')
-
-	def set_size(self,size):
-		self.add_query_param('size',size)
-
-	def get_page(self):
-		return self.get_query_params().get('page')
-
-	def set_page(self,page):
-		self.add_query_param('page',page)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListMixCategoriesRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListUmengAppkeysRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListMixCategoriesRequest(RoaRequest):
+class ListUmengAppkeysRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListMixCategories','airec')
-		self.set_uri_pattern('/v2/openapi/configurations/mixCategories')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListUmengAppkeys','airec')
+		self.set_uri_pattern('/v2/openapi/umeng/appkeys')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
+
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListRankingModelsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListRankingModelTemplatesRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,42 +16,34 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListRankingModelsRequest(RoaRequest):
+class ListRankingModelTemplatesRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListRankingModels','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-models')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListRankingModelTemplates','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-model-templates')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_size(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_size(self): # Long
 		return self.get_query_params().get('size')
 
-	def set_size(self,size):
-		self.add_query_param('size',size)
-
-	def get_rankingModelId(self):
-		return self.get_query_params().get('rankingModelId')
-
-	def set_rankingModelId(self,rankingModelId):
-		self.add_query_param('rankingModelId',rankingModelId)
-
-	def get_page(self):
+	def set_size(self, size):  # Long
+		self.add_query_param('size', size)
+	def get_page(self): # Long
 		return self.get_query_params().get('page')
 
-	def set_page(self,page):
-		self.add_query_param('page',page)
+	def set_page(self, page):  # Long
+		self.add_query_param('page', page)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListRuleConditionsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateCustomAnalysisTaskRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,24 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListRuleConditionsRequest(RoaRequest):
+class CreateCustomAnalysisTaskRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListRuleConditions','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/rule-conditions')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateCustomAnalysisTask','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dashboard/custom-analysis-tasks')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_type(self): # String
+		return self.get_query_params().get('type')
+
+	def set_type(self, type):  # String
+		self.add_query_param('type', type)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListRuleTasksRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteRankingModelTemplateRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListRuleTasksRequest(RoaRequest):
+class DeleteRankingModelTemplateRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListRuleTasks','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/rule-tasks')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DeleteRankingModelTemplate','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-model-templates/[templateId]')
+		self.set_method('DELETE')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
-		return self.get_query_params().get('sceneId')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_templateId(self): # String
+		return self.get_path_params().get('templateId')
 
-	def set_sceneId(self,sceneId):
-		self.add_query_param('sceneId',sceneId)
+	def set_templateId(self, templateId):  # String
+		self.add_path_param('templateId', templateId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListRulesRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/RollbackRankingSystemRequest.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,66 +16,34 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListRulesRequest(RoaRequest):
+class RollbackRankingSystemRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListRules','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/rules')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'RollbackRankingSystem','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-systems/[name]/actions/rollback')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_size(self):
-		return self.get_query_params().get('size')
-
-	def set_size(self,size):
-		self.add_query_param('size',size)
-
-	def get_ruleType(self):
-		return self.get_query_params().get('ruleType')
-
-	def set_ruleType(self,ruleType):
-		self.add_query_param('ruleType',ruleType)
-
-	def get_sceneId(self):
-		return self.get_query_params().get('sceneId')
-
-	def set_sceneId(self,sceneId):
-		self.add_query_param('sceneId',sceneId)
-
-	def get_endTime(self):
-		return self.get_query_params().get('endTime')
-
-	def set_endTime(self,endTime):
-		self.add_query_param('endTime',endTime)
-
-	def get_page(self):
-		return self.get_query_params().get('page')
-
-	def set_page(self,page):
-		self.add_query_param('page',page)
-
-	def get_startTime(self):
-		return self.get_query_params().get('startTime')
-
-	def set_startTime(self,startTime):
-		self.add_query_param('startTime',startTime)
-
-	def get_status(self):
-		return self.get_query_params().get('status')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_name(self): # String
+		return self.get_path_params().get('name')
+
+	def set_name(self, name):  # String
+		self.add_path_param('name', name)
+	def get_body(self): # String
+		return self.get_body_params().get('body')
 
-	def set_status(self,status):
-		self.add_query_param('status',status)
+	def set_body(self, body):  # String
+		self.add_body_params('body', body)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListSceneItemsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/QueryRawDataRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,66 +16,54 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListSceneItemsRequest(RoaRequest):
+class QueryRawDataRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListSceneItems','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/items')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'QueryRawData','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/tables/[table]/raw-data')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_itemId(self): # String
+		return self.get_query_params().get('itemId')
 
-	def get_selectionRuleId(self):
-		return self.get_query_params().get('selectionRuleId')
-
-	def set_selectionRuleId(self,selectionRuleId):
-		self.add_query_param('selectionRuleId',selectionRuleId)
-
-	def get_instanceId(self):
+	def set_itemId(self, itemId):  # String
+		self.add_query_param('itemId', itemId)
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_size(self):
-		return self.get_query_params().get('size')
-
-	def set_size(self,size):
-		self.add_query_param('size',size)
-
-	def get_queryCount(self):
-		return self.get_query_params().get('queryCount')
-
-	def set_queryCount(self,queryCount):
-		self.add_query_param('queryCount',queryCount)
-
-	def get_sceneId(self):
-		return self.get_path_params().get('sceneId')
-
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
-
-	def get_operationRuleId(self):
-		return self.get_query_params().get('operationRuleId')
-
-	def set_operationRuleId(self,operationRuleId):
-		self.add_query_param('operationRuleId',operationRuleId)
-
-	def get_previewType(self):
-		return self.get_query_params().get('previewType')
-
-	def set_previewType(self,previewType):
-		self.add_query_param('previewType',previewType)
-
-	def get_page(self):
-		return self.get_query_params().get('page')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_itemType(self): # String
+		return self.get_query_params().get('itemType')
+
+	def set_itemType(self, itemType):  # String
+		self.add_query_param('itemType', itemType)
+	def get_userType(self): # String
+		return self.get_query_params().get('userType')
+
+	def set_userType(self, userType):  # String
+		self.add_query_param('userType', userType)
+	def get_imei(self): # String
+		return self.get_query_params().get('imei')
+
+	def set_imei(self, imei):  # String
+		self.add_query_param('imei', imei)
+	def get_userId(self): # String
+		return self.get_query_params().get('userId')
+
+	def set_userId(self, userId):  # String
+		self.add_query_param('userId', userId)
+	def get_table(self): # String
+		return self.get_path_params().get('table')
 
-	def set_page(self,page):
-		self.add_query_param('page',page)
+	def set_table(self, table):  # String
+		self.add_path_param('table', table)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListSceneParametersRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListSceneParametersRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class ListSceneParametersRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListSceneParameters','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dashboard/scene-parameters')
-		self.set_method('GET')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListScenesRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateRankingModelRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,48 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListScenesRequest(RoaRequest):
+class CreateRankingModelRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListScenes','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateRankingModel','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-models')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_size(self):
-		return self.get_query_params().get('size')
-
-	def set_size(self,size):
-		self.add_query_param('size',size)
-
-	def get_sceneId(self):
-		return self.get_query_params().get('sceneId')
-
-	def set_sceneId(self,sceneId):
-		self.add_query_param('sceneId',sceneId)
-
-	def get_page(self):
-		return self.get_query_params().get('page')
-
-	def set_page(self,page):
-		self.add_query_param('page',page)
-
-	def get_status(self):
-		return self.get_query_params().get('status')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_dryRun(self): # Boolean
+		return self.get_query_params().get('dryRun')
 
-	def set_status(self,status):
-		self.add_query_param('status',status)
+	def set_dryRun(self, dryRun):  # Boolean
+		self.add_query_param('dryRun', dryRun)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListUmengAppkeysRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateDataDiagnoseTaskRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,17 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListUmengAppkeysRequest(RoaRequest):
+class CreateDataDiagnoseTaskRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListUmengAppkeys','airec')
-		self.set_uri_pattern('/v2/openapi/umeng/appkeys')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateDataDiagnoseTask','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/data-diagnose-task')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
+
+	def get_instanceId(self): # String
+		return self.get_path_params().get('instanceId')
+
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ListUserClustersRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyOfflineStoragesRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ListUserClustersRequest(RoaRequest):
+class ModifyOfflineStoragesRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListUserClusters','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/user-clusters')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ModifyOfflineStorages','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/offlineStorages')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ModifyDataSourceRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyRuleRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ModifyDataSourceRequest(RoaRequest):
+class ModifyRuleRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ModifyDataSource','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dataSources/[tableName]')
-		self.set_method('PUT')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ModifyRule','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/rules/[ruleId]')
+		self.set_method('PUT')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_tableName(self):
-		return self.get_path_params().get('tableName')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_ruleId(self): # String
+		return self.get_path_params().get('ruleId')
 
-	def set_tableName(self,tableName):
-		self.add_path_param('tableName',tableName)
+	def set_ruleId(self, ruleId):  # String
+		self.add_path_param('ruleId', ruleId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ModifyFilteringAlgorithmMetaRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyFilteringAlgorithmMetaRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,25 +21,24 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class ModifyFilteringAlgorithmMetaRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ModifyFilteringAlgorithmMeta','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms/[algorithmId]/meta')
-		self.set_method('PUT')
+		self.set_method('PUT')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_algorithmId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_algorithmId(self): # String
 		return self.get_path_params().get('algorithmId')
 
-	def set_algorithmId(self,algorithmId):
-		self.add_path_param('algorithmId',algorithmId)
+	def set_algorithmId(self, algorithmId):  # String
+		self.add_path_param('algorithmId', algorithmId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ModifyInstanceRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateCustomSampleRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ModifyInstanceRequest(RoaRequest):
+class CreateCustomSampleRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ModifyInstance','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]')
-		self.set_method('PUT')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateCustomSample','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/samples')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ModifyItemsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ModifyItemsRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class ModifyItemsRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ModifyItems','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/items')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ModifyRankingModelRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListExperimentsRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ModifyRankingModelRequest(RoaRequest):
+class ListExperimentsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ModifyRankingModel','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-models/[rankingModelId]')
-		self.set_method('PUT')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListExperiments','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiments')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_rankingModelId(self):
-		return self.get_path_params().get('rankingModelId')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sceneId(self): # String
+		return self.get_path_params().get('sceneId')
 
-	def set_rankingModelId(self,rankingModelId):
-		self.add_path_param('rankingModelId',rankingModelId)
+	def set_sceneId(self, sceneId):  # String
+		self.add_path_param('sceneId', sceneId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ModifyRuleRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListSampleFormatConfigsRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ModifyRuleRequest(RoaRequest):
+class ListSampleFormatConfigsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ModifyRule','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/rules/[ruleId]')
-		self.set_method('PUT')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListSampleFormatConfigs','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/samples/[sampleId]/format-configs')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_ruleId(self):
-		return self.get_path_params().get('ruleId')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sampleId(self): # String
+		return self.get_path_params().get('sampleId')
 
-	def set_ruleId(self,ruleId):
-		self.add_path_param('ruleId',ruleId)
+	def set_sampleId(self, sampleId):  # String
+		self.add_path_param('sampleId', sampleId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ModifySceneRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/GetRankingSystemHistoryRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,30 +16,34 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ModifySceneRequest(RoaRequest):
+class GetRankingSystemHistoryRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ModifyScene','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]')
-		self.set_method('PUT')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'GetRankingSystemHistory','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-systems/[name]/histories/[operateId]')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_operateId(self): # String
+		return self.get_path_params().get('operateId')
 
-	def get_sceneId(self):
-		return self.get_path_params().get('sceneId')
+	def set_operateId(self, operateId):  # String
+		self.add_path_param('operateId', operateId)
+	def get_name(self): # String
+		return self.get_path_params().get('name')
 
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
+	def set_name(self, name):  # String
+		self.add_path_param('name', name)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/OfflineFilteringAlgorithmRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/UnLockIndexVersionRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class OfflineFilteringAlgorithmRequest(RoaRequest):
+class UnLockIndexVersionRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'OfflineFilteringAlgorithm','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms/[algorithmId]/actions/offline')
-		self.set_method('POST')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'UnLockIndexVersion','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms/[algorithmId]/actions/unlock')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_algorithmId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_algorithmId(self): # String
 		return self.get_path_params().get('algorithmId')
 
-	def set_algorithmId(self,algorithmId):
-		self.add_path_param('algorithmId',algorithmId)
+	def set_algorithmId(self, algorithmId):  # String
+		self.add_path_param('algorithmId', algorithmId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/PublishRuleRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/UpdateExperimentStatusRequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,42 +16,34 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class PublishRuleRequest(RoaRequest):
+class UpdateExperimentStatusRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'PublishRule','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/rules/[ruleId]/actions/publish')
-		self.set_method('PUT')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'UpdateExperimentStatus','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiments/[experimentId]/status')
+		self.set_method('PUT')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_ruleType(self):
-		return self.get_query_params().get('ruleType')
-
-	def set_ruleType(self,ruleType):
-		self.add_query_param('ruleType',ruleType)
-
-	def get_sceneId(self):
-		return self.get_query_params().get('sceneId')
-
-	def set_sceneId(self,sceneId):
-		self.add_query_param('sceneId',sceneId)
-
-	def get_ruleId(self):
-		return self.get_path_params().get('ruleId')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sceneId(self): # String
+		return self.get_path_params().get('sceneId')
+
+	def set_sceneId(self, sceneId):  # String
+		self.add_path_param('sceneId', sceneId)
+	def get_experimentId(self): # String
+		return self.get_path_params().get('experimentId')
 
-	def set_ruleId(self,ruleId):
-		self.add_path_param('ruleId',ruleId)
+	def set_experimentId(self, experimentId):  # String
+		self.add_path_param('experimentId', experimentId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/PushDocumentRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/PushDocumentRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,25 +21,24 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class PushDocumentRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'PushDocument','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/tables/[tableName]/actions/bulk')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_tableName(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_tableName(self): # String
 		return self.get_path_params().get('tableName')
 
-	def set_tableName(self,tableName):
-		self.add_path_param('tableName',tableName)
+	def set_tableName(self, tableName):  # String
+		self.add_path_param('tableName', tableName)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/PushInterventionRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/PushInterventionRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class PushInterventionRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'PushIntervention','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/actions/intervene')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/QueryDataMessageRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/QueryDataMessageStatisticsRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,108 +16,89 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class QueryDataMessageRequest(RoaRequest):
+class QueryDataMessageStatisticsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'QueryDataMessage','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/tables/[table]/data-message')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'QueryDataMessageStatistics','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/tables/[table]/data-message-statistics')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_traceId(self):
+	def get_traceId(self): # String
 		return self.get_query_params().get('traceId')
 
-	def set_traceId(self,traceId):
-		self.add_query_param('traceId',traceId)
-
-	def get_messageSource(self):
+	def set_traceId(self, traceId):  # String
+		self.add_query_param('traceId', traceId)
+	def get_messageSource(self): # String
 		return self.get_query_params().get('messageSource')
 
-	def set_messageSource(self,messageSource):
-		self.add_query_param('messageSource',messageSource)
-
-	def get_endTime(self):
+	def set_messageSource(self, messageSource):  # String
+		self.add_query_param('messageSource', messageSource)
+	def get_endTime(self): # Long
 		return self.get_query_params().get('endTime')
 
-	def set_endTime(self,endTime):
-		self.add_query_param('endTime',endTime)
-
-	def get_userType(self):
+	def set_endTime(self, endTime):  # Long
+		self.add_query_param('endTime', endTime)
+	def get_userType(self): # String
 		return self.get_query_params().get('userType')
 
-	def set_userType(self,userType):
-		self.add_query_param('userType',userType)
-
-	def get_startTime(self):
+	def set_userType(self, userType):  # String
+		self.add_query_param('userType', userType)
+	def get_startTime(self): # Long
 		return self.get_query_params().get('startTime')
 
-	def set_startTime(self,startTime):
-		self.add_query_param('startTime',startTime)
-
-	def get_userId(self):
+	def set_startTime(self, startTime):  # Long
+		self.add_query_param('startTime', startTime)
+	def get_userId(self): # String
 		return self.get_query_params().get('userId')
 
-	def set_userId(self,userId):
-		self.add_query_param('userId',userId)
-
-	def get_itemId(self):
+	def set_userId(self, userId):  # String
+		self.add_query_param('userId', userId)
+	def get_itemId(self): # String
 		return self.get_query_params().get('itemId')
 
-	def set_itemId(self,itemId):
-		self.add_query_param('itemId',itemId)
-
-	def get_instanceId(self):
+	def set_itemId(self, itemId):  # String
+		self.add_query_param('itemId', itemId)
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_itemType(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_itemType(self): # String
 		return self.get_query_params().get('itemType')
 
-	def set_itemType(self,itemType):
-		self.add_query_param('itemType',itemType)
-
-	def get_cmdType(self):
+	def set_itemType(self, itemType):  # String
+		self.add_query_param('itemType', itemType)
+	def get_cmdType(self): # String
 		return self.get_query_params().get('cmdType')
 
-	def set_cmdType(self,cmdType):
-		self.add_query_param('cmdType',cmdType)
-
-	def get_size(self):
-		return self.get_query_params().get('size')
-
-	def set_size(self,size):
-		self.add_query_param('size',size)
-
-	def get_sceneId(self):
+	def set_cmdType(self, cmdType):  # String
+		self.add_query_param('cmdType', cmdType)
+	def get_sceneId(self): # String
 		return self.get_query_params().get('sceneId')
 
-	def set_sceneId(self,sceneId):
-		self.add_query_param('sceneId',sceneId)
-
-	def get_bhvType(self):
+	def set_sceneId(self, sceneId):  # String
+		self.add_query_param('sceneId', sceneId)
+	def get_imei(self): # String
+		return self.get_query_params().get('imei')
+
+	def set_imei(self, imei):  # String
+		self.add_query_param('imei', imei)
+	def get_bhvType(self): # String
 		return self.get_query_params().get('bhvType')
 
-	def set_bhvType(self,bhvType):
-		self.add_query_param('bhvType',bhvType)
-
-	def get_page(self):
-		return self.get_query_params().get('page')
-
-	def set_page(self,page):
-		self.add_query_param('page',page)
-
-	def get_table(self):
+	def set_bhvType(self, bhvType):  # String
+		self.add_query_param('bhvType', bhvType)
+	def get_table(self): # String
 		return self.get_path_params().get('table')
 
-	def set_table(self,table):
-		self.add_path_param('table',table)
+	def set_table(self, table):  # String
+		self.add_path_param('table', table)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/QueryDataMessageStatisticsRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/RecommendRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,96 +16,84 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class QueryDataMessageStatisticsRequest(RoaRequest):
+class RecommendRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'QueryDataMessageStatistics','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/tables/[table]/data-message-statistics')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'Recommend','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/actions/recommend')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_returnCount(self): # Integer
+		return self.get_query_params().get('returnCount')
 
-	def get_traceId(self):
-		return self.get_query_params().get('traceId')
-
-	def set_traceId(self,traceId):
-		self.add_query_param('traceId',traceId)
-
-	def get_messageSource(self):
-		return self.get_query_params().get('messageSource')
-
-	def set_messageSource(self,messageSource):
-		self.add_query_param('messageSource',messageSource)
-
-	def get_endTime(self):
-		return self.get_query_params().get('endTime')
-
-	def set_endTime(self,endTime):
-		self.add_query_param('endTime',endTime)
-
-	def get_userType(self):
-		return self.get_query_params().get('userType')
-
-	def set_userType(self,userType):
-		self.add_query_param('userType',userType)
-
-	def get_startTime(self):
-		return self.get_query_params().get('startTime')
-
-	def set_startTime(self,startTime):
-		self.add_query_param('startTime',startTime)
-
-	def get_userId(self):
+	def set_returnCount(self, returnCount):  # Integer
+		self.add_query_param('returnCount', returnCount)
+	def get_recType(self): # String
+		return self.get_query_params().get('recType')
+
+	def set_recType(self, recType):  # String
+		self.add_query_param('recType', recType)
+	def get_ip(self): # String
+		return self.get_query_params().get('ip')
+
+	def set_ip(self, ip):  # String
+		self.add_query_param('ip', ip)
+	def get_userId(self): # String
 		return self.get_query_params().get('userId')
 
-	def set_userId(self,userId):
-		self.add_query_param('userId',userId)
-
-	def get_itemId(self):
-		return self.get_query_params().get('itemId')
-
-	def set_itemId(self,itemId):
-		self.add_query_param('itemId',itemId)
-
-	def get_instanceId(self):
+	def set_userId(self, userId):  # String
+		self.add_query_param('userId', userId)
+	def get_filter(self): # String
+		return self.get_query_params().get('filter')
+
+	def set_filter(self, filter):  # String
+		self.add_query_param('filter', filter)
+	def get_serviceType(self): # String
+		return self.get_query_params().get('serviceType')
+
+	def set_serviceType(self, serviceType):  # String
+		self.add_query_param('serviceType', serviceType)
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_itemType(self):
-		return self.get_query_params().get('itemType')
-
-	def set_itemType(self,itemType):
-		self.add_query_param('itemType',itemType)
-
-	def get_cmdType(self):
-		return self.get_query_params().get('cmdType')
-
-	def set_cmdType(self,cmdType):
-		self.add_query_param('cmdType',cmdType)
-
-	def get_sceneId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sceneId(self): # String
 		return self.get_query_params().get('sceneId')
 
-	def set_sceneId(self,sceneId):
-		self.add_query_param('sceneId',sceneId)
-
-	def get_bhvType(self):
-		return self.get_query_params().get('bhvType')
-
-	def set_bhvType(self,bhvType):
-		self.add_query_param('bhvType',bhvType)
-
-	def get_table(self):
-		return self.get_path_params().get('table')
+	def set_sceneId(self, sceneId):  # String
+		self.add_query_param('sceneId', sceneId)
+	def get_imei(self): # String
+		return self.get_query_params().get('imei')
+
+	def set_imei(self, imei):  # String
+		self.add_query_param('imei', imei)
+	def get_rankOpen(self): # Boolean
+		return self.get_query_params().get('rankOpen')
+
+	def set_rankOpen(self, rankOpen):  # Boolean
+		self.add_query_param('rankOpen', rankOpen)
+	def get_strategy(self): # String
+		return self.get_query_params().get('strategy')
+
+	def set_strategy(self, strategy):  # String
+		self.add_query_param('strategy', strategy)
+	def get_items(self): # String
+		return self.get_query_params().get('items')
+
+	def set_items(self, items):  # String
+		self.add_query_param('items', items)
+	def get_userInfo(self): # String
+		return self.get_query_params().get('userInfo')
 
-	def set_table(self,table):
-		self.add_path_param('table',table)
+	def set_userInfo(self, userInfo):  # String
+		self.add_query_param('userInfo', userInfo)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/QueryExceptionHistoryRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CloneSampleRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,42 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class QueryExceptionHistoryRequest(RoaRequest):
+class CloneSampleRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'QueryExceptionHistory','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/sync-reports/exception-history')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CloneSample','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/samples/[sampleId]/actions/clone')
+		self.set_method('PUT')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_endTime(self):
-		return self.get_query_params().get('endTime')
-
-	def set_endTime(self,endTime):
-		self.add_query_param('endTime',endTime)
-
-	def get_startTime(self):
-		return self.get_query_params().get('startTime')
-
-	def set_startTime(self,startTime):
-		self.add_query_param('startTime',startTime)
-
-	def get_type(self):
-		return self.get_query_params().get('type')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sampleId(self): # String
+		return self.get_path_params().get('sampleId')
 
-	def set_type(self,type):
-		self.add_query_param('type',type)
+	def set_sampleId(self, sampleId):  # String
+		self.add_path_param('sampleId', sampleId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/QuerySingleAggregationReportRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateFlowControlTaskRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,24 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class QuerySingleAggregationReportRequest(RoaRequest):
+class CreateFlowControlTaskRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'QuerySingleAggregationReport','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/sync-reports/single-aggregation-report')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateFlowControlTask','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/flowControlTasks')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_dryRun(self): # Boolean
+		return self.get_query_params().get('dryRun')
+
+	def set_dryRun(self, dryRun):  # Boolean
+		self.add_query_param('dryRun', dryRun)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/QuerySingleReportRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/QuerySingleReportRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,25 +21,24 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class QuerySingleReportRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'QuerySingleReport','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/sync-reports/single-report')
-		self.set_method('GET')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_reportType(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_reportType(self): # String
 		return self.get_query_params().get('reportType')
 
-	def set_reportType(self,reportType):
-		self.add_query_param('reportType',reportType)
+	def set_reportType(self, reportType):  # String
+		self.add_query_param('reportType', reportType)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/QuerySyncReportAggregationRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/QuerySyncReportAggregationRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,31 +21,29 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class QuerySyncReportAggregationRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'QuerySyncReportAggregation','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/sync-reports/aggregation')
-		self.set_method('GET')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_endTime(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_endTime(self): # Long
 		return self.get_query_params().get('endTime')
 
-	def set_endTime(self,endTime):
-		self.add_query_param('endTime',endTime)
-
-	def get_startTime(self):
+	def set_endTime(self, endTime):  # Long
+		self.add_query_param('endTime', endTime)
+	def get_startTime(self): # Long
 		return self.get_query_params().get('startTime')
 
-	def set_startTime(self,startTime):
-		self.add_query_param('startTime',startTime)
+	def set_startTime(self, startTime):  # Long
+		self.add_query_param('startTime', startTime)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/RebuildIndexRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/RebuildIndexRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,25 +21,24 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class RebuildIndexRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'RebuildIndex','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms/[algorithmId]/actions/rebuild')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_algorithmId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_algorithmId(self): # String
 		return self.get_path_params().get('algorithmId')
 
-	def set_algorithmId(self,algorithmId):
-		self.add_path_param('algorithmId',algorithmId)
+	def set_algorithmId(self, algorithmId):  # String
+		self.add_path_param('algorithmId', algorithmId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/RunInstanceRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/RunInstanceRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from aliyunsdkairec.endpoint import endpoint_data
 
 class RunInstanceRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'RunInstance','airec')
 		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/actions/import')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/StopDataSetRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/GetRankingModelVersionRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class StopDataSetRequest(RoaRequest):
+class GetRankingModelVersionRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'StopDataSet','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/dataSets/[versionId]/actions/stop')
-		self.set_method('POST')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'GetRankingModelVersion','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-model-versions/[versionId]')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_versionId(self):
+	def get_versionId(self): # String
 		return self.get_path_params().get('versionId')
 
-	def set_versionId(self,versionId):
-		self.add_path_param('versionId',versionId)
-
-	def get_instanceId(self):
+	def set_versionId(self, versionId):  # String
+		self.add_path_param('versionId', versionId)
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/UnLockIndexVersionRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DescribeLatestTaskRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class UnLockIndexVersionRequest(RoaRequest):
+class DescribeLatestTaskRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'UnLockIndexVersion','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms/[algorithmId]/actions/unlock')
-		self.set_method('POST')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DescribeLatestTask','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/filtering-algorithms/[algorithmId]/tasks/latest')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_algorithmId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_algorithmId(self): # String
 		return self.get_path_params().get('algorithmId')
 
-	def set_algorithmId(self,algorithmId):
-		self.add_path_param('algorithmId',algorithmId)
+	def set_algorithmId(self, algorithmId):  # String
+		self.add_path_param('algorithmId', algorithmId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/UpdateExperimentBasicInfoRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteSampleRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,36 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class UpdateExperimentBasicInfoRequest(RoaRequest):
+class DeleteSampleRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'UpdateExperimentBasicInfo','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiments/[experimentId]/basic')
-		self.set_method('PUT')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DeleteSample','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/samples/[sampleId]')
+		self.set_method('DELETE')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
-		return self.get_path_params().get('sceneId')
-
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
-
-	def get_experimentId(self):
-		return self.get_path_params().get('experimentId')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sampleId(self): # String
+		return self.get_path_params().get('sampleId')
 
-	def set_experimentId(self,experimentId):
-		self.add_path_param('experimentId',experimentId)
+	def set_sampleId(self, sampleId):  # String
+		self.add_path_param('sampleId', sampleId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/UpdateExperimentConfigRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListSamplesRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,36 +16,39 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class UpdateExperimentConfigRequest(RoaRequest):
+class ListSamplesRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'UpdateExperimentConfig','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiments/[experimentId]/config')
-		self.set_method('PUT')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListSamples','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/samples')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
-		return self.get_path_params().get('sceneId')
-
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
-
-	def get_experimentId(self):
-		return self.get_path_params().get('experimentId')
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_size(self): # Long
+		return self.get_query_params().get('size')
+
+	def set_size(self, size):  # Long
+		self.add_query_param('size', size)
+	def get_sampleId(self): # String
+		return self.get_query_params().get('sampleId')
+
+	def set_sampleId(self, sampleId):  # String
+		self.add_query_param('sampleId', sampleId)
+	def get_page(self): # Long
+		return self.get_query_params().get('page')
 
-	def set_experimentId(self,experimentId):
-		self.add_path_param('experimentId',experimentId)
+	def set_page(self, page):  # Long
+		self.add_query_param('page', page)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/UpdateExperimentStatusRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/DeleteExperimentRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,36 +16,34 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class UpdateExperimentStatusRequest(RoaRequest):
+class DeleteExperimentRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'UpdateExperimentStatus','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiments/[experimentId]/status')
-		self.set_method('PUT')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'DeleteExperiment','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/scenes/[sceneId]/experiments/[experimentId]')
+		self.set_method('DELETE')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
-
-	def get_sceneId(self):
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
+	def get_sceneId(self): # String
 		return self.get_path_params().get('sceneId')
 
-	def set_sceneId(self,sceneId):
-		self.add_path_param('sceneId',sceneId)
-
-	def get_experimentId(self):
+	def set_sceneId(self, sceneId):  # String
+		self.add_path_param('sceneId', sceneId)
+	def get_experimentId(self): # String
 		return self.get_path_params().get('experimentId')
 
-	def set_experimentId(self,experimentId):
-		self.add_path_param('experimentId',experimentId)
+	def set_experimentId(self, experimentId):  # String
+		self.add_path_param('experimentId', experimentId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/UpgradeInstanceRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/ListOfflineStoragesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class UpgradeInstanceRequest(RoaRequest):
+class ListOfflineStoragesRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'UpgradeInstance','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/actions/upgrade')
-		self.set_method('POST')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ListOfflineStorages','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/offlineStorages')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/aliyunsdkairec/request/v20201126/ValidateInstanceRequest.py` & `aliyun-python-sdk-airec-2.1.0/aliyunsdkairec/request/v20201126/CreateRankingSystemRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdkairec.endpoint import endpoint_data
 
-class ValidateInstanceRequest(RoaRequest):
+class CreateRankingSystemRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'ValidateInstance','airec')
-		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/actions/validate')
-		self.set_method('POST')
+		RoaRequest.__init__(self, 'Airec', '2020-11-26', 'CreateRankingSystem','airec')
+		self.set_uri_pattern('/v2/openapi/instances/[instanceId]/ranking-systems')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_instanceId(self):
+	def get_instanceId(self): # String
 		return self.get_path_params().get('instanceId')
 
-	def set_instanceId(self,instanceId):
-		self.add_path_param('instanceId',instanceId)
+	def set_instanceId(self, instanceId):  # String
+		self.add_path_param('instanceId', instanceId)
```

### Comparing `aliyun-python-sdk-airec-2.0.1/setup.py` & `aliyun-python-sdk-airec-2.1.0/setup.py`

 * *Files identical despite different names*

